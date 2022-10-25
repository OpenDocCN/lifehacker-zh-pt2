# 使用此快捷键在 Mac 上的暗模式和亮模式之间切换

> 原文：<https://lifehacker.com/switch-between-dark-and-light-mode-on-your-mac-with-thi-1838488087>

[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)) : title[![](../Images/80a55aae3a4e6ac59b23fae8fccddf22.png)](https://applemacos.kinja.com)[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)Many people turn to Macs because they're incredibly easy to operate. That's true, but there's still plenty worth knowing before you can truly master your Mac.

Mojave 引入的 macOS 最好的部分之一是操作系统的黑暗模式。这是一个全系统的触发器，在你的核心 Mac 应用程序和任何支持该功能的第三方应用程序中给你一个更暗淡的颜色主题——我认为它对眼睛来说更容易，但也许这只是我的看法。

Watch

升级到 macOS Catalina，你甚至会得到一个额外的设置——“自动”，它会根据时间在亮暗模式之间切换你的系统。但是，如果您想要手动控制您正在使用的“模式”呢？不得不在系统偏好设置中导航，在亮暗模式之间切换，这是一件痛苦的事情。相反，只要有一点创意，你就可以设置一个键盘快捷键，让你在这两个世界之间穿梭，速度比 [林克的魔镜](https://zelda.fandom.com/wiki/Magic_Mirror) 还要快。

### 设置键盘快捷键以在 macOS 中切换明暗模式

首先，在 macOS 中打开 **Automator** 应用程序。点击文件>新建，并从出现的菜单中选择快速操作:

在下一个屏幕中，将第一个下拉菜单设置为“工作流接收电流...”从“自动(文本)”到“无输入”

然后，点击第二栏“激活字体”上方的小搜索框。输入“苹果”，双击“运行 AppleScript”。删除框中出现的所有紫色文本，改为输入以下内容(由 [AppleInsider](https://appleinsider.com/articles/18/06/14/how-to-toggle-dark-mode-with-a-keyboard-shortcut-or-the-touch-bar) 提供):

`tell application "System Events"`

`tell appearance preferences`

`set dark mode to not dark mode`

`end tell`

`end tell`

你现在应该可以点击第一行文字上方的“播放”图标，这样做应该可以将你的系统从黑暗模式切换到光明模式(然后再切换回来)。保存您的快速操作(通过 Command + S ),并给它一个您稍后会记住的名称(一分钟内)。

退出 Automator 并调出**系统偏好设置**。打开键盘，点击快捷键标签。点击左栏中的“服务”,然后向下滚动右栏找到您的新快速行动——可能在“常规”下通过点击“无”，然后“添加快捷键”，然后你想使用的任何一个或几个键来启动或关闭黑暗模式。

如果这是你第一次设置这样的东西，你也可能会被要求某种许可。确保你接受，否则你的热键设置将无法工作。