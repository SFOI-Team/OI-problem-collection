- 题目名：Gnalcats
- 来源：
   - 竞赛：SWERC
   - 年份：2019-2020
   - 编号：D
- 时间限制：300 ms
- 空间限制：? MiB
- 类型：传统
- 翻译来源：cnyz

### 题目描述
有两个栈，现在要对它们做出一些操作。

初始，你可以认为，栈里有无数个数。

**请注意，本题中的可能被插入栈中的元素有两种，一对和一个数。**

一共有七种操作：

| 操作标志 | 作用 |
| :-----------: | :-----------: |
| `C` | 复制栈顶元素并压入栈。 |
| `D` | 弹出栈顶元素。 |
| `L` | 如果栈顶元素为一对，弹出栈顶元素并压入其左边的元素，否则请什么都不做。|
| `R` | 如果栈顶元素为一对，弹出栈顶元素并压入其右边的元素，否则请什么都不做。 |
| `P` | 将栈顶的两个元素相继弹出，将两个元素捆绑成一对后压入栈中，原栈顶元素作为左边的元素，第二个元素作为右边的元素。 |
| `S` | 交换栈顶的两个元素。 |
| `U` | 如果栈顶元素为一对，弹出栈顶元素并依次压入其左边，其右边的元素，否则请什么都不做。 |

如果您并没有看懂上面的话，这里有一个栗子：

设操作序列为 `PSDSPCRPSDUL`。

- 初始的栈为：$1,2,3,4,5,6\ldots$（这里将栈用数列表示，同时用大括号表示一对）。
- 执行 `P` 操作：$\{1,2\},3,4,5,6\ldots$。
- 执行 `S` 操作：$3,\{1,2\},4,5,6\ldots$。
- 执行 `D` 操作：$\{1,2\},4,5,6\ldots$。
- 执行 `S` 操作：$4,\{1,2\},5,6\ldots$。
- 执行 `P` 操作：$\{4,\{1,2\}\},5,6\ldots$。
- 执行 `C` 操作：$\{4,\{1,2\}\},\{4,\{1,2\}\},5,6\ldots$。
- 执行 `R` 操作：$\{1,2\},\{4,\{1,2\}\},5,6\ldots$。
- 执行 `P` 操作：$\{\{1,2\},\{4,\{1,2\}\}\},5,6\ldots$。
- 执行 `S` 操作：$5,\{\{1,2\},\{4,\{1,2\}\}\},6\ldots$。
- 执行 `D` 操作：$\{\{1,2\},\{4,\{1,2\}\}\},6\ldots$。
- 执行 `U` 操作：$\{1,2\},\{4,\{1,2\}\},6\ldots$。
- 执行 `L` 操作：$1,\{4,\{1,2\}\},6\ldots$。

您需要判定两个栈操作完后的结果是否相同，是的话输出 `True`，否则输出 `False`。

### 输入格式
仅两行，一行一个字符串，表示两个栈的操作序列。
### 输出格式
两个栈操作完后的结果是否相同，是的话输出 `True`，否则输出 `False`。
### 样例
#### 样例输入 1
```
PU
SS
```
#### 样例输出 1
```
True
```
#### 样例解释 1
这些操作序列什么都没有做。
#### 样例输入 2
```
L
R
```
#### 样例输出 2
```
True
```
#### 样例解释 2
这些操作序列均不合法，被忽略了。
#### 样例输入 3
```
PSPCRSL
PS
```
#### 样例输出 3
```
True
```
#### 样例输入 4
```
U
C
```
#### 样例输出 4
```
False
```
#### 样例输入 5
```
PL
PR
```
#### 样例输出 5
```
False
```
### 数据范围与限制
对于 $100\%$ 的数据，保证 $1\le $ 操作序列长度 $\le 10^4$，操作序列中仅含有题目描述中的其中操作。
