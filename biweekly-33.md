3 - [Thousand Separator](https://leetcode.com/contest/biweekly-contest-33/problems/thousand-separator/)

实现。

时间复杂度$O(\log n)$，空间复杂度$O(\log n)$。

4 - [Minimum Number of Vertices to Reach All Nodes](https://leetcode.com/contest/biweekly-contest-33/problems/minimum-number-of-vertices-to-reach-all-nodes/)

找入度为0的点。

时间复杂度$O(n)$，空间复杂度$O(n)$。

5 - [Minimum Numbers of Funtion Calls to Make Target Array](https://leetcode.com/contest/biweekly-contest-33/problems/minimum-numbers-of-function-calls-to-make-target-array/)

反向贪心，每一轮数组中的数字如果是奇数就减1，然后整体除2。注意最后一轮可能不用除2。

时间复杂度$O(n \log n)$，空间复杂度$O(1)$。

6 - [Detect Cycles in 2D Grid](https://leetcode.com/contest/biweekly-contest-33/problems/detect-cycles-in-2d-grid/)

本质上DFS、BFS均可，如果一个点之前被别的点访问过就存在环。

时间复杂度$O(nm)$，空间复杂度$O(nm)$。
