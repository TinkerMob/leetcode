## 3 - [Sum of All Odd Length Subarrays](https://leetcode.com/contest/biweekly-contest-35/problems/sum-of-all-odd-length-subarrays/)

实现。

时间复杂度$O(n^2)$，空间复杂度$O(n)$。

## 5 - [Maximum Sum Obtained of Any Permutation](https://leetcode.com/contest/biweekly-contest-35/problems/maximum-sum-obtained-of-any-permutation/)

贪心。统计每个位置被区间覆盖多少次，对于每个区间用进入+1，离开-1排序后进行统计。对覆盖次数和原数组排序，结果为这两个数组对应位置相乘。

时间复杂度$O(n\log n)$，空间复杂度$O(n)$。

## 5 - [Make Sum Divisible by P](https://leetcode.com/contest/biweekly-contest-35/problems/make-sum-divisible-by-p/)

先统计从后向前累加和的余数，再从前向后每一步记录前缀和余数最后一次出现的位置，结果为每个后缀与满足条件的前缀和的差的最小值。

时间复杂度$O(n)$，空间复杂度$O(n)$。

## 6 - [Strange Printer II](https://leetcode.com/contest/biweekly-contest-35/problems/strange-printer-ii/)

每个数字所在的矩形区间内如果有其它的数字，那么其它的数字必须先于当前数字。能成功进行拓扑排序就能打印。

时间复杂度$O(n^3)$，空间复杂度$O(n^2)$。
