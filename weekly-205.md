# 3 - [Replace All ?'s to Avoid Consecutive Repeating Characters](https://leetcode.com/contest/weekly-contest-205/problems/replace-all-s-to-avoid-consecutive-repeating-characters/)

枚举。

时间复杂度$O(n)$，空间复杂度$O(1)$。

# 5 - [Number of Ways Where Square of Number Is Equal to Product of Two Numbers](https://leetcode.com/contest/weekly-contest-205/problems/number-of-ways-where-square-of-number-is-equal-to-product-of-two-numbers/)

用hash记录平方的个数。

时间复杂度$O(n^2)$，空间复杂度$O(n)$。

# 5 - [Minimum Deletion Cost to Avoid Repeating Letters](https://leetcode.com/contest/weekly-contest-205/problems/minimum-deletion-cost-to-avoid-repeating-letters/)

贪心。

时间复杂度$O(n)$，空间复杂度$O(1)$。

# 6 - [Remove Max Number of Edges to Keep Graph Fully Traversable](https://leetcode.com/contest/weekly-contest-205/problems/remove-max-number-of-edges-to-keep-graph-fully-traversable/)

第三种类型的边比其它两种更重要，当两个点间同时包含不同类型的边时，保留第三类边不会导致更差的结果。首先对第三种边计算最小生成树，在这个结果上再分别计算第一类和第二类的最小生成树。

时间复杂度$O(n)$，空间复杂度$O(n)$。
