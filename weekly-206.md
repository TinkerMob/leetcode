# 3 - [Special Positions in a Binary Matrix](https://leetcode.com/contest/weekly-contest-206/problems/special-positions-in-a-binary-matrix/)

分别统计行和列的和。

时间复杂度$O(n^2)$，空间复杂度$O(n)$。

# 4 - [Count Unhappy Friends](https://leetcode.com/contest/weekly-contest-206/problems/count-unhappy-friends/)

记录反向下标。

时间复杂度$O(n^2)$，空间复杂度$O(n^2)$。

# 5 - [Min Cost to Connect All Points](https://leetcode.com/contest/weekly-contest-206/problems/min-cost-to-connect-all-points/)

数据范围比较小，可全连接建边最小生成树。

时间复杂度$O(n^2 \log n)$，空间复杂度$O(n^2)$。

# 6 - [Check If String Is Transformable With Substring Sort Operations](https://leetcode.com/contest/weekly-contest-206/problems/check-if-string-is-transformable-with-substring-sort-operations/)

本质上排序的过程可以转换成每次只对相邻的两个位置排序，对于目标的每个位置，只需看最近的那个数字前有没有比它更小的数字即可。用数组分别记录源串里不同数字的下标。

时间复杂度$O(n)$，空间复杂度$O(n)$。
