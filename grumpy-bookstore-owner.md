[1052. 爱生气的书店老板](https://leetcode-cn.com/problems/grumpy-bookstore-owner/)

今天，书店老板有一家店打算试营业 `customers.length` 分钟。每分钟都有一些顾客（`customers[i]`）会进入书店，所有这些顾客都会在那一分钟结束后离开。

在某些时候，书店老板会生气。 如果书店老板在第 i 分钟生气，那么 `grumpy[i] = 1`，否则 `grumpy[i] = 0`。 当书店老板生气时，那一分钟的顾客就会不满意，不生气则他们是满意的。

书店老板知道一个秘密技巧，能抑制自己的情绪，可以让自己连续 `X` 分钟不生气，但却只能使用一次。

请你返回这一天营业下来，最多有多少客户能够感到满意的数量。
 

示例：

```
输入：customers = [1,0,1,2,1,1,7,5], grumpy = [0,1,0,1,0,1,0,1], X = 3
输出：16
解释：
书店老板在最后 3 分钟保持冷静。
感到满意的最大客户数量 = 1 + 1 + 1 + 1 + 7 + 5 = 16.
```

提示：

>  * 1 <= X <= customers.length == grumpy.length <= 20000

> * 0 <= customers[i] <= 1000

> * 0 <= grumpy[i] <= 1

解答：

1.  求出不使用秘密技巧时的总满意数量 `total`
2. 求出从 `0` 开始，大小为 `K` 的窗口内，使用秘密技巧时能增加的满意量 `increase`
3. 滑动窗口，求出使用秘密技巧时能增加的最大满意量 `maxIncrease`
4. 结果为 `total + maxIncrease`

```swift
func maxSatisfied(_ customers: [Int], _ grumpy: [Int], _ X: Int) -> Int {
    let n = customers.count
    // total 为不使用秘密技巧时的满意量
    var total = 0
    for i in 0 ..< n {
        if 0 == grumpy[i] {
            total += customers[i]
        }
    }
    // increase 为使用秘密技巧时能增加的满意量
    var increase = 0
    for i in 0 ..< X {
        // grumpy[i] 为 1 时，customers[i] * grumpy[i] 即为使用秘密技巧后可增加的满意量
        increase += customers[i] * grumpy[i]
    }
    // 使用滑动窗口求出使用秘密技巧能增加的最大满意量
    var maxIncrease = increase
    for i in X ..< n {
        // customers[i - X] * grumpy[i - X] 为滑动窗口的第一个值，需减去，customers[i] * grumpy[i] 为刚刚进入滑动窗口的值，需加上
        increase = increase - customers[i - X] * grumpy[i - X] + customers[i] * grumpy[i]
        maxIncrease = max(maxIncrease, increase)
    }
    return total + maxIncrease
}
```


