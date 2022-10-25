# 如何使用 Excel 的 Xlookup，更新更强大的 Vlookup

> 原文：<https://lifehacker.com/how-to-use-excels-xlookup-the-newer-and-more-powerful-1838636148>

我还记得第一天我想出如何在 Excel 中运行一个 vlookup 命令；我坐在我的咖啡桌旁，不知道这个愚蠢的小命令有什么意义。一旦我意识到它的力量，我就再也没有回去过。作为斯坦福大学的一名商业分析师，我经常求助于 vlookup 来完成一天的工作。

Watch

你会问，什么是 vlookup？对于不知情的人，这个有趣的小 Excel 命令允许您根据另一个值的位置提取一个值。例如，假设您有一个如下所示的电子表格:

如果您运行一个 vlookup，那么您可以告诉单元格(f5)在一个列(比如“bus”)中查找一个值，然后从同一行的另一列中返回一个值(" blue" )。Hlookup 以同样的方式工作，只是颠倒了行/列的名称:在一行中查找一个值，然后从更下面的另一行返回一个值。

现在我们来到了 xlookup，正如微软的 [乔·麦克戴德](https://techcommunity.microsoft.com/t5/Excel-Blog/Announcing-XLOOKUP/ba-p/811376) 所描述的，“标志性的 vlookup 功能的继承者”。它是这样工作的:

> XLOOKUP 因其能够垂直和水平查看而得名(是的，它也取代了 HLOOKUP！).在其最简单的形式中，XLOOKUP 只需要 3 个参数来执行最常见的精确查找(比 VLOOKUP 少一个)。让我们以最简单的形式来考虑它的签名:

> *XLOOKUP(查找值，查找数组，返回数组)*
> 
> ***查找 _ 值:**你要找的东西*
> 
> ***lookup_array:** 去哪里找*
> 
> ***返回 _ 数组:**返回什么*

因此，回到我的例子，如果您想找到与单词“house”相关联的颜色并将该信息提取到一个单元格中，您只需键入:

`xlookup(“house”,a:a,c:c)`

简单。

Xlookup，除了是一个比 vlookup 更短的命令之外，还可以让你使用精明的 vlookup 用户梦寐以求的功能:反向搜索。换句话说，你现在也可以拉进锚点左边的值，而不是默认的右边。这简直是魔术。

不幸的是，今天不是每个人都能玩 xlookup。微软正在向 [Office 365 内部人士](https://insider.office.com/en-us/) 率先推出该功能。所以，如果你想在其他人之前掌握 xlookup，你最好进入测试版。