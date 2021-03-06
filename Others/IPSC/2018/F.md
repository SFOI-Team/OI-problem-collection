- 题目名：Farmer's code
- 来源：
  - 竞赛：IPSC
  - 年份：2018
  - 编号：F

Bob 是一位农民，他种植苹果树。然而，它的树木并不完美，有些树长出的苹果是酸的，有些树的产量又太少，有些树又弯曲了。他的梦想是种出一棵完美对称的树，长出极其甜美的苹果。然而他的遗传学知识并不丰富，所以他需要你的帮助！

### 问题描述

在本题中，你将在 [这个页面](https://ipsc.ksp.sk/2018/real/problems/f_client.html) 与服务器进行交互。

你有 $n$ 棵树，在开始时，所有树的基因和形状都不同，但这可能会根据你的行为而改变。你同时还会得知目标树的图像。

你可以选择任意两棵树来杂交，会发生如下事件：

- 这两棵树的基因将会融合，一棵新树将会长出。新树被认为是最年轻的。
- 所有树中最老的树死亡。因为有一棵树长出，一棵树死亡，树的总数将保持不变。
- 如果你得到了目标树，你将获得该子任务的胜利，该子任务的状态将被标记为 OK。

如果从两个不同的浏览器打开网页，你将看到相同的界面。

如果你认为有必要重新开始的话，你可以点击 reset 按钮执行重置操作，所有树都将回到初始状态，你将得到一个 **Wrong Answer**。你可以根据需要随时执行重置操作（每个子任务的重置次数不限于 10 次）。

但是，你的杂交操作次数是有限的，对于每个子任务，限制是独立的，并将显示在游戏界面上。点击重置按钮时，操作次数**不会**重置。如果操作次数达到上限，你将无法再解决该子任务。

### 输入格式

对于 **简单子任务 F1**，有 $n=4$ 。

对于 **困难子任务 F2**，有 $n=18$。

### 输出格式

你不必提交任何文件，只需与游戏页面交互即可。

### 提示

了解真实遗传学知识可能无法帮助你解决这个问题。

