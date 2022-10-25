# 如何将 Android 10 加载到你的 Pixel 上，而不是等待自动更新

> 原文:[https://life hacker . com/how-to-side load-Android-10-on-your-pixel-of-w-1838072534](https://lifehacker.com/how-to-sideload-android-10-onto-your-pixel-instead-of-w-1838072534)

Android 10 已经为 Pixel 手机提供了几天，但一些用户可能还没有收到自动更新。你可以在你的 Pixel 上进入**设置>关于手机>系统更新**来检查待更新；更新可能会在未来几天内到达你的 Pixel，但如果你急于安装 Android 10，不想等待谷歌，你可以手动下载新的操作系统版本。这种方法适用于所有的像素模型，我们将向你展示它是如何工作的。

Watch

### 设置

在升级到 Android 10 之前，有一些 [的事情你应该做，比如备份重要文件。虽然使用本指南中概述的步骤更新到 Android 10 应该会保持你的文件完整，但仍然值得花几分钟额外备份东西，以防出现问题或你因错误](https://lifehacker.com/do-this-before-installing-android-10-on-your-phone-1837842182) 而需要回滚。

备份文件后，你需要将 Android 10 下载到 Pixel 上:

*   你的 Pixel 手机。
*   USB-C 充电线。
*   一台 PC(我们的指南遵循 Windows 的步骤，但谷歌也有针对 Mac 和 Linux 的替代步骤)。
*   ADP 和快速启动工具已下载并安装到您的电脑上。我们已经在其他地方 介绍过如何做到这一点，但是最简单的方法是使用这个来自 XDA 论坛的 [一体化 15 秒安装包](https://forum.xda-developers.com/showthread.php?t=2588979) 。
*   适用于您手机的正确 Android 10 OTA 文件。 [这些可以从谷歌](https://developers.google.com/android/ota) 获得——只要确保你下载的是与你的设备对应的最新更新。您应该将该文件保存在一个容易访问的位置，并确保记下该文件的名称，因为我们稍后将需要它来执行更新命令。

### 在 Pixel 手机上侧装 Android 10

1.  关掉你的 Pixel 手机。
2.  同时按住**电源和音量降低**按钮，直到手机重启并显示引导程序屏幕。
3.  使用音量按钮滚动到**恢复模式**，然后轻按一次电源按钮选择它。
4.  等到你看到 Android 吉祥物躺下，然后同时按下**电源和音量按钮**进入恢复模式。
5.  再次使用音量按钮滚动菜单，突出显示**应用来自 ADB 的更新**，然后按下电源按钮进行选择。
6.  通过 USB 将 pixel 手机连接到 PC。
7.  在你的电脑上，点击**“Windows 键+R”**打开命令提示符，然后输入**“CMD”**找到并运行程序。在命令提示符窗口中执行以下命令:`adb devices`。您的设备应在其名称旁边列出“侧装”。
8.  接下来，使用您之前下载的 OTA 映像的名称键入`adb sideload [filename]`，并按 **Enter。**你应该会在你的设备上看到一些对话框，然后更新应该会开始。等待安装完成。
9.  更新完成后，突出显示**“立即重启”**，然后使用电源按钮选择它。当你的 pixel 再次启动时，它应该正在运行 Android 10。