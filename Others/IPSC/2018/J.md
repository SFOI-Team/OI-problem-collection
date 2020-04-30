- 题目名：Jumping over walls
- 来源：
  - 竞赛：IPSC
  - 年份：2018
  - 编号：J

你一直都是一位迷宫的狂热玩家，还有些喜欢作弊。难怪你想出了一个可以用来在迷宫中作弊的特殊装置。你只需选择一个方向，这个装置将帮助你跳过这个方向上的墙壁，让你直接跳到这个方向上最近的空地。

你已经构建了两个装置原型。其中 J1 只允许你选择 4 个跳跃方向（上下左右），J2 还允许你沿着对角线跳跃，因此每次跳跃都有 8 个可用方向。

你想制造更多的装置——许多迷宫玩家都希望拥有这样的装置！但在开始销售这些装置之前，你需要对它们进行一些测试，以确保你不会因为销售有缺陷的装置而损坏你的名声。你决定构造一个测试迷宫。

### 问题描述

你将构建两个的测试迷宫，一个用于装置 J1，另一个用于装置 J2。测试迷宫的目的是为了确保装置能在所有支持的方向上正确跳跃，因此要求解决这个迷宫时，每个可用方向必须都要使用至少一次。构建迷宫需要花钱，所有你需要让迷宫尽可能小。

在迷宫中，你只能使用装置跳跃。但请注意，该装置也可以跳过零堵墙，即如果你选择的方向上下一个格子是空地，你将跳到这个空地上。

每个测试迷宫必须满足如下要求：

- 迷宫是矩形，且面积尽可能小；
- 一些格子是墙（#），其他格子是空地（.）；
- 只有恰好一个起点（A）和恰好一个终点（B）。两者都被认为是空地，它们可以被安排在迷宫中的任意位置；
- 我们假设迷宫四周是无限多的墙壁，这意味着跳到迷宫外面是不可能的。
- 必须能从 A 跳到 B。
- 要想从 A 跳到 B，每个可用方向必须都要使用至少一次。

**简单子任务 J1** 的目标是为装置原型 J1（有 4 个跳跃方向）构造满足上述要求的测试迷宫；**困难子任务 J2** 的目标是为装置原型 J2（有 8 个跳跃方向）构造满足上述要求的测试迷宫；

### 输入格式

本题没有输入。

### 输出格式

输出的第一行包含两个整数：行数 $r$ 和列数 $c$。$r \times c$ 的值应该尽可能小。

接下来 $r$ 行，每行 $c$ 个字符，描述你构造的迷宫。

### 样例

#### 一个可能的输出

```plain
5 6
......
.#.#.B
###...
#A#...
#.#...
```

这是一个在语法上正确的输出，但它描述的迷宫并不满足要求。因为可以在不向下跳的情况下解决这个迷宫（你可以向右跳三次，然后向上跳两次）。

对于上面的迷宫，如果你用 J2 装置来解决的话，你的第一次跳跃有四种可能性：

- 向下跳 1 格；
- 向上跳 3 格；
- 向右跳 2 格；
- 向右上方跳 3 格。

请注意，如果该方向上没有空地，你就不能选择往该方向跳跃。