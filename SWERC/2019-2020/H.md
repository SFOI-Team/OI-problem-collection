- 题目名：Pseudo-Random Number Generator
- 来源：
  - 竞赛：SWERC
  - 年份：2019-2020
  - 编号：H
- 时间限制：300 ms
- 空间限制：? MiB
- 类型：传统

### 题目描述
有一个数列的计算方式如下：
$$\begin{cases}s_0=1611516670\\s_{n+1}=(s_n+(s_n>>20)+12345)\bmod 2^{40}\end{cases}$$

其中 $>>$ 为二进制左移运算。

现在给定 $n$，请您求出 $s_0\sim s_{n-1}$ 中有多少个偶数。

### 输入格式
仅一行一个整数 $n$。

### 输出格式
仅一行一个整数，为 $s_0\sim s_{n-1}$ 的偶数个数。

### 样例
#### 样例输入 1
```
3
```
#### 样例输出 1
```
2
```
#### 样例输入 2
```
500000000
```
#### 样例输出 2
```
250065867
```
### 数据范围及限制
对于 $100\%$ 的数据保证 $0\le n<2^{63}$。