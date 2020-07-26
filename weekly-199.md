需要用[TeX All the Things](https://chrome.google.com/webstore/detail/cbimabofgmfdkicghcadidpemeenbffn)查看。

## 3 - [Shuffle String](https://leetcode.com/contest/weekly-contest-199/problems/shuffle-string)

简单实现。

## 4 - [Bulb Switcher IV](https://leetcode.com/contest/weekly-contest-199/problems/bulb-switcher-iv)

从前向后，如果当前位置需要翻转就翻转。

时间复杂度$O(n)$，空间复杂度$O(1)$.

## 5 - [Number of Good Leaf Nodes Pairs](https://leetcode.com/contest/weekly-contest-199/problems/number-of-good-leaf-nodes-pairs)

从下至上统计当前节点到所有叶子的距离种类的个数，因为最多也就$n / 2 = 512$个叶子，考虑类似完全二叉树，最顶端左右各$n / 4$个叶子，计算量大概是：

$\left ( \frac{n}{4} \right ) ^ 2 + 2 \times \left ( \frac{n}{8} \right ) ^ 2 + 4 \times \left ( \frac{n}{16} \right ) ^ 2 + \cdots$

由于系数下降非常快，结果明显小于$n^2$，而且记录的是每种距离有多少个，实际计算量还会远远小于$n^2$.

时间复杂度$o(n^2)$，空间复杂度$O(n)$.

## 8 - [String Compression II](https://leetcode.com/contest/weekly-contest-199/problems/string-compression-ii)

### 方法1

明显的动态规划，令最大删除次数为$K$，$\text{len}(x)$表示连续$x$字符需要用多少长度的数字表示。
用$dp_{i, k, l} = 1$记录以$i$（从0开始）的字符为结尾，已经有连续$l$个`s[i]`对应的字符，已经使用了$k$次删除的情况下的最短长度。
同时用另外的数组记录一下$\min\_{l} dp_{i, k, l}$。

边界条件：

如果$i = k$，那么可以删除之前所有字符，只保留`s[i]`，$dp_{i, i, 1} = 1$。

递推：

对于每一组$i$和$k$，枚举向前删除$0$到$k$的连续区间，令区间被删除后前一个位置为$j$，则：

* 如果`s[i] == s[j]`，枚举$l$，则增加连续值，$dp\_{i, k, l} = \min (dp\_{i, k, l}, \text{len}(l) - \text{len}(l - 1) + \min\_j dp\_{j, k - (i - j - 1), l - 1})$.
* 如果`s[i] != s[j]`，则与之前不连续，新的连续长度为1，$dp\_{i, k, 1} = \min (dp\_{i, k, l}, 1 + \min\_{l} dp\_{i, k, l})$.

复杂度：

虽然看起来有4层循环，但`s[i] == s[j]`里面的枚举最多执行12743775次，而在`s[i] != s[j]`里需要枚举的最小值已经被记录，不需要循环，时间复杂度控制在$O(n^3)$。

### 方法2

用$dp_{i, k} = 1$记录到$i$（从1开始）为止，已经使用了$k$次删除的情况下的最短长度。

边界条件：

$dp_{0, 0} = 0$

递推：

* 如果删除当前字符，那么$dp\_{i, k} = \min(dp\_{i, k}, dp\_{i - 1, k - 1})$；
* 如果不删除当前字符，那么从当前为止$i$尽可能往后延伸，将`s[i]`作为连续字符的起始（如果前面的字符和`s[i]`相同，则前面延伸长度一定大于当前长度，编码长度不会更长）。令$j>i$且$[i, j]$之间有$d$个字符与`s[i]`不同，$k \ge d$, 那么$dp\_{j, k} = \min(dp\_{i - 1, k - d} + 1 + \text{len}(j - i + 1 - d))$。


时间复杂度$o(n^3)$，空间复杂度$O(n^2)$.
