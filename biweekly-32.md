## 3 - [Kth Missing Positive Number](https://leetcode.com/contest/biweekly-contest-32/problems/kth-missing-positive-number)

$k$的数值很小，直接枚举即可。

时间复杂度$O(k)$，空间复杂度$O(1)$。

## 4 - [Can Convert String in K Moves](https://leetcode.com/contest/biweekly-contest-32/problems/can-convert-string-in-k-moves)

算一下每种转换需要多少个，如果需要转移$s$的个数为$c\_i$，那么需要满足$c\_i \le \lceil (k - s + 1) / 26 \rceil$。

时间复杂度$O(n)$，空间复杂度$O(1)$。

## 5 - [Minimum Insertions to Balance a Parentheses String](https://leetcode.com/contest/biweekly-contest-32/problems/minimum-insertions-to-balance-a-parentheses-string)

记录累计有多少个左括号，然后每次遇到右括号贪心匹配，如果是连续两个右括号则跳过下一个括号，否则在计算步数时需要加1。最后给所有剩下的左括号补上右括号。

时间复杂度$O(n)$，空间复杂度$O(1)$。

## 6 - [Find Longest Awesome Substring](https://leetcode.com/contest/biweekly-contest-32/problems/find-longest-awesome-substring)

首先回文的条件是各个字符个数全为偶数或只有一个字符个数为奇数，而奇偶的统计可以靠异或来记录，因为只有数字，那么可以只用一个整数状态记录当前各个数字的奇偶值。
为了获得最长的字串，只需记录每种状态第一次出现的位置即可。对于当前状态，除了找第一次出现的位置，还需要枚举状态每一位发生改变对应的状态第一次出现的位置。

时间复杂度$O(10n) = O(n)$，空间复杂度$O(2^{10})$。
