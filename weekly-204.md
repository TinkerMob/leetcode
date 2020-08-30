3 - [Detect Pattern of Length m Repeated k or More Times](https://leetcode.com/contest/weekly-contest-204/problems/detect-pattern-of-length-m-repeated-k-or-more-times/)

实现。

时间复杂度$O(n^2)$，空间复杂度$O(1)$。

4 - [Maximum Length of Subarray with Positive Product](https://leetcode.com/contest/weekly-contest-204/problems/maximum-length-of-subarray-with-positive-product/)

用0把数组分为子区间，如果一个区间内有奇数个负数，那么这个区间里最大个数一定以第一个负数作为开头到结尾，或开头到最后一个负数作为结尾。

时间复杂度$O(n)$，空间复杂度$O(1)$。

6 - [Minimum Number of Days to Disconnected Island](https://leetcode.com/contest/weekly-contest-204/problems/minimum-number-of-days-to-disconnect-island/)

题目样例具有误导性，最差情况也可以通过两次操作将一个角落的点分割开，剩下的主要检测是否存在一个割点。

时间复杂度$O(n^2m^2)$，空间复杂度$O(nm)$。

7 - [Number of Ways to Reorder Array to Get Same BST](https://leetcode.com/contest/weekly-contest-204/problems/number-of-ways-to-reorder-array-to-get-same-bst/)

二叉树树左右两边的元素可以以任意顺序交叉，预处理出交错的组合数`dp[i][j] = dp[i - 1][j] + dp[i][j - 1]`，对于每个节点，个数为两个子树的排列数的乘积再乘以交错组合数。

总时间复杂度$O(n^2)$，单次查询$O(n\log n)$，空间复杂度$O(n^2)$。
