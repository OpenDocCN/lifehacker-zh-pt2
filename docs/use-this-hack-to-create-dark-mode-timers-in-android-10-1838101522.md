# 使用这个黑客在 Android 10 中创建“黑暗模式”计时器

> 原文:[https://life hacker . com/use-this-hack-to-create-dark-mode-timers-in-Android-10-1838101522](https://lifehacker.com/use-this-hack-to-create-dark-mode-timers-in-android-10-1838101522)

我可以在任何操作系统、应用程序或网站上启用深色主题，升级到 Android 10 意味着我现在可以 [将深色主题设置为系统级所有支持的应用程序和菜单的默认外观](https://lifehacker.com/how-to-find-gmails-new-dark-mode-setting-1838066217)。

Watch

虽然我完全满足于只打开黑暗模式并且永不回头，但是你可能更喜欢根据一天中的时间或者你的环境在黑暗和光明模式之间切换。不幸的是，即使是 Android 10 也没有一个简单的方法来做到这一点，你不得不从系统设置或每个应用程序中手动改变主题，除非你寻求外部帮助。

理想情况下，Android 会有一个内置的调度程序，在设定的时间自动在亮暗模式之间切换，但碰巧有一个名为 **Automatic Dark Theme** 的第三方应用程序可以做到这一点。S 安装这个应用比平常要复杂一点，但是绝对值得一试。

1.  从 Google PlayT3 安装 [自动黑暗主题。](https://play.google.com/store/apps/details?id=com.cannic.apps.automaticdarktheme)
2.  进入到**设置>关于手机**，然后点击 **【版本号】**七次，直到你看到一个确认你已经启用开发者模式的弹出窗口。
3.  接下来，进入**设置>系统>开发者选项。**
4.  向下滚动，打开**“USB 调试”**
5.  O 在你的电脑上，使用这个来自 XDA 论坛的 15 秒安装包安装 ADB。
6.  通过 USB 充电器将手机插入 PC。
7.  通过按下**“Windows+R”**，然后键入**“cmd”，打开 PC 上的命令提示符**在命令提示符窗口中，键入:`adb shell pm grant com.cannic.apps.automaticdarktheme android.permission.WRITE_SECURE_SETTINGS`
8.  按**“回车”**运行命令。
9.  应用更改后，您可以关闭命令提示符并断开电话与 PC 的连接。然后你也应该能够关闭 USB 调试(为了额外的安全)。

安装了应用程序，下面是如何在自动黑暗主题中设置计时器:

1.  打开自动黑暗主题 app。
2.  点击**“启用”**旁边的滑块，打开定时器。
3.  点击**“在**启用暗主题”或**“在**启用亮主题”来调整每个主题的应用次数。

您还可以更改应用程序是在指定的时刻应用更改，还是仅在屏幕锁定时应用更改。在手机屏幕锁定时切换是首选的选项。O 否则，当主题改变时，任何打开的应用程序或菜单都必须重新加载，这可能会导致视觉错误或性能问题。