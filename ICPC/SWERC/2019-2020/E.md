- 题目名：Pixels
- 来源：
  - 竞赛：SWERC
  - 年份：2019-2020
  - 编号：E
- 时间限制：3000 ms
- 空间限制：? MiB
- 类型：传统

### 题目描述
您现在要显示一幅图片，但是，屏幕出现了故障，如果您选择显示第 $x$ 行，第 $y$ 列的像素，那么，第 $x+1$ 行，第 $y$ 列的像素、第 $x-1$ 行，第 $y$ 列的像素、第 $x$ 行，第 $y+1$ 列的像素、第 $x$ 行，第 $y-1$ 列的像素均会被改变。

上述的改变指若像素已被显示则让其不被显示，若未被显示则反之。

现在，我们会给您这幅图片，请您输出您选择显示像素。

如果我们的图片无法显示，请输出 `IMPOSSIBLE`。

### 输入格式
第一行两个整数 $k$ 和 $l$。

接下来 $k$ 行，每行 $l$ 个字符，用空格隔开。

如果第 $i$ 行，第 $j$ 列有一个字符 `B`，说明这里需要有一个像素。

如果第 $i$ 行，第 $j$ 列有一个字符 `W`，说明这里不需要有一个像素。
### 输出格式

**本题存在 SPJ**。

共 $k$ 行，每行 $l$ 个字符，用空格隔开。

如果第 $i$ 行，第 $j$ 列有一个字符 `A`，说明您选择显示这里的像素。

如果第 $i$ 行，第 $j$ 列有一个字符 `W`，说明您不选择显示这里的像素。

### 样例
#### 样例输入 1
```
1 2
B W
```
#### 样例输出 1
```
IMPOSSIBLE
```
#### 样例解释 1
两个像素，选择一个像素显示，另一个像素也必定会改变，无法达成要求。
#### 样例输入 2
```
5 22
B B B W B W W W B W B B B W B B B B W B B B
B W W W B W W W B W B W W W B W W B W B W W
B B B W B W B W B W B B B W B B B B W B W W
W W B W B W B W B W B W W W B W B W W B W W
B B B W W B W B W W B B B W B W W B W B B B
```
#### 样例输出 2
```
A P P A P P A A P A A P P P A A P A P A P A
A P P A P A P P A P A P A A A A A P P P A A
A P P A P P A A A P P A A P P A A P A P A A
A A A A A A P P A P P P A A P A A P P P P A
A P A A A A P A P P P A P A P P A P P P A P
```
### 数据范围及限制
对于 $100\%$ 的数据，保证 $1\le k\times l\le 10^5$，读入的所有字符均为 `B` 或 `R`。
