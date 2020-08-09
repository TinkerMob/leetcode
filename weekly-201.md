## 3 - [Make the String Great](https://leetcode.com/contest/weekly-contest-201/problems/make-the-string-great/)

栈，贪心。

时间复杂度$O(n)$，空间复杂度$O(n)$。

## 4 - [Find kth bit in nth Binary String](https://leetcode.com/contest/weekly-contest-201/problems/find-kth-bit-in-nth-binary-string/)

从上往下递推。

时间复杂度$O(n)$，空间复杂度$O(1)$。

## 6 - [Maximum Number of Non-overlaping Subarrays with Sum Equals Target](https://leetcode.com/contest/weekly-contest-201/problems/maximum-number-of-non-overlapping-subarrays-with-sum-equals-target/)

用$dp\_i$记录到位置$i$为止最大满足条件的非空子数组的个数$dp\_i = \max(dp\_i, dp\_{i - 1})$，同时记录历史前缀和最后一次出现的位置，每个位置只需找之前前缀和为$sum\_i - target$的最后一次的位置$j$，$dp\_i = dp\_j + 1$。

时间复杂度$O(n)$，空间复杂度$O(n)$。

## 7 - [Minimum Cost to Cut a Stick](https://leetcode.com/contest/weekly-contest-201/problems/minimum-cost-to-cut-a-stick/)

自下而上合并，对$cut$排序，$dp\_{i,j}$表示从$i$到$j$需要的最小$cost$。$dp\_{i,j} = \min\_{k \in (i, j)} dp\_{i,k} + dp\_{k,j} + cut\_j - cut\_i$。

时间复杂度$O(n^3)$，空间复杂度$O(n^2)$。
