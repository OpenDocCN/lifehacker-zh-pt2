# 如何为你的安卓系统获取华硕 ROG 手机 3 的动态壁纸

> 原文:[https://life hacker . com/how-to-get-ASUS-rog-phone-3s-live-wallpapers-for-your-a-1844498897](https://lifehacker.com/how-to-get-asus-rog-phone-3s-live-wallpapers-for-your-a-1844498897)

华硕的 ROG Phone 3 是一款强大的专注于游戏的设备。甚至它的壁纸也被设计成当你打开它的高性能“X 模式”时会产生动画效果其目的是唤起那种“极限游戏”的氛围(有时是错误的)，但动画壁纸实际上看起来非常整洁——多亏了 XDA 论坛用户 linuxct，你现在可以在任何运行 Android 9 或更高版本的 手机上安装它们。

Watch

Linuxct 甚至创建了一个特殊的 X-Mode Toggler 应用程序，模拟 X-Mode 按钮来启用壁纸动画。配套 app 需要使用壁纸，但按下按钮纯粹是审美；我不会影响你手机的性能。

你可以从 XDA 开发者 那里下载 ROG Phone 3 的动态壁纸和 linuxct 的 X-Mode 应用 [，但是你需要做一些事情来将所有东西安装到你的 Android 手机上。这个过程还需要一台个人电脑、一根 USB 线和一个 ADB 工具。](https://www.xda-developers.com/download-asus-rog-phone-3-live-wallpapers/)

### 如何安装 X 模式的托格勒和 ROG 现场壁纸

1.  从上面的链接下载 X-Mode Toggler 应用程序和壁纸 apk 到你的 Android 手机。
2.  提取文件，然后点击安装 X 模式的托格勒 APK 和任何你想使用的壁纸的 apk。
3.  在你的手机上，进入**设置>关于手机，**然后点击**“Build Number”**七次进入开发者模式。
4.  退出并进入**设置>系统>高级>开发者选项。**向下滚动并切换**“USB 调试”**
5.  将 ADB 工具下载并安装到您的电脑上。如果你以前没有这样做过，这本指南 将会帮助你。)
6.  用 USB 线把你的手机和电脑连接起来。
7.  打开你的 ADB 工具或者你电脑的命令行窗口，运行下面的命令: *`adb shell pm grant space.linuxct.rogcontroller android.permission.WRITE_SECURE_SETTINGS`*
8.  命令运行后，您现在可以使用实时壁纸了。
9.  转到手机的壁纸设置。
10.  选择一个 ROG 电话 3 壁纸。
11.  应用壁纸后，在屏幕上向下拖动打开快速访问菜单。
12.  点击**“编辑”**
13.  将 X 模式切换添加到快速访问。
14.  点击快速访问菜单中的 X-Mode 按钮，你的壁纸将进入动画 X-Mode。