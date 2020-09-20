## 3 - [Rearrange Spaces Between Words](https://leetcode.com/contest/weekly-contest-207/problems/rearrange-spaces-between-words/)

实现。

时间复杂度$O(n)$，空间复杂度$O(n)$。

## 4 - [Split a String Into the Max Number of Unique Substrings](https://leetcode.com/contest/weekly-contest-207/problems/split-a-string-into-the-max-number-of-unique-substrings/)

深搜。

时间复杂度$O(2^n n)$，空间复杂度$O(n)$。

## 5 - [Maximum Non Negative Product in a Matrix](https://leetcode.com/contest/weekly-contest-207/problems/maximum-non-negative-product-in-a-matrix/)

动态规划。记录每个位置能取得的最小非正数和最大非负数。

时间复杂度$O(n^2)$，空间复杂度$O(n)$。

## 6 - [Minimum Cost to Connect Two Groups of Points](https://leetcode.com/contest/weekly-contest-207/problems/minimum-cost-to-connect-two-groups-of-points/)

动态规划。`dp[i][j]`中`j`为状态压缩后已经被连接的属于第一组里的点，记录第二组里前`i`个点且第一组连接状态为`j`的最小cost。对于第`i`个第二组点有两种选择：
* 选择一个最小cost连接，不管第一组中对应的点是否已经连接；
* 尽可能去连接未被连接的第一组中的点，假设未被连接的点的状态压缩为`target`，令`mask`的初始值为`target`，每一轮更新`mask = (mask - 1) & target`可以枚举所有未被连接状态的子集。

时间复杂度$O(2^{2n}m)$，空间复杂度$O(2^n m)$。
