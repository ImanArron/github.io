---
title: 算法学习路线
type: 算法学习路线
order: 0
---

## 时间服务度和空间复杂度分析

[如何理解算法时间复杂度的表示法](http://www.zhihu.com/question/21387264)

[Master theorem](http://en.wikipedia.org/wiki/Master_theorem_(analysis_of_algorithms))

[主定理](http://zh.wikipedia.org/wiki/%E4%B8%BB%E5%AE%9A%E7%90%86)

[数据结构与算法总览](https://pan.baidu.com/s/1rucC3q-9zD-lzs3yBkFU_g)（提取码：ykyn）
	
## 数组、链表、跳表

1. 数组、链表、跳表的基本实现和特性
	
	[Java 源码分析（ArrayList）](http://developer.classpath.org/doc/java/util/ArrayList-source.html)
	
	[Linked List 的标准实现代码](https://www.geeksforgeeks.org/implementing-a-linked-list-in-java-using-class/)
	
	[Linked List 示例代码](http://www.cs.cmu.edu/~adamchik/15-121/lectures/Linked%20Lists/code/LinkedList.java)
	
	[Java 源码分析（LinkedList）](http://developer.classpath.org/doc/java/util/LinkedList-source.html)
	
	LRU Cache - Linked list： [LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache/)
	
	Redis - Skip List：[跳跃表](https://redisbook.readthedocs.io/en/latest/internal-datastruct/skiplist.html)、[为啥 Redis 使用跳表（Skip List）而不是使用 Red-Black？](https://www.zhihu.com/question/20202931)

2.  Array 实战题目

	[两数之和](https://leetcode-cn.com/problems/two-sum/)（近半年内，字节跳动在面试中考查此题达到 152 次）
	
	[盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water/)（腾讯、百度、字节跳动在近半年内面试常考）
	
	[移动零](https://leetcode-cn.com/problems/move-zeroes/)（华为、字节跳动在近半年内面试常考）
	
	[爬楼梯](https://leetcode.com/problems/climbing-stairs/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[三数之和](https://leetcode-cn.com/problems/3sum/)（国内、国际大厂历年面试高频老题）
	
3. Linked List 实战题目

	[反转链表](https://leetcode.com/problems/reverse-linked-list/)（字节跳动、亚马逊在半年内面试常考）
	
	[两两交换链表中的节点](https://leetcode.com/problems/swap-nodes-in-pairs)（阿里巴巴、字节跳动在半年内面试常考）
	
	[环形链表](https://leetcode.com/problems/linked-list-cycle)（阿里巴巴、字节跳动、腾讯在半年内面试常考）
	
	[环形链表 II](https://leetcode.com/problems/linked-list-cycle-ii)
	
	[K 个一组翻转链表](https://leetcode.com/problems/reverse-nodes-in-k-group/)（字节跳动、猿辅导在半年内面试常考）

## 栈、队列、优先队列、双端队列

1. 栈和队列的实现与特性

	[Java 的 PriorityQueue 文档](https://docs.oracle.com/javase/10/docs/api/java/util/PriorityQueue.html)
	
	[Java 的 Stack 源码](http://developer.classpath.org/doc/java/util/Stack-source.html)
	
	[Java 的 Queue 源码](http://fuseyism.com/classpath/doc/java/util/Queue-source.html)
	
	[Python 的 heapq](http://docs.python.org/2/library/heapq.html)
	
	[高性能的 container 库](http://docs.python.org/2/library/collections.html)

2.  实战题目

	[有效的括号](https://leetcode-cn.com/problems/valid-parentheses/)（亚马逊、JPMorgan 在半年内面试常考）
	
	[最小栈](https://leetcode-cn.com/problems/min-stack/)（亚马逊在半年内面试常考）
	
	[柱状图中最大的矩形](https://leetcode-cn.com/problems/largest-rectangle-in-histogram)（亚马逊、微软、字节跳动在半年内面试中考过）
	
	[滑动窗口最大值](https://leetcode-cn.com/problems/sliding-window-maximum)（亚马逊在半年内面试常考）
	
	[设计循环双端队列](https://leetcode.com/problems/design-circular-deque)（Facebook 在 1 年内面试中考过）
	
	[接雨水](https://leetcode.com/problems/trapping-rain-water/)（亚马逊、字节跳动、高盛集团、Facebook 在半年内面试常考）
	
	[删除排序数组中的重复项](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array/)（Facebook、字节跳动、微软在半年内面试中考过）
	
	[旋转数组](https://leetcode-cn.com/problems/rotate-array/)（微软、亚马逊、PayPal 在半年内面试中考过）
	
	[合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists/)（亚马逊、字节跳动在半年内面试常考）
	
	[合并两个有序数组](https://leetcode-cn.com/problems/merge-sorted-array/)（Facebook 在半年内面试常考）
	
	[加一](https://leetcode-cn.com/problems/plus-one/)（谷歌、字节跳动、Facebook 在半年内面试中考过）
	
	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/description/)
	
	[二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/)
	
	[最小的 k 个数](https://leetcode-cn.com/problems/zui-xiao-de-kge-shu-lcof/)
	
## 哈希表、映射、集合

1. 哈希表、映射、集合的实现与特性

	[Java Set 文档](http://docs.oracle.com/en/java/javase/12/docs/api/java.base/java/util/Set.html)
	
	[Java Map 文档](http://docs.oracle.com/en/java/javase/12/docs/api/java.base/java/util/Map.html)
	
2. 实战题目

	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/description/)（亚马逊、Facebook、谷歌在半年内面试中考过）
	
	[字母异位词分组](https://leetcode-cn.com/problems/group-anagrams/)（亚马逊在半年内面试中常考）
	
	[两数之和](https://leetcode-cn.com/problems/two-sum/description/)（亚马逊、字节跳动、谷歌、Facebook、苹果、微软、腾讯在半年内面试中常考）
	
3. 养成收藏精选代码的好习惯

	[养成收藏精选代码的习惯（示例）](http://shimo.im/docs/R6g9WJV89QkHrDhr)
	
## 树、二叉树、二叉搜索树

1. 树、二叉树、二叉搜索树的实现与特性

	[二叉搜索树 Demo](https://visualgo.net/zh/bst)
	
2. 树的面试题解法一般都是递归，为什么？

3.  实战题目
	
	[二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/)（亚马逊、微软、字节跳动在半年内面试中考过）
	
	[二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal/)（谷歌、微软、字节跳动在半年内面试中考过）
	
	[N 叉树的后序遍历](https://leetcode-cn.com/problems/n-ary-tree-postorder-traversal/)（亚马逊在半年内面试中考过）
	
	[N 叉树的前序遍历](https://leetcode-cn.com/problems/n-ary-tree-preorder-traversal/description/)（亚马逊在半年内面试中考过）
	
	[N 叉树的层序遍历](https://leetcode-cn.com/problems/n-ary-tree-level-order-traversal/)
	
## 堆和二叉堆、图

1. 堆和二叉堆的实现和特性

	[维基百科：堆（Heap）](https://en.wikipedia.org/wiki/Heap_(data_structure))
	
	堆的实现代码： [https://shimo.im/docs/Lw86vJzOGOMpWZz2/](https://shimo.im/docs/Lw86vJzOGOMpWZz2/)
	
2. 图的实现和特性

	连通图个数： [https://leetcode-cn.com/problems/number-of-islands/](https://leetcode-cn.com/problems/number-of-islands/)

	拓扑排序（Topological Sorting）： [https://zhuanlan.zhihu.com/p/34871092](https://zhuanlan.zhihu.com/p/34871092)
	
	最短路径（Shortest Path）：Dijkstra [https://www.bilibili.com/video/av25829980?from=search&seid=13391343514095937158](https://www.bilibili.com/video/av25829980?from=search&seid=13391343514095937158)
	
	最小生成树（Minimum Spanning Tree）： [https://www.bilibili.com/video/av84820276?from=search&seid=17476598104352152051](https://www.bilibili.com/video/av84820276?from=search&seid=17476598104352152051)
	
3. 实战题目

	[最小的 k 个数](https://leetcode-cn.com/problems/zui-xiao-de-kge-shu-lcof/)（字节跳动在半年内面试中考过）
	
	[滑动窗口最大值](https://leetcode-cn.com/problems/sliding-window-maximum/)（亚马逊在半年内面试中常考）
	
	HeapSort ：自学 [https://www.geeksforgeeks.org/heap-sort/](https://www.geeksforgeeks.org/heap-sort/)
	
	[丑数](https://leetcode-cn.com/problems/chou-shu-lcof/)（字节跳动在半年内面试中考过）
	
	[前 K 个高频元素](https://leetcode-cn.com/problems/top-k-frequent-elements/)（亚马逊在半年内面试中常考）
	
	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/description/)（亚马逊、Facebook、谷歌在半年内面试中考过）
	
	[两数之和](https://leetcode-cn.com/problems/two-sum/description/)（近半年内，亚马逊考查此题达到 216 次、字节跳动 147 次、谷歌 104 次，Facebook、苹果、微软、腾讯也在近半年内面试常考）
	
	[N 叉树的前序遍历](https://leetcode-cn.com/problems/n-ary-tree-preorder-traversal/description/)（亚马逊在半年内面试中考过）
	
	[字母异位词分组](https://leetcode-cn.com/problems/group-anagrams/)（亚马逊在半年内面试中常考
	
	[二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/)（亚马逊、字节跳动、微软在半年内面试中考过）
	
	[二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal/)（字节跳动、谷歌、腾讯在半年内面试中考过）
	
	[N 叉树的层序遍历](https://leetcode-cn.com/problems/n-ary-tree-level-order-traversal/)（亚马逊在半年内面试中考过）
	
	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)
	
	[括号生成](https://leetcode-cn.com/problems/generate-parentheses/)
	
	[Pow(x, n)](https://leetcode-cn.com/problems/powx-n/)
	
	[子集](https://leetcode-cn.com/problems/subsets/)
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/)
	
## 泛型递归、树的递归

1. 递归的实现、特性以及思维要点

	[递归代码模板](https://shimo.im/docs/EICAr9lRPUIPHxsH/)

2. 实战题目

	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[括号生成](https://leetcode-cn.com/problems/generate-parentheses/) (字节跳动在半年内面试中考过)
	
	[翻转二叉树](https://leetcode-cn.com/problems/invert-binary-tree/description/) (谷歌、字节跳动、Facebook 在半年内面试中考过)
	
	[验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree)（亚马逊、微软、Facebook 在半年内面试中考过）
	
	[二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree)（亚马逊、微软、字节跳动在半年内面试中考过）
	
	[二叉树的最小深度](https://leetcode-cn.com/problems/minimum-depth-of-binary-tree)（Facebook、字节跳动、谷歌在半年内面试中考过）
	
	[二叉树的序列化与反序列化](https://leetcode-cn.com/problems/serialize-and-deserialize-binary-tree/)（Facebook、亚马逊在半年内面试常考）
	
	[二叉树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/)（Facebook 在半年内面试常考）
	
	[从前序与中序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal)（字节跳动、亚马逊、微软在半年内面试中考过）
	
	[组合](https://leetcode-cn.com/problems/combinations/)（微软、亚马逊、谷歌在半年内面试中考过）
	
	[全排列](https://leetcode-cn.com/problems/permutations/)（字节跳动在半年内面试常考）
	
	[全排列 II ](https://leetcode-cn.com/problems/permutations-ii/)（亚马逊、字节跳动、Facebook 在半年内面试中考过）
	
## 分治、回溯

1. 分治、回溯的实现和特性

	[分治代码模板](https://shimo.im/docs/zvlDqLLMFvcAF79A/)
	
	[括号生成问题](https://leetcode-cn.com/problems/generate-parentheses/)
	
2.  牛顿迭代法

	[牛顿迭代法原理](http://www.matrix67.com/blog/archives/361)
	
	[牛顿迭代法代码](http://www.voidcn.com/article/p-eudisdmk-zm.html)
	
3. 实战题目

	[Pow(x, n)](https://leetcode-cn.com/problems/powx-n/) （Facebook 在半年内面试常考）
	
	[子集](https://leetcode-cn.com/problems/subsets/)（Facebook、字节跳动、亚马逊在半年内面试中考过）
	
	[多数元素](https://leetcode-cn.com/problems/majority-element/description/) （亚马逊、字节跳动、Facebook 在半年内面试中考过）
	
	[电话号码的字母组合](https://leetcode-cn.com/problems/letter-combinations-of-a-phone-number/)（亚马逊在半年内面试常考）
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/)（字节跳动、苹果、谷歌在半年内面试中考过）
	
	[二叉树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/)（Facebook 在半年内面试常考）
	
	[从前序与中序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/)（字节跳动、亚马逊、微软在半年内面试中考过）
	
	[组合](https://leetcode-cn.com/problems/combinations/)（微软、亚马逊、谷歌在半年内面试中考过）
	
	[全排列](https://leetcode-cn.com/problems/permutations/)（字节跳动在半年内面试常考）
	
	[全排列 II](https://leetcode-cn.com/problems/permutations-ii/) （亚马逊、字节跳动、Facebook 在半年内面试中考过）
	
	[二叉树的层次遍历](http://leetcode-cn.com/problems/binary-tree-level-order-traversal/#/description)
	
	[分发饼干](http://leetcode-cn.com/problems/assign-cookies/description/)
	
	[买卖股票的最佳时机 II](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/description/)
	
	[跳跃游戏](http://leetcode-cn.com/problems/jump-game/)
	
	[x 的平方根](http://leetcode-cn.com/problems/sqrtx/)
	
	[有效的完全平方数](http://leetcode-cn.com/problems/valid-perfect-square/)
	
## 深度优先搜索和广度优先搜索

1. 深度优先搜索、广度优先搜索的实现和特性

	[DFS 代码模板（递归写法、非递归写法）](https://shimo.im/docs/UdY2UUKtliYXmk8t/)
	
	[BFS 代码模板](https://shimo.im/docs/ZBghMEZWix0Lc2jQ/)
	
2. 实战题目

	[二叉树的层序遍历](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/#/description)（字节跳动、亚马逊、微软在半年内面试中考过）
	
	[最小基因变化](https://leetcode-cn.com/problems/minimum-genetic-mutation/#/description)
	
	[括号生成](https://leetcode-cn.com/problems/generate-parentheses/#/description)（字节跳动、亚马逊、Facebook 在半年内面试中考过）
	
	[在每个树行中找最大值](https://leetcode-cn.com/problems/find-largest-value-in-each-tree-row/#/description)（微软、亚马逊、Facebook 在半年内面试中考过）
	
	[单词接龙](https://leetcode-cn.com/problems/word-ladder/description/)（亚马逊在半年内面试常考）
	
	[单词接龙 II](https://leetcode-cn.com/problems/word-ladder-ii/description/) （微软、亚马逊、Facebook 在半年内面试中考过）
	
	[岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)（近半年内，亚马逊在面试中考查此题达到 350 次）
	
	[扫雷游戏](https://leetcode-cn.com/problems/minesweeper/description/)（亚马逊、Facebook 在半年内面试中考过）
	
## 贪心算法

1. 贪心的实现、特性及实战题目

	[coin change 题目](https://leetcode-cn.com/problems/coin-change/)
	
	[动态规划定义](https://zh.wikipedia.org/wiki/%E5%8A%A8%E6%80%81%E8%A7%84%E5%88%92)
	
	[柠檬水找零](https://leetcode-cn.com/problems/lemonade-change/description/)（亚马逊在半年内面试中考过）
	
	[买卖股票的最佳时机 II ](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/description/)（亚马逊、字节跳动、微软在半年内面试中考过）
	
	[分发饼干](https://leetcode-cn.com/problems/assign-cookies/description/)（亚马逊在半年内面试中考过）
	
	[模拟行走机器人](https://leetcode-cn.com/problems/walking-robot-simulation/description/)
	
	[跳跃游戏](https://leetcode-cn.com/problems/jump-game/) （亚马逊、华为、Facebook 在半年内面试中考过）
	
	[跳跃游戏 II](https://leetcode-cn.com/problems/jump-game-ii/) （亚马逊、华为、字节跳动在半年内面试中考过）
	
## 二分查找

1. 二分查找的实现和特性

	[二分查找代码模板](https://shimo.im/docs/xvIIfeEzWYEUdBPD/)
	
	[Fast InvSqrt() 扩展阅读](https://www.beyond3d.com/content/articles/8/)
	
2. 实战题目

	[x 的平方根](https://leetcode-cn.com/problems/sqrtx/)（字节跳动、微软、亚马逊在半年内面试中考过）
	
	[有效的完全平方数](https://leetcode-cn.com/problems/valid-perfect-square/)（亚马逊在半年内面试中考过）
	
	[搜索旋转排序数组](https://leetcode-cn.com/problems/search-in-rotated-sorted-array/)（Facebook、字节跳动、亚马逊在半年内面试常考）
	
	[搜索二维矩阵](https://leetcode-cn.com/problems/search-a-2d-matrix/)（亚马逊、微软、Facebook 在半年内面试中考过）
	
	[寻找旋转排序数组中的最小值](https://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array/)（亚马逊、微软、字节跳动在半年内面试中考过）
	
	[柠檬水找零](https://leetcode-cn.com/problems/lemonade-change/description/)（亚马逊在半年内面试中考过）
	
	[买卖股票的最佳时机 II ](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/description/)（亚马逊、字节跳动、微软在半年内面试中考过）
	
	[分发饼干](https://leetcode-cn.com/problems/assign-cookies/description/)（亚马逊在半年内面试中考过）
	
	[模拟行走机器人](https://leetcode-cn.com/problems/walking-robot-simulation/description/)
	
	[单词接龙](https://leetcode-cn.com/problems/word-ladder/description/)（亚马逊在半年内面试常考）
	
	[岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)（近半年内，亚马逊在面试中考查此题达到 350 次）
	
	[扫雷游戏](https://leetcode-cn.com/problems/minesweeper/description/)（亚马逊、Facebook 在半年内面试中考过）
	
	[跳跃游戏](https://leetcode-cn.com/problems/jump-game/) （亚马逊、华为、Facebook 在半年内面试中考过）
	
	[单词接龙 II ](https://leetcode-cn.com/problems/word-ladder-ii/description/)（微软、亚马逊、Facebook 在半年内面试中考过）
	
	[跳跃游戏 II ](https://leetcode-cn.com/problems/jump-game-ii/)（亚马逊、华为、字节跳动在半年内面试中考过）
	
	[最长公共子序列题目](https://leetcode-cn.com/problems/longest-common-subsequence/)
	
	[三角形最小路径和](https://leetcode-cn.com/problems/triangle/description/)
	
	[最大子序和](https://leetcode-cn.com/problems/maximum-subarray/)
	
	[打家劫舍](https://leetcode-cn.com/problems/house-robber/)
	
## 动态规划

1. 动态规划的实现及关键点

	[递归代码模板](https://shimo.im/docs/EICAr9lRPUIPHxsH)
	
	[分治代码模板](https://shimo.im/docs/zvlDqLLMFvcAF79A)
	
	[动态规划定义](https://en.wikipedia.org/wiki/Dynamic_programming)
	
	[MIT 动态规划课程最短路径算法](https://www.bilibili.com/video/av53233912?from=search&seid=2847395688604491997)
	
2. 实战题目

	[不同路径](https://leetcode-cn.com/problems/unique-paths/)（Facebook、亚马逊、微软在半年内面试中考过）
	
	[不同路径 II ](https://leetcode-cn.com/problems/unique-paths-ii/)（谷歌、美团、微软在半年内面试中考过）
	
	[最长公共子序列](https://leetcode-cn.com/problems/longest-common-subsequence/)（字节跳动、谷歌、亚马逊在半年内面试中考过）
	
	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/description/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[三角形最小路径和](https://leetcode-cn.com/problems/triangle/description/)（亚马逊、苹果、字节跳动在半年内面试考过）
	
	三角形最小路径和高票回答： [https://leetcode.com/problems/triangle/discuss/38735/Python-easy-to-understand-solutions-(top-down-bottom-up)](https://leetcode.com/problems/triangle/discuss/38735/Python-easy-to-understand-solutions-(top-down-bottom-up))
	
	[最大子序和](https://leetcode-cn.com/problems/maximum-subarray/)（亚马逊、字节跳动在半年内面试常考）
	
	[乘积最大子数组](https://leetcode-cn.com/problems/maximum-product-subarray/description/)（亚马逊、字节跳动、谷歌在半年内面试中考过）
	
	[零钱兑换](https://leetcode-cn.com/problems/coin-change/description/)（亚马逊在半年内面试中常考）
	
	[打家劫舍](https://leetcode-cn.com/problems/house-robber/)（字节跳动、谷歌、亚马逊在半年内面试中考过）
	
	[打家劫舍 II](https://leetcode-cn.com/problems/house-robber-ii/description/) （字节跳动在半年内面试中考过）
	
	[买卖股票的最佳时机](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock/#/description)（亚马逊、字节跳动、Facebook 在半年内面试中常考）
	
	[买卖股票的最佳时机 II](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/) （亚马逊、字节跳动、微软在半年内面试中考过）
	
	[买卖股票的最佳时机 III ](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iii/)（字节跳动在半年内面试中考过）
	
	[最佳买卖股票时机含冷冻期](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/)（谷歌、亚马逊在半年内面试中考过）
	
	[买卖股票的最佳时机 IV](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iv/) （谷歌、亚马逊、字节跳动在半年内面试中考过）
	
	[买卖股票的最佳时机含手续费](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee/)
	
	[股票问题系列通解](https://leetcode-cn.com/circle/article/qiAgHn/)
	
	[完全平方数](https://leetcode-cn.com/problems/perfect-squares/)（亚马逊、谷歌在半年内面试中考过）
	
	[编辑距离](https://leetcode-cn.com/problems/edit-distance/) （重点）
	
	[跳跃游戏](https://leetcode-cn.com/problems/jump-game/)（亚马逊在半年内面试中考过）
	
	[跳跃游戏 II](https://leetcode-cn.com/problems/jump-game-ii/) （亚马逊、华为字节跳动在半年内面试中考过）
	
	[不同路径](https://leetcode-cn.com/problems/unique-paths/)（Facebook、亚马逊、微软在半年内面试中考过）
	
	[不同路径 II](https://leetcode-cn.com/problems/unique-paths-ii/) （谷歌、美团、微软在半年内面试中考过）
	
	[不同路径 III ](https://leetcode-cn.com/problems/unique-paths-iii/)（谷歌在半年内面试中考过）
	
	[零钱兑换 II](https://leetcode-cn.com/problems/coin-change-2/) （亚马逊、字节跳动在半年内面试中考过）
	
	[最小路径和](https://leetcode-cn.com/problems/minimum-path-sum/)（亚马逊、高盛集团、谷歌在半年内面试中考过）
	
	[解码方法](https://leetcode-cn.com/problems/decode-ways)（亚马逊、Facebook、字节跳动在半年内面试中考过）
	
	[最大正方形](https://leetcode-cn.com/problems/maximal-square/)（华为、谷歌、字节跳动在半年内面试中考过）
	
	[任务调度器](https://leetcode-cn.com/problems/task-scheduler/)（Facebook 在半年内面试中常考）
	
	[回文子串](https://leetcode-cn.com/problems/palindromic-substrings/)（Facebook、苹果、字节跳动在半年内面试中考过）
	
	[最长有效括号](https://leetcode-cn.com/problems/longest-valid-parentheses/)（字节跳动、亚马逊、微软在半年内面试中考过）
	
	[矩形区域不超过 K 的最大数值和](https://leetcode-cn.com/problems/max-sum-of-rectangle-no-larger-than-k/)（谷歌在半年内面试中考过）
	
	[青蛙过河](https://leetcode-cn.com/problems/frog-jump/)（亚马逊、苹果、字节跳动在半年内面试中考过）
	
	[分割数组的最大值](https://leetcode-cn.com/problems/split-array-largest-sum)（谷歌、亚马逊、Facebook 在半年内面试中考过）
	
	[学生出勤记录 II](https://leetcode-cn.com/problems/student-attendance-record-ii/) （谷歌在半年内面试中考过）
	
	[最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring/)（Facebook 在半年内面试中常考）
	
	[戳气球](https://leetcode-cn.com/problems/burst-balloons/)（亚马逊在半年内面试中考过）
	
	[实现 Trie (前缀树)](https://leetcode-cn.com/problems/implement-trie-prefix-tree/#/description)
	
	[单词搜索 II](https://leetcode-cn.com/problems/word-search-ii/)
	
	[岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)
	
	[有效的数独](https://leetcode-cn.com/problems/valid-sudoku/description/)
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/)
	
	[单词接龙](https://leetcode-cn.com/problems/word-ladder/)
	
	[二进制矩阵中的最短路径](https://leetcode-cn.com/problems/shortest-path-in-binary-matrix/)
	
## 字典树和并查集

1. Trie 树的基本实现和特性

	[二叉树的层次遍历](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/)
	
	[实现 Trie](https://leetcode-cn.com/problems/implement-trie-prefix-tree/solution/)
	
	[Trie 树代码模板](https://shimo.im/docs/DP53Y6rOwN8MTCQH)
	
2. 并查集的基本实现和特性

	[并查集代码模板](https://shimo.im/docs/VtcxL0kyp04OBHak)
	
3. 实战题目

	[实现 Trie (前缀树)](https://leetcode-cn.com/problems/implement-trie-prefix-tree/#/description) （亚马逊、微软、谷歌在半年内面试中考过）
	
	[单词搜索 II](https://leetcode-cn.com/problems/word-search-ii/) （亚马逊、微软、苹果在半年内面试中考过）
	
	[省份数量](https://leetcode-cn.com/problems/number-of-provinces/)（亚马逊、Facebook、字节跳动在半年内面试中考过）
	
	[岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)（近半年内，亚马逊在面试中考查此题达到 361 次）
	
	[被围绕的区域](https://leetcode-cn.com/problems/surrounded-regions/)（亚马逊、eBay、谷歌在半年内面试中考过）
	
## 高级搜索

1. 剪枝的实现和特性

	[DFS 代码模板](https://shimo.im/docs/UdY2UUKtliYXmk8t)
	
	[BFS 代码模板](https://shimo.im/docs/ZBghMEZWix0Lc2jQ)
	
	[AlphaZero Explained](https://nikcheerla.github.io/deeplearningschool/2018/01/01/AlphaZero-Explained/)
	
	[棋类复杂度](https://en.wikipedia.org/wiki/Game_complexity)
	
2. 双向 BFS 的实现、特性

	[单词接龙](https://leetcode-cn.com/problems/word-ladder/)（亚马逊、Facebook、谷歌在半年内面试中考过）
	
	[最小基因变化](https://leetcode-cn.com/problems/minimum-genetic-mutation/)（谷歌、Twitter、腾讯在半年内面试中考过）
	
3. 启发式搜索的实现、特性

	[A* 代码模板](https://shimo.im/docs/8CzMlrcvbWwFXA8r)
	
	[相似度测量方法](https://dataaspirant.com/2015/04/11/five-most-popular-similarity-measures-implementation-in-python/)
	
	[二进制矩阵中的最短路径的 A* 解法](https://leetcode.com/problems/shortest-path-in-binary-matrix/discuss/313347/A*-search-in-Python)
	
	[8 puzzles 解法比较](https://zxi.mytechroad.com/blog/searching/8-puzzles-bidirectional-astar-vs-bidirectional-bfs/)
	
4. 实战题目

	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[括号生成](https://leetcode-cn.com/problems/generate-parentheses/)（亚马逊、Facebook、字节跳动在半年内面试中考过）
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/)（亚马逊、苹果、字节跳动在半年内面试中考过）
	
	[有效的数独](https://leetcode-cn.com/problems/valid-sudoku/description/)（亚马逊、苹果、微软在半年内面试中考过）
	
	[解数独](https://leetcode-cn.com/problems/sudoku-solver/#/description)（亚马逊、华为、微软在半年内面试中考过）
	
	[二进制矩阵中的最短路径](https://leetcode-cn.com/problems/shortest-path-in-binary-matrix/)（亚马逊、字节跳动、Facebook 在半年内面试中考过）
	
	[滑动谜题](https://leetcode-cn.com/problems/sliding-puzzle/)（微软、谷歌、Facebook 在半年内面试中考过）	
	
	[解数独](https://leetcode-cn.com/problems/sudoku-solver/)（微软、华为、亚马逊在半年内面试中考过）
	
## 红黑树和 AVL 树

1. 红黑树、AVL 树的实现和特性

	[维基百科：平衡树](https://en.wikipedia.org/wiki/Self-balancing_binary_search_tree)
	
2. 实战题目

	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[实现 Trie (前缀树)](https://leetcode-cn.com/problems/implement-trie-prefix-tree/#/description) （亚马逊、微软、谷歌在半年内面试中考过）
	
	[省份数量](https://leetcode-cn.com/problems/number-of-provinces/)（亚马逊、Facebook、字节跳动在半年内面试中考过）
	
	[岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)（近半年内，亚马逊在面试中考查此题达到 361 次）
	
	[被围绕的区域](https://leetcode-cn.com/problems/surrounded-regions/)（亚马逊、eBay、谷歌在半年内面试中考过）
	
	[有效的数独](https://leetcode-cn.com/problems/valid-sudoku/description/)（亚马逊、苹果、微软在半年内面试中考过）
	
	[括号生成](https://leetcode-cn.com/problems/generate-parentheses/)（亚马逊、Facebook、字节跳动在半年内面试中考过）
	
	[单词接龙](https://leetcode-cn.com/problems/word-ladder/)（亚马逊、Facebook、谷歌在半年内面试中考过）
	
	[最小基因变化](https://leetcode-cn.com/problems/minimum-genetic-mutation/)（谷歌、Twitter、腾讯在半年内面试中考过）
	
	[单词搜索 II](https://leetcode-cn.com/problems/word-search-ii/) （亚马逊、微软、苹果在半年内面试中考过）
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/)（亚马逊、苹果、字节跳动在半年内面试中考过）
	
	[解数独](https://leetcode-cn.com/problems/sudoku-solver/#/description)（亚马逊、华为、微软在半年内面试中考过）
	
	[LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache/#/)
	
	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/)
	
## 位运算

1. 位运算基础及实战要点

	[如何从十进制转换为二进制](https://zh.wikihow.com/%E4%BB%8E%E5%8D%81%E8%BF%9B%E5%88%B6%E8%BD%AC%E6%8D%A2%E4%B8%BA%E4%BA%8C%E8%BF%9B%E5%88%B6)
	
	[N 皇后位运算代码示例](https://shimo.im/docs/YzWa5ZZrZPYWahK2)
	
2. 实战题目

	[位 1 的个数](https://leetcode-cn.com/problems/number-of-1-bits/)（Facebook、苹果在半年内面试中考过）
	
	[2 的幂](https://leetcode-cn.com/problems/power-of-two/)（谷歌、亚马逊、苹果在半年内面试中考过）
	
	[颠倒二进制位](https://leetcode-cn.com/problems/reverse-bits/)（苹果在半年内面试中考过）
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/description/)（字节跳动、亚马逊、百度在半年内面试中考过）
	
	[N 皇后 II](https://leetcode-cn.com/problems/n-queens-ii/description/) （亚马逊在半年内面试中考过）
	
	[比特位计数](https://leetcode-cn.com/problems/counting-bits/description/)（字节跳动、Facebook、MathWorks 在半年内面试中考过）
	
## 布隆过滤器和 LRU 缓存

1. 布隆过滤器的实现及应用

	[布隆过滤器的原理和实现](https://www.cnblogs.com/cpselvis/p/6265825.html)
	
	[使用布隆过滤器解决缓存击穿、垃圾邮件识别、集合判重](https://blog.csdn.net/tianyaleixiaowu/article/details/74721877)
	
	[布隆过滤器 Python 代码示例](https://shimo.im/docs/UITYMj1eK88JCJTH)
	
	[布隆过滤器 Python 实现示例](https://www.geeksforgeeks.org/bloom-filters-introduction-and-python-implementation/)
	
	[高性能布隆过滤器 Python 实现示例](https://github.com/jhgg/pybloof)
	
	[布隆过滤器 Java 实现示例 1](https://github.com/lovasoa/bloomfilter/blob/master/src/main/java/BloomFilter.java)
	
	[布隆过滤器 Java 实现示例 2](https://github.com/Baqend/Orestes-Bloomfilter)
	
2. LRU Cache 的实现、应用

	[Understanding the Meltdown exploit](https://www.sqlpassion.at/archive/2018/01/06/understanding-the-meltdown-exploit-in-my-own-simple-words/)
	
	[替换算法总览](https://en.wikipedia.org/wiki/Cache_replacement_policies)
	
	[LRU Cache Python 代码示例](https://shimo.im/docs/CoyPAyXooGcDuLQo)
	
	[LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache/#/)（亚马逊、字节跳动、Facebook、微软在半年内面试中常考）
	
## 排序算法

1. 初级排序和高级排序的实现和特性

	[十大经典排序算法](https://www.cnblogs.com/onepixel/p/7674659.html)
	
	[快速排序代码示例](https://shimo.im/docs/TX9bDbSC7C0CR5XO)
	
	[归并排序代码示例](https://shimo.im/docs/sDXxjjiKf3gLVVAU)
	
	[堆排序代码示例](https://shimo.im/docs/M2xfacKvwzAykhz6)
	
	[9 种经典排序算法可视化动画](https://www.bilibili.com/video/av25136272)
	
	[6 分钟看完 15 种排序算法动画展示](https://www.bilibili.com/video/av63851336)
	
2. 实战题目

	[数组的相对排序](https://leetcode-cn.com/problems/relative-sort-array/)（谷歌在半年内面试中考过）
	
	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/)（Facebook、亚马逊、谷歌在半年内面试中考过）
	
	[力扣排行榜](https://leetcode-cn.com/problems/design-a-leaderboard/)（Bloomberg 在半年内面试中考过）
	
	[合并区间](https://leetcode-cn.com/problems/merge-intervals/)（Facebook、字节跳动、亚马逊在半年内面试中常考）
	
	[翻转对](https://leetcode-cn.com/problems/reverse-pairs/)（字节跳动在半年内面试中考过）
	
	[位 1 的个数](https://leetcode-cn.com/problems/number-of-1-bits/)（Facebook、苹果在半年内面试中考过）
	
	[2 的幂](https://leetcode-cn.com/problems/power-of-two/)（谷歌、亚马逊、苹果在半年内面试中考过）
	
	[颠倒二进制位](https://leetcode-cn.com/problems/reverse-bits/)（苹果在半年内面试中考过）
	
	[数组的相对排序](https://leetcode-cn.com/problems/relative-sort-array/)（谷歌在半年内面试中考过）
	
	[LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache/#/)（亚马逊、字节跳动、Facebook、微软在半年内面试中常考）
	
	[N 皇后](https://leetcode-cn.com/problems/n-queens/description/)（字节跳动、亚马逊、百度在半年内面试中考过）
	
	[N 皇后 II](https://leetcode-cn.com/problems/n-queens-ii/description/) （亚马逊在半年内面试中考过）
	
	[不同路径](http://leetcode-cn.com/problems/unique-paths/)
	
	[最小路径和](http://leetcode-cn.com/problems/minimum-path-sum/)
	
## 高级动态规划

1. 实战题目

	[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)（阿里巴巴、腾讯、字节跳动在半年内面试常考）
	
	[使用最小花费爬楼梯](https://leetcode-cn.com/problems/min-cost-climbing-stairs/)（亚马逊在半年内面试中考过）
	
	[不同路径](https://leetcode-cn.com/problems/unique-paths/)（亚马逊、微软、Facebook 在半年内面试中考过）
	
	[打家劫舍](https://leetcode-cn.com/problems/house-robber/)（字节跳动、谷歌、苹果在半年内面试中考过）
	
	[最小路径和](https://leetcode-cn.com/problems/minimum-path-sum/)（字节跳动、谷歌、亚马逊在半年内面试中考过）
	
	[股票买卖](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock/)（字节跳动、亚马逊、Facebook 在半年内面试常考）
	
	[编辑距离](https://leetcode-cn.com/problems/edit-distance/)（字节跳动、亚马逊、谷歌在半年内面试中考过）
	
	[最长上升子序列](https://leetcode-cn.com/problems/longest-increasing-subsequence/)（字节跳动、亚马逊、微软在半年内面试中考过）
	
	[解码方法](https://leetcode-cn.com/problems/decode-ways/)（Facebook、亚马逊、字节跳动在半年内面试中考过）
	
	[最长有效括号](https://leetcode-cn.com/problems/longest-valid-parentheses/)（华为、亚马逊、字节跳动在半年内面试中考过）
	
	[最大矩形](https://leetcode-cn.com/problems/maximal-rectangle/)（谷歌、微软、字节跳动在半年内面试中考过）
	
	[不同的子序列](https://leetcode-cn.com/problems/distinct-subsequences/)（MathWorks 在半年内面试中考过）
	
	[赛车](https://leetcode-cn.com/problems/race-car/)（谷歌在半年内面试中考过）
	
## 字符串算法

1. 字符串基础知识

	[不可变字符串](https://lemire.me/blog/2017/07/07/are-your-strings-immutable/)
	
	[Atoi 代码示例](https://shimo.im/docs/5kykuLmt7a4DdjSP)
	
2.  字符串匹配算法

	[Boyer-Moore 算法](https://www.ruanyifeng.com/blog/2013/05/boyer-moore_string_search_algorithm.html)

	[Sunday 算法](https://blog.csdn.net/u012505432/article/details/52210975)

	[字符串匹配暴力法代码示例](https://shimo.im/docs/8G0aJqNL86wWrPUE)

	[Rabin-Karp 代码示例](https://shimo.im/docs/1wnsM7eaZ6Ab9j9M)

	[KMP 字符串匹配算法视频](https://www.bilibili.com/video/av11866460?from=search&seid=17425875345653862171)

	[字符串匹配的 KMP 算法](http://www.ruanyifeng.com/blog/2013/05/Knuth%E2%80%93Morris%E2%80%93Pratt_algorithm.html)
	
3. 字符串基础问题

	[转换成小写字母](https://leetcode-cn.com/problems/to-lower-case/)（谷歌在半年内面试中考过）
	
	[最后一个单词的长度](https://leetcode-cn.com/problems/length-of-last-word/)（苹果、谷歌、字节跳动在半年内面试中考过）
	
	[宝石与石头](https://leetcode-cn.com/problems/jewels-and-stones/)（亚马逊在半年内面试中考过）
	
	[字符串中的第一个唯一字符](https://leetcode-cn.com/problems/first-unique-character-in-a-string/)（亚马逊、微软、Facebook 在半年内面试中考过）

	[字符串转换整数 (atoi)](https://leetcode-cn.com/problems/string-to-integer-atoi/) （亚马逊、微软、Facebook 在半年内面试中考过）
	
4. 字符串操作问题

	[最长公共前缀](https://leetcode-cn.com/problems/longest-common-prefix/description/)（亚马逊、谷歌、Facebook 在半年内面试中考过）
	
	[反转字符串](https://leetcode-cn.com/problems/reverse-string)（亚马逊、谷歌、苹果在半年内面试中考过）
	
	[反转字符串 II](https://leetcode-cn.com/problems/reverse-string-ii/) （亚马逊在半年内面试中考过）
	
	[翻转字符串里的单词](https://leetcode-cn.com/problems/reverse-words-in-a-string/)（微软、字节跳动、苹果在半年内面试中考过）
	
	[反转字符串中的单词 III](https://leetcode-cn.com/problems/reverse-words-in-a-string-iii/) （微软、字节跳动、华为在半年内面试中考过）
	
	[仅仅反转字母](https://leetcode-cn.com/problems/reverse-only-letters/)（字节跳动在半年内面试中考过）
	
5. 异位词问题

	[有效的字母异位词](https://leetcode-cn.com/problems/valid-anagram/)（Facebook、亚马逊、谷歌在半年内面试中考过）

	[字母异位词分组](https://leetcode-cn.com/problems/group-anagrams/)（亚马逊在半年内面试中常考）

	[找到字符串中所有字母异位词](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/)（Facebook 在半年内面试中常考）
	
6. 回文串问题

	[验证回文串](https://leetcode-cn.com/problems/valid-palindrome/)（Facebook 在半年内面试中常考）

	[验证回文字符串 Ⅱ](https://leetcode-cn.com/problems/valid-palindrome-ii/)（Facebook 在半年内面试中常考）

	[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)（亚马逊、字节跳动、华为在半年内面试中常考）
	
7. 最长子串、子序列问题

	[最长公共子序列](https://leetcode-cn.com/problems/longest-common-subsequence/)（亚马逊、字节跳动、谷歌在半年内面试中考过）

	[编辑距离](https://leetcode-cn.com/problems/edit-distance/)（亚马逊、字节跳动、谷歌在半年内面试中考过）

	[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)（亚马逊、华为、字节跳动在半年内面试常考）
	
8. 字符串 + DP 问题

	[正则表达式匹配](https://leetcode-cn.com/problems/regular-expression-matching/)（Facebook、微软、字节跳动在半年内面试中考过）
	
	题解： [https://leetcode-cn.com/problems/regular-expression-matching/solution/ji-yu-guan-fang-ti-jie-gen-xiang-xi-de-jiang-jie-b/](https://leetcode-cn.com/problems/regular-expression-matching/solution/ji-yu-guan-fang-ti-jie-gen-xiang-xi-de-jiang-jie-b/)
	
	[通配符匹配](https://leetcode-cn.com/problems/wildcard-matching/)（Facebook、微软、字节跳动在半年内面试中考过）
	
	[不同的子序列](https://leetcode-cn.com/problems/distinct-subsequences/)（MathWorks 在半年内面试中考过）
	
9. 实战题目

	[字符串中的第一个唯一字符](https://leetcode-cn.com/problems/first-unique-character-in-a-string/)（亚马逊、微软、Facebook 在半年内面试中考过）

	[反转字符串 II](https://leetcode-cn.com/problems/reverse-string-ii/) （亚马逊在半年内面试中考过）

	[翻转字符串里的单词](https://leetcode-cn.com/problems/reverse-words-in-a-string/)（微软、字节跳动、苹果在半年内面试中考过）

	[反转字符串中的单词 III](https://leetcode-cn.com/problems/reverse-words-in-a-string-iii/) （微软、字节跳动、华为在半年内面试中考过）

	[仅仅反转字母](https://leetcode-cn.com/problems/reverse-only-letters/)（字节跳动在半年内面试中考过）

	[同构字符串](https://leetcode-cn.com/problems/isomorphic-strings/)（谷歌、亚马逊、微软在半年内面试中考过）

	[验证回文字符串 Ⅱ](https://leetcode-cn.com/problems/valid-palindrome-ii/)（Facebook 在半年内面试中常考）

	[最长上升子序列](https://leetcode-cn.com/problems/longest-increasing-subsequence/)（字节跳动、亚马逊、微软在半年内面试中考过）

	[解码方法](https://leetcode-cn.com/problems/decode-ways/)（字节跳动、亚马逊、Facebook 在半年内面试中考过）

	[字符串转换整数 (atoi)](https://leetcode-cn.com/problems/string-to-integer-atoi/) （亚马逊、微软、Facebook 在半年内面试中考过）

	[找到字符串中所有字母异位词](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/)（Facebook 在半年内面试中常考）

	[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/)（亚马逊、字节跳动、华为在半年内面试中常考）

	[最长有效括号](https://leetcode-cn.com/problems/longest-valid-parentheses/)（亚马逊、字节跳动、华为在半年内面试中考过）

	[赛车](https://leetcode-cn.com/problems/race-car/)（谷歌在半年内面试中考过）

	[通配符匹配](https://leetcode-cn.com/problems/wildcard-matching/)（Facebook、微软、字节跳动在半年内面试中考过）

	[不同的子序列](https://leetcode-cn.com/problems/distinct-subsequences/)（MathWorks 在半年内面试中考过）
	
## 推荐题目

1. 基础

	[两数之和](http://leetcode-cn.com/problems/two-sum)（简单）
	
	[有效的括号](http://leetcode-cn.com/problems/valid-parentheses/)（简单）
	
	[字符串解码](http://leetcode-cn.com/problems/decode-string/)（中等）
	
	[LRU 缓存机制](http://leetcode-cn.com/problems/lru-cache/submissions/)（困难）
	
	[实现 Trie（前缀树）](http://leetcode-cn.com/problems/implement-trie-prefix-tree/)（中等）
	
	[添加与搜索单词 - 数据结构设计](http://leetcode-cn.com/problems/add-and-search-word-data-structure-design/)（中等）
	
	[单词搜索 II](http://leetcode-cn.com/problems/word-search-ii/) （困难）
	
	[找不同](http://leetcode-cn.com/problems/find-the-difference/)（简单）
	
	[单词规律](http://leetcode-cn.com/problems/word-pattern/)（简单）
	
	[字符串中的第一个唯一字符](http://leetcode-cn.com/problems/first-unique-character-in-a-string)（简单）
	
	[无重复字符的最长子串](http://leetcode-cn.com/problems/longest-substring-without-repeating-characters)（中等）
	
	[最小覆盖子串](http://leetcode-cn.com/problems/minimum-window-substring/)（困难）
	
	[合并两个有序链表](http://leetcode-cn.com/problems/merge-two-sorted-lists)（简单）
	
	[环形链表](http://leetcode-cn.com/problems/linked-list-cycle)（简单）
	
	[环形链表 II](http://leetcode-cn.com/problems/linked-list-cycle-ii) （中等）
	
	[反转链表](http://leetcode-cn.com/problems/reverse-linked-list)（简单）
	
	[反转链表 II](http://leetcode-cn.com/problems/reverse-linked-list-ii) （中等）
	
	[旋转链表](http://leetcode-cn.com/problems/rotate-list)（中等）
	
	[排序链表](http://leetcode-cn.com/problems/sort-list/)
	
	[链表中倒数第 k 个节点](http://leetcode-cn.com/problems/lian-biao-zhong-dao-shu-di-kge-jie-dian-lcof/)
	
	[两两交换链表中的节点](http://leetcode-cn.com/problems/swap-nodes-in-pairs)（中等）
	
	[按奇偶排序数组](http://leetcode-cn.com/problems/sort-array-by-parity/)（简单）
	
	[按奇偶排序数组 II](http://leetcode-cn.com/problems/sort-array-by-parity-ii/) （简单）
	
	[有序数组的平方](http://leetcode-cn.com/problems/squares-of-a-sorted-array/)（简单）
	
	[山脉数组的峰顶索引](http://leetcode-cn.com/problems/peak-index-in-a-mountain-array)（简单）
	
	[搜索旋转排序数组](http://leetcode-cn.com/problems/search-in-rotated-sorted-array)（困难）
	
	[搜索旋转排序数组 II](http://leetcode-cn.com/problems/search-in-rotated-sorted-array-ii/) （中等）
	
	[寻找旋转排序数组中的最小值](http://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array/)（中等）
	
	[寻找旋转排序数组中的最小值 II](http://leetcode-cn.com/problems/find-minimum-in-rotated-sorted-array-ii/) （困难）
	
	[搜索二维矩阵](http://leetcode-cn.com/problems/search-a-2d-matrix)（中等）
	
	[等式方程的可满足性](http://leetcode-cn.com/problems/satisfiability-of-equality-equations/)（中等）
	
	[朋友圈](http://leetcode-cn.com/problems/friend-circles/)（中等）
	
	[账户合并](http://leetcode-cn.com/problems/accounts-merge/)（中等）
	
2. 深度优先搜索

	[二叉树的最大深度](http://leetcode-cn.com/problems/maximum-depth-of-binary-tree)（简单）
	
	[路径总和](http://leetcode-cn.com/problems/path-sum/)（简单）
	
	[路径总和 II](http://leetcode-cn.com/problems/path-sum-ii/) （中等）
	
	[被围绕的区域](http://leetcode-cn.com/problems/surrounded-regions/)（中等）
	
	[岛屿数量](http://leetcode-cn.com/problems/number-of-islands/)（中等）
	
	[岛屿的最大面积](http://leetcode-cn.com/problems/max-area-of-island/)（中等）
	
	[在二叉树中分配硬币](http://leetcode-cn.com/problems/distribute-coins-in-binary-tree/)（中等）
	
3. 回溯

	[括号生成](http://leetcode-cn.com/problems/generate-parentheses/)（中等）
	
	[N 皇后](http://leetcode-cn.com/problems/n-queens/)（困难）
	
	[N 皇后 II](http://leetcode-cn.com/problems/n-queens-ii/) （困难）
	
	[解数独](http://leetcode-cn.com/problems/sudoku-solver/) （中等）
	
	[不同路径 III](http://leetcode-cn.com/problems/unique-paths-iii/) （困难）
	
	[单词搜索](http://leetcode-cn.com/problems/word-search/)（中等）
	
4. 分治

	[搜索二维矩阵 II](http://leetcode-cn.com/problems/search-a-2d-matrix-ii/) （中等）

	[合并 K 个排序链表](http://leetcode-cn.com/problems/merge-k-sorted-lists)（中等）

	[为运算表达式设计优先级](http://leetcode-cn.com/problems/different-ways-to-add-parentheses)（中等）

	[给表达式添加运算符](http://leetcode-cn.com/problems/expression-add-operators)（困难）

	[数组中的第 K 个最大元素](http://leetcode-cn.com/problems/kth-largest-element-in-an-array)（中等）

	[最接近原点的 K 个点](http://leetcode-cn.com/problems/k-closest-points-to-origin/)（中等）

	[鸡蛋掉落](http://leetcode-cn.com/problems/super-egg-drop/)（困难）
	
5. 动态规划

	[使用最小花费爬楼梯](http://leetcode-cn.com/problems/min-cost-climbing-stairs)（简单）
	
	[爬楼梯](http://leetcode-cn.com/problems/climbing-stairs)（简单）
	
	[不同路径](http://leetcode-cn.com/problems/unique-paths/)（简单）
	
	[最小路径和](http://leetcode-cn.com/problems/minimum-path-sum/) （中等）
	
	[最大子序和](http://leetcode-cn.com/problems/maximum-subarray/) （简单）

	[乘积最大子数组](http://leetcode-cn.com/problems/maximum-product-subarray/)（中等）
	
	[买卖股票的最佳时机](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock)（简单）
	
	[买卖股票的最佳时机 II](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii/) （简单）

	[买卖股票的最佳时机 III](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iii/) （困难）

	[买卖股票的最佳时机 IV](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iv/) （困难）

	[最佳买卖股票时机含冷冻期](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/)（中等）
	
	[买卖股票的最佳时机含手续费](http://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee)（中等）

	[零钱兑换](http://leetcode-cn.com/problems/coin-change) （中等）

	[零钱兑换 II](http://leetcode-cn.com/problems/coin-change-2) （中等）

	[编辑距离](http://leetcode-cn.com/problems/edit-distance)（困难）

	[不同的子序列](http://leetcode-cn.com/problems/distinct-subsequences/)（困难）

	[柱状图中最大的矩形](http://leetcode-cn.com/problems/largest-rectangle-in-histogram/)（困难）

	[最大矩形](http://leetcode-cn.com/problems/maximal-rectangle/)（困难）

	[最大正方形](http://leetcode-cn.com/problems/maximal-square/)（中等）

	[最低票价](http://leetcode-cn.com/problems/minimum-cost-for-tickets/)（中等）

	[区域和检索 - 数组不可变](http://leetcode-cn.com/problems/range-sum-query-immutable/)（简单）

	[二维区域和检索 - 矩阵不可变](http://leetcode-cn.com/problems/range-sum-query-2d-immutable/)（中等）

	[最长上升子序列](http://leetcode-cn.com/problems/longest-increasing-subsequence) （中等）

	[鸡蛋掉落](http://leetcode-cn.com/problems/super-egg-drop/)（困难）
	
##  附

1. Big O Cheat Sheet

	[Big O Cheat Sheet](https://www.bigocheatsheet.com/)
	
2. Steve Jobs 演讲

	[Steve Jobs 演讲](https://www.youtube.com/watch?v=Hd_ptbiPoXM)
	