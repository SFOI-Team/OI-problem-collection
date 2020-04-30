- 题目名：McDroid's
- 来源：
  - 竞赛：IPSC
  - 年份：2018
  - 编号：M

世界上机器人的数量正在快速增长，你决定成为一名企业家并开设世界上第一家机器人餐厅！注意，不是机器人经营的餐厅，而是为机器人服务的餐厅。经过长时间的准备，开业前的一切工作都已经准备就绪。

你有一个很长的菜单，有很多种不同的食物。大多数人可能会感到困惑，因为机器人餐厅的食谱没有名字，只有数字——毕竟机器人只使用二进制。你确信自己的餐厅将会大受欢迎，有很多机器人将会光顾。作为餐厅的老板，你最大的挑战是如何管理你的时间，确保没有人（机器人？）等待太久时间。而你第二大的挑战则是，理解机器人想点的菜并非那么容易。

### 问题描述

在本题中，你将与 [该页面](https://ipsc.ksp.sk/2018/real/problems/m_client.html) 进行交互。

该页面有一个餐厅开业的按钮。当你按下这个按钮时，你的餐厅将会开门，它将会开始接待机器人顾客。你的团队只有一家餐厅，如果你从多个浏览器访问该页面，你将看到同一个餐厅。请注意，即使你关闭页面，餐厅也会继续运行。

每个顾客都将会告诉你他们想要什么，你必须正确给出要提供给他们的食物。游戏机器人可能会告诉你：“你好，我想要点一份 1101。”，在这种情况下，你显然会提供给他们 1101。但对于其他顾客，你将会看到，弄清楚他们想要什么可能会复杂的多。

机器人将会实时到达，每个机器人只愿意等待一段时间（至少一分钟，也许会更长）。你的餐厅同一时刻可能同时有多个机器人在等待。对于每个机器人，你都能看到他们能等待的剩余时间。

当你的餐厅第一次开门时，你将拥有 10 个声誉点。

在你的餐厅中有两种可能出错的情况：

- 如果你向一个顾客提供了**错误的食物**，你将失去一个声誉点，**该顾客**将会离开。
- 如果你**未能及时向一个顾客提供食物**，你将失去一个声誉点，**所有等待的顾客**都会离开。

最初，解决子任务 M1 和 M2 的规则如下：

- 如果你的餐厅的总开业时间达到 $t_1 = 60 \min$，你将解决子任务 M1；
- 如果你的餐厅的总开业时间达到 $t_2 = 180 \min$，你将解决子任务 M2。

每当你的声誉点数耗尽时，你就会破产。你的餐厅可以重新开门来继续解决本问题。每当你的餐厅重新开门时，将会发生如下情况：

- 你将获得 5 个声誉点；
- 如果你还没有解决**子任务 M1**，$t_1$ 将会增加 $20 \min$。
- 如果你还没有解决**子任务 M2**，$t_2$ 将会增加 $20 \min$。
- 作为额外的惩罚，你的餐厅将会有人类顾客光顾，你也需要为人类顾客提供服务。人类通常比机器人更加烦人。

### 注意事项

- 该问题采用正常的评分规则。你越早开始，你解决子任务时的罚时也就越少。
- 游戏页面自动更新，请不要频繁按 F5 刷新页面。如果你这样做，服务器可能会暂时拒绝你的访问请求，你可能无法为某些顾客提供服务。
- 和往常一样，如果你遇到了技术问题，请与我们联系。
- 最后一句警告：随着时间的推移，你的餐厅将会更受欢迎，你将可能接待更挑剔的顾客。

### 输入和输出格式

本题无输入输出。当你的餐厅总开放时间达到预定的阈值时，相应的子问题将自动获得 OK 的结果。