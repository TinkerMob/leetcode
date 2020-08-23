3 - [Most Visited Sector in a Circular Track](https://leetcode.com/contest/weekly-contest-203/problems/most-visited-sector-in-a-circular-track/)

直接模拟。

时间复杂度$O(nm)$，空间复杂度$O(n)$。

4 - [Maximum Number of Coins You Can Get](https://leetcode.com/contest/weekly-contest-203/problems/maximum-number-of-coins-you-can-get/)

贪心，每次拿剩下里面第二大的，让Bob拿最小的。

时间复杂度$O(n\log n)$，空间复杂度$O(1)$。

6 - [Find Latest Group of Size m](https://leetcode.com/contest/weekly-contest-203/problems/find-latest-group-of-size-m/)

用并查集维护相邻1的合并和个数的记录，用另外一个数组记录一个每种连续1对应的个数。每次新增一个1时，先把左右两边连续1的个数减去，然后增加合并后连续1的长度。

时间复杂度$O(n)$，空间复杂度$O(n)$。

7 - [Stone Game V](https://leetcode.com/contest/weekly-contest-203/problems/stone-game-v/)

区间DP，注意到每个区间存在凹性，用三分法来找极大点。

时间复杂度$O(n^2 \log n)$，空间复杂度$O(n^2)$。
