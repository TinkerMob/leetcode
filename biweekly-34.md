# 3 - [Matrix Diagnoal Sum](https://leetcode.com/contest/biweekly-contest-34/problems/matrix-diagonal-sum/)

实现。

时间复杂度$O(n)$，空间复杂度$O(1)$。

# 4 - [Nuber of Ways to Split a String](https://leetcode.com/contest/biweekly-contest-34/problems/number-of-ways-to-split-a-string/)

如果没有1，数量为C(n - 1, 2)；如果1的个数能被3整除，数量为两组1的间隔的乘积。

时间复杂度$O(n)$，空间复杂度$O(1)$。

# 5 - [Shortest Subarray to Be Removed to Make Array Sorted](https://leetcode.com/contest/biweekly-contest-34/problems/shortest-subarray-to-be-removed-to-make-array-sorted/)

记录从前往后递增序列末位值到下标的映射，在从后往前找时找到第一个小于等于当前值的下标。

时间复杂度$O(n)$，空间复杂度$O(n)$。

# 6 - [Count All Possible Routes](https://leetcode.com/contest/biweekly-contest-34/problems/count-all-possible-routes/)

优先队列，记录油量和位置，使用油量作为优先队列的键值作为大顶堆。

时间复杂度$O(n^2 f)$，空间复杂度$O(nf)$。
