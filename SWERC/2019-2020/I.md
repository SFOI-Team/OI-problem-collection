- 题目名：Pseudo-Random Number Generator
- 来源：
  - 竞赛：SWERC
  - 年份：2019-2020
  - 编号：I
- 时间限制：1000 ms
- 空间限制：? MiB
- 类型：传统

### 题目描述
给您三个整数 $a,b,c$，请输出：

$$\lfloor \frac{(a+1)\times (b+1)}{c+1}-1 \rfloor$$

### 输入格式
仅一行三个整数 $a,b,c$。

### 输出格式
仅一行一个整数，表示 $\lfloor \frac{(a+1)\times (b+1)}{c+1}-1 \rfloor$。

### 样例输入
```
15 18 11
```
### 样例输出
```
24
```
### 数据范围及限制
对于 $100\%$ 的数据，保证 $1\le a,b\le 10^4$，$1\le c\le \min(a,b)$。
