# 如何在 Chrome 的匿名模式下通过付费墙

> 原文:[https://life hacker . com/how-to-get-past-pay walls-in-chromes-incognity-mode-1835513589](https://lifehacker.com/how-to-get-past-paywalls-in-chromes-incognito-mode-1835513589)

绕过付费墙——并检测用户这样做的方法——是新闻出版商和读者之间的一场猫捉老鼠的游戏，已经持续了一段时间。虽然在匿名模式下浏览网站一直是~~向记者隐瞒~~绕过网站对你在任何给定时间可以浏览多少免费文章的限制的屡试不爽的方法，但出版商也不是没有自己的花招。最近，一些网站在如何检测匿名模式方面变得更有创意:

Watch

我们之前讨论过一个特殊的标志，你可以在 Chrome 的设置中进行调整，这个标志可以防止网站知道你正在使用匿名模式。截止到 Chrome 74，效果不是很好。

现在，如果你将浏览器升级到 Chrome 75——点击右上角的三点图标，点击帮助，然后点击“关于谷歌 Chrome”——这个小技巧实际上似乎又起作用了。要启用它(如果你以前没有)，在地址栏中键入 **chrome://flags** ，搜索短语“filesystem”，并在下拉菜单中选择“Enabled”作为“Filesystem API in Incognito”设置。

不过，这都是一个有争议的问题，因为谷歌在 Chrome 76 中默认启用了这个标志，这大大增加了赌注，Chrome 76 定于 7 月底公开发布。如果你现在想试试，你可以下载最近发布的浏览器 [Beta 通道版本](https://www.chromestatus.com/features/schedule) 。

新闻出版商对 Chrome 即将到来的调整感到兴奋吗？大概不会。他们会找到另一种方法来检测和限制运行隐名模式的 Chrome 浏览器吗？大概如此。

这应该没什么关系，因为你真的应该向你最喜欢的出版商支付少得可怜的新闻订阅费。这是合法的明智之举。然而，对于一篇偶尔出现的一次性文章来说，隐姓埋名模式——一种已经存在了十多年的伎俩——在道德上就像回到好市多(Costco)购买第二份免费样品一样可疑。不要滥用它，因为那样你就是一个混蛋，但是如果你用它在一个月内看了四篇文章，而不是你被允许享受的三篇免费文章，不要有道德恐慌。它发生了。

### 如何测试你的浏览器是否隐藏了匿名模式

如果你好奇一个网站是否能知道你是否在使用 Chrome 的匿名模式，那就访问这个奇怪命名的网站[【jsfiddle.net/w49x9f1a/】](https://jsfiddle.net/w49x9f1a/)。当你打开它时，网站会运行一个快速测试，并在你浏览器的角落报告结果:

目标？确保该网站声明您的浏览器没有运行匿名模式。如果该网站正确地检测到隐名模式，那么一定是出了问题:要么你运行的是一个旧版本的 Chrome，你没有正确地设置前面提到的标志，要么 Chrome 在隐名模式 下对 [文件系统 API 的实现出了问题。](https://www.bleepingcomputer.com/news/google/google-fixing-chrome-api-to-prevent-incognito-mode-detection/)