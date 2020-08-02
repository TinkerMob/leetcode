需要用[TeX All the Things](https://chrome.google.com/webstore/detail/cbimabofgmfdkicghcadidpemeenbffn)查看。

## 3 - [Count Good Triplets](https://leetcode.com/contest/weekly-contest-200/problems/count-good-triplets/)

简单实现。

时间复杂度$o(n^3)$，空间复杂度$O(1)$。

## 4 - [Find the Winner of an Array Game](https://leetcode.com/contest/weekly-contest-200/problems/find-the-winner-of-an-array-game/)

用一个队列来模拟游戏过程，如果遇到原数组里的最大值那么以后的结果永远不会变，可以直接退出循环。

时间复杂度$o(n)$，空间复杂度$O(n)$。

## 5 - [Minimum Swaps to Arrange a Binary Grid](https://leetcode.com/contest/weekly-contest-200/problems/minimum-swaps-to-arrange-a-binary-grid/)

统计每一行尾部有多少个连续的0，对于每一行找其后第一个满足0的数量的行进行交换。

时间复杂度$o(n^2)$，空间复杂度$O(n)$。

## 6 - [Get the Maximum Score](https://leetcode.com/contest/weekly-contest-200/problems/get-the-maximum-score/)

维护两个数组的下标，如果两个数组的下标指向的数字不相等，那么优先移动数值较小的那个；如果相等，那么最大得分为两个数组所在位置的最大值加上当前相等的数字。

时间复杂度$o(n)$，空间复杂度$O(1)$。
