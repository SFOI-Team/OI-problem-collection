- 题目名：Biodiversity
- 来源：
   - 竞赛：SWERC
   - 年份：2019-2020
   - 编号：B
- 时间限制：3000 ms
- 空间限制：? MiB
- 类型：传统
- 翻译来源：cnyz

### 题目描述
给定 $n$ 个字符串，如果一个字符串的个数大于其他所有字符串的总数，输出这个字符串，如果没有这样的字符串，输出 `NONE`。
### 输入格式
第一行一个整数 $n$。

接下来 $n$ 行，一行一个字符串 $s_i$。
### 输出格式
如果一个字符串的个数大于其他所有字符串的总数，输出这个字符串，如果没有这样的字符串，输出 `NONE`。
### 样例
#### 样例输入 1
```
3
frog
fish
frog
```
#### 样例输出 1
```
frog
```
#### 样例输入 2
```
4
cat
mouse
mouse
cat
```
#### 样例输出 2
```
NONE
```
### 数据范围与限制
对于 $100\%$ 的数据，保证 $1\le n\le 10^5$，$1\le |s_i|\le 20$，读入的字符串只包含字母和数字。
