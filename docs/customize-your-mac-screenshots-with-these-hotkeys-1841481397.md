# 使用这些热键自定义您的 Mac 屏幕截图

> 原文：<https://lifehacker.com/customize-your-mac-screenshots-with-these-hotkeys-1841481397>

我们之前讨论过一些快速截取 macOS 屏幕截图的小技巧——是的，我总是要查找哪个键盘快捷键能让你捕捉有和没有 [花哨边框和阴影](https://lifehacker.com/how-to-take-prettier-screenshots-on-a-mac-1828009545) 的窗口。但是常驻生活黑客金融女王出身的截图大师 [丽莎·罗文](https://kinja.com/lisatella) 最近向我透露了一个我以前不知道的 macOS 中的小屏幕黑客。我现在与你分享这个。

Watch

它如此简单，你会奇怪为什么你以前从来没有注意到它——除非每个人*以前都*注意到了它，而我只是对截图快捷方式不太明智。总之，诀窍是这样的。当你使用**命令+ Shift + 4** 在屏幕的某个部分画一个正方形来截图时，你搞砸了，并且在错误的地方开始，不要放弃。相反，按住空格键，你就可以将矩形移动到任何你想要的地方。释放空格键，您可以像以前一样继续调整它的大小。

这在实际操作中更有趣，所以我们来看看:

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1224913758721658880&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1224913758721658880&autosize=1) 

但这还不是全部。

如果你按住 **CTRL + Command + Shift + 4** ，那么你拍的截图会保存到你的剪贴板，而不是你的桌面。如果你只是想在其他地方复制和粘贴一些东西，这可以节省你很多步骤。

戳 **Command + Shift + 4** ，然后在你仍然按住触控板或鼠标的同时释放它，然后你可以使用 **Shift** 来锁定矩形的 x 轴或 y 轴。如果你按住**键/Alt 键**，你将能够从矩形的中心(默认情况下不是角)扩展和收缩矩形。

如果你想变得狂野，并且出于某种原因只对你的 Touch Bar 进行截屏，那就是 **Command + Shift + 6** 。

当然，你也可以在 macOS Mojave 或更高版本中点击 **Command + Shift + 5** 来打开它的截图应用程序，这给了你很多选项来定制你正在拍摄的照片，结果文件将保存在哪里，以及你是否想启用定时器。

### 如何通过 macOS 终端超级定制你的截图

拉起终端，输入以下命令，通用更改你的截图设置(感谢 [科里金尼万的优秀线程](https://twitter.com/CoreyGinnivan/status/1187209574303973376) ):

**默认值写 com。apple . screen capture disable-shadow-bool true**

**默认值写 com。apple . screen capture type-string“png”**
*—将“png”更改为另一种文件格式(如“jpg”或 pdf”)，将您的截图保存为该类型，而不是 png*

**默认值写 com。apple . screen capture location-string/Users/$ { HOME }/Desktop/**
*—修改位置改变 macOS 保存截图的位置*