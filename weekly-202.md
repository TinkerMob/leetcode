# 3 - [Three Consecutive Odds](https://leetcode.com/contest/weekly-contest-202/problems/three-consecutive-odds/)

实现。

时间复杂度$O(n)$，空间复杂度$O(1)$。

# 4 - [Minimum Operations to Make Array Equal](https://leetcode.com/contest/weekly-contest-202/problems/minimum-operations-to-make-array-equal/)

中位数是$n$，用等差数列求和公式算前一半与$n$的差值。

时间复杂度$O(1)$，空间复杂度$O(1)$。

# 5 - [Magnetic Force Between Two Balls](https://leetcode.com/contest/weekly-contest-202/problems/magnetic-force-between-two-balls/)

对原数组排序，二分搜索最小距离，对于每一个候选距离贪心地放球，每次与上一球距离大于等于候选距离即可放球，如果可以放的球的数目大于等于$m$则当前距离满足条件。

时间复杂度$O(n\log n)$，空间复杂度$O(1)$。

# 6 - [Minimum Number of Days to Eat n Oranges](https://leetcode.com/contest/weekly-contest-202/problems/minimum-number-of-days-to-eat-n-oranges/)

优先搜索$n / 2$和$n / 3$的情况，如果其中一个条件不满足就去搜索$n - 1$。

时间复杂度$O(\log n)$，空间复杂度$O(\log n)$。
