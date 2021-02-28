[42. 接雨水](https://leetcode-cn.com/problems/trapping-rain-water/)

给定 n 个非负整数表示每个宽度为 1 的柱子的高度图，计算按此排列的柱子，下雨之后能接多少雨水。

**示例 1：**

![rainwatertrap](./img/rainwatertrap.png)

```
输入：height = [0,1,0,2,1,0,1,3,2,1,2,1]
输出：6
解释：上面是由数组 [0,1,0,2,1,0,1,3,2,1,2,1] 表示的高度图，在这种情况下，可以接 6 个单位的雨水（蓝色部分表示雨水）。 
```

**示例 2：**

```
输入：height = [4,2,0,3,2,5]
输出：9
```

**提示：**

> * `n == height.length`
> * `0 <= n <= 3 * 104`
> * `0 <= height[i] <= 105`


## 解题思路

黑色的看成墙，蓝色的看成水，单位一样，给定一个数组，每个数表示墙的高度，求出能装多少单位的水，也就是图中蓝色正方形的个数。

### 解法一：暴力法，枚举列

求每一列的水，只需关注当前列，以及左边最高的墙和右边最高的墙。

装水量，根据木桶理论，只需要知道左边的墙和右边的墙中的较矮的即可。

代码如下：

```swift
func trap(_ height: [Int]) -> Int {
	var sum = 0
	if height.count > 2 {
	    for i in 1 ... height.count - 2 {
	        // 求左边最高
	        var leftMax = 0
	        for j in 0 ... i - 1 {
	            leftMax = max(leftMax, height[j])
	        }
	        
	        // 求右边最高
	        var rightMax = 0
	        for j in i + 1 ... height.count - 1 {
	            rightMax = max(rightMax, height[j])
	        }
	        
	        if min(leftMax, rightMax) > height[i] {
	            sum += (min(leftMax, rightMax) - height[i])
	        }
	    }
	}
	return sum
}
```
该解法，时间复杂度为 O(n²），在 LeetCode 上无法 AC。


### 解法二：动态规划

解法一中，对于每一列，求其最左边及最右边高度的时候，都需要重新遍历一次数组，这里可以优化一下。

首先用两个数组 `maxLeft` 和 `maxRight`，`maxLeft[i]` 表示第 `i` 列左边最高的墙的高度，`maxRight[i]` 表示第 `i` 列右边最高的墙的高度。

那么对于 `maxLeft` 有动态转移方程 `maxLeft[i] = max(maxLeft[i - 1], height[i - 1])`，它前边的墙的左边的最大高度和前边的墙的高度中选一个较大的，就是当前列左边最高的墙了。

对于 `maxRight` 有动态转移方程 `maxRight[i] = max(maxLeft[i + 1], height[i + 1])`，它后边的墙的右边的最大高度和后边的墙的高度中选一个较大的，就是当前列右边最高的墙了。

然后根据解法一，就可以得到能接的雨水量了：

```swift
func trap(_ height: [Int]) -> Int {
	var sum = 0
	if height.count > 2 {
	    var maxLeft = [Int](repeating: 0, count: height.count)
	    for i in 1 ... height.count - 1 {
	        maxLeft[i] = max(maxLeft[i - 1], height[i - 1])
	    }
	    
	    var maxRight = [Int](repeating: 0, count: height.count)
	    for i in (0 ... height.count - 2).reversed() {
	        maxRight[i] = max(maxRight[i + 1], height[i + 1])
	    }
	    
	    for i in 1 ... height.count - 2 {
	        if min(maxLeft[i], maxRight[i]) > height[i] {
	            sum += (min(maxLeft[i], maxRight[i]) - height[i])
	        }
	    }
	}
	    
	return sum
}
```

### 解法三：双指针

动态规划中，常可以对空间复杂度进行优化，如本题，由于 `maxLeft[i]` 和 `maxRight[i]` 的值只会用到一次，所以可以不用数组，只用一个元素就行了。首先，改造一下 `maxLeft`。

```swift
func trap(_ height: [Int]) -> Int {
	var sum = 0
	let n = height.count
	guard n > 2 else { return sum }
	var maxLeft = 0
	var maxRight = [Int](repeating: 0, count: n)
	for i in (1 ... n - 2).reversed() {
	    maxRight[i] = max(maxRight[i + 1], height[i + 1])
	}
	for i in 1 ... n - 2 {
	    maxLeft = max(maxLeft, height[i - 1])
	    let minVal = min(maxLeft, maxRight[i])
	    if minVal > height[i] {
	        sum += (minVal - height[i])
	    }
	}
	return sum
}
``` 

这里成功将 `maxLeft` 数组去掉了，但是发现不能同时将 `maxRight` 去掉，因为最后求 `sum` 的 `for` 循环是从左往右遍历的，但是求 `maxRight` 是需要从右往左遍历的，所以，这里需要用到两个指针 `left` 和 `right`，从两个方向去遍历。

```swift
func trap(_ height: [Int]) -> Int {
	var sum = 0
	let n = height.count
	guard n > 2 else { return sum }
	var left = 1, right = n - 1
	var maxLeft = 0, maxRight = 0
	for _ in 1 ... n - 2 {
	    // 从左到右更新
	    if height[left - 1] < height[right + 1] {
	        maxLeft = max(maxLeft, height[left - 1])
	        if maxLeft > height[left] {
	            sum += (maxLeft - height[left])
	        }
	        left += 1
	    } else {    // 从右到左更新
	        maxRight = max(maxRight, height[right + 1])
	        if maxRight > height[right] {
	            sum += (maxRight - height[right])
	        }
	        right -= 1
	    }
	}
	return sum
}
```

### 解法四：栈

说到栈，肯定会想到括号匹配。仔细观察蓝色部分，可以和括号匹配进行类比。每次匹配出一对括号(找到对应的一堵墙)，就计算这两堵墙中的水。

![rainwatertrapstack](./img/rainwatertrapstack.png)

用栈保存每堵墙，当遍历墙的高度时，若当前高度小于栈顶的墙高度，说明这里会有积水，将墙的高度的下标入栈，如果当前高度大于栈顶的墙高度，说明之前的积水到这里停下了，就可以计算有多少积水了。计算完，就把墙的高度的下标入栈，作为新的积水的墙。

总体原则是：

1. 当前高度小于等于栈顶高度，入栈，指针后移
2. 当前高度大于栈顶高度，出栈，计算出当前墙和栈顶的墙之间的水量，然后比较当前高度和新的栈顶高度，重复第 2 步，直到当前高度不大于栈顶高度或者栈为空，然后把当前墙入栈，指针后移

```swift
func trap(_ height: [Int]) -> Int {
	var sum = 0
	let n = height.count
	guard n > 2 else { return sum }
	var stack = [Int]()
	var index = 0
	while index < n {
	    // 如果栈不空并且当前指向的高度大于栈顶高度就一直循环
	    while !stack.isEmpty && height[index] > height[stack.last!] {
	        // 要出栈的元素
	        let h = height[stack.removeLast()]
	        if stack.isEmpty {
	            break
	        }
	        // 两堵墙之间的距离
	        let distance = index - stack.last! - 1
	        // 当前墙与新的栈顶，取较小值，计算墙之间的水量
	        let minVal = min(height[stack.last!], height[index])
	        sum += distance * (minVal - h)
	    }
	    // 当前墙入栈
	    stack.append(index)
	    // 指针后移
	    index += 1
	}
	return sum
}
```

注：本文参考 [https://leetcode-cn.com/problems/trapping-rain-water/solution/xiang-xi-tong-su-de-si-lu-fen-xi-duo-jie-fa-by-w-8/](https://leetcode-cn.com/problems/trapping-rain-water/solution/xiang-xi-tong-su-de-si-lu-fen-xi-duo-jie-fa-by-w-8/)
