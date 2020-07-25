## 3 - [Count Odd Numbers in an Interval Range](https://leetcode.com/contest/biweekly-contest-31/problems/count-odd-numbers-in-an-interval-range)

从0～n，奇数的个数是(n + 1) / 2，用0～r和0～(l - 1)的奇数个数相减。

## 4 - [Number of Sub-arrays With Odd Sum](https://leetcode.com/contest/biweekly-contest-31/problems/number-of-sub-arrays-with-odd-sum)

从前向后统计奇偶前缀和的个数，如果当前前缀和为奇数，则总数量加上之前前缀和为偶数的个数。

时间复杂度$O(n)$，空间复杂度$O(1)$.

## 5 - [Number of Good Ways to Split a String](Number of Good Ways to Split a String)

前后分别统计不同字符个数。

时间复杂度$O(n)$，空间复杂度$O(n)$.

## 7 - [Minimum Number of Increments on Subarrays to Form a Target Array](Minimum Number of Increments on Subarrays to Form a Target Array)

从前向后：
* 如果当前值比上一个值大，则说明需要在上一个值的基础上执行差值的步数才能达到当前的结果；
* 如果比前一个值小，则可以靠扩展之前操作的范围达成，不需要额外步骤。

时间复杂度$O(n)$，空间复杂度$O(1)$.
