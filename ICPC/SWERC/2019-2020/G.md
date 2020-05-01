- 题目名：Swapping Places
- 来源：
  - 竞赛：SWERC
  - 年份：2019-2020
  - 编号：G
- 时间限制：1000 ms
- 空间限制：? MiB
- 类型：传统

### 题目描述
现在有一个字符串序列，如果一对字符串可以交换且它们相邻，则它们可以交换，求经过交换后，字典序最小的字符串序列。
### 输入格式
第一行三个整数 $s,l,n$。$s$ 代表字符串的种类个数，$l$ 代表可以交换的字符串对数，$n$ 代表字符串序列的长度。

接下来 $s$ 行，每一行的字符串代表在接下来的输出内会出现的字符串。

接下来 $l$ 行，每行两个字符串，表示两个字符串可以进行交换。

接下来一行 $n$ 个字符串，表示字符串序列。
### 输出格式
一行 $n$ 个字符串，经过交换后，字典序最小的字符串序列。
### 样例输入
```
3 2 6
ANTILOPE
CAT
ANT
CAT ANTILOPE
ANTILOPE ANT
ANT CAT CAT ANTILOPE CAT ANT
```
### 样例输出
```
ANT ANTILOPE CAT CAT CAT ANT
```
### 样例解释
共有六种可能的顺序：

1. `ANT ANTILOPE CAT CAT CAT ANT`
1. `ANT CAT ANTILOPE CAT CAT ANT`
1. `ANT CAT CAT ANTILOPE CAT ANT`
1. `ANT CAT CAT CAT ANT ANTILOPE`
1. `ANT CAT CAT CAT ANTILOPE ANT`
1. `ANTILOPE ANT CAT CAT CAT ANT`
### 数据范围及限制
对于 $100\%$ 的数据，保证 $1\le s\le 200$，$0\le l\le 10^4$，$1\le n\le 10^5$，读入的字符串中仅含有大写字母且 $1\le $ 读入的字符串长度 $\le 20$。
