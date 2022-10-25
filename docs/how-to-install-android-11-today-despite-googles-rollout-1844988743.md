# 如何在谷歌推出 Android 11 的今天安装它

> 原文:[https://life hacker . com/how-to-install-Android-11-today-尽管-Google-rollout-1844988743](https://lifehacker.com/how-to-install-android-11-today-despite-googles-rollout-1844988743)

Android 11 已经上市——稳定版，也就是说——只有在你运行谷歌的 Pixel 手机(Pixel 2、3、3A、4 或 4A)的情况下才会上市。从今天开始，Android 11 的测试版也可以用于一加 8 和一加 8 Pro，以及 Oppo X2 和雷诺 3。

Watch

由于这是首次展示*(叹息)*，你可能可以通过我们所谓的“简单”方法简单地将你的 Pixel 升级到 Android 11。确保你连接到 wifi，启动你的**设置**应用，点击**系统**，点击**高级**，点击“系统更新”如果你幸运的话，你会看到一个全新的更新，将你的设备一直带到 Android 11(尽管你可能需要先点击“检查更新”选项)。

如果是这样的话，确保你已经备份了手机上任何你不想在错误更新的情况下丢失的东西，然后让我们开始吧。如果没有，你将不得不变得更有创造力一点，才能在你的手机上安装 Android 11，也就是众所周知的“硬”模式。

好吧，这并没有那么难，如果你不耐烦的话，它会让你获得 Android 11，这只是一些你可能从未尝试过的新东西。

### 如何在任意像素上侧装 Android 11

首先将你的 Android 连接到你的 PC——Windows 或 Mac(我使用 Windows 进行演练)——然后再次打开设置应用程序。滚动到底部并点击**关于电话。**在随后的屏幕上向下滚动，并开始点击**“Build number”**，直到你解锁了手机的开发者模式。相信我，你做完这个就知道了。

回到你的主**设置**屏幕，然后点击**系统**，接着点击**高级**和**开发者选项**在这个巨大的菜单中，你需要启用两个选项: **OEM 解锁**和 **USB 调试**。一旦你这样做了，你就可以回到你的机器人的主屏幕。

接下来，下载 [**Android SDK 平台工具**](https://developer.android.com/studio/releases/platform-tools) 并解压到你电脑的某个地方。然后你会想要为你的像素下载正确的 [OTA 图像](https://developers.google.com/android/ota)——首先找到你的设备，然后一路向下滚动并抓取“11.0.0”图像。将它保存或复制到您解压缩 SDK 平台工具的同一文件夹中。

好消息是:这一过程中的征税部分已经基本完成。现在，您需要启动一个命令提示符(或终端),并导航到解压 SDK 平台工具的目录。

假设你的手机还插在电脑上，输入`adb reboot recovery`并回车。如果您在重新启动时看到一个看起来像损坏的 android 而不是菜单的徽标，请按住设备的电源按钮，按下音量按钮，然后松开电源按钮。然后，您需要使用设备的音量和向下按钮来突出显示“应用来自 ADB 的更新”，并通过使用电源按钮来选择它。

最后，在命令提示符中键入`adb sideload [name of the OTA image you downloaded]`，让更新突突地进行。完成后，突出显示“立即重启系统”并使用电源按钮选择它。

你的设备*应该*重启进入 Android 11，你可以随时通过进入**设置>关于手机**并寻找**“Android 版本”来检查**你可能还想访问**设置>系统>高级>系统更新**并再三检查你的手机没有任何新的更新。

一旦你满意了，重新访问开发者选项(设置>系统>开发者选项)并禁用 **USB 调试**。深呼吸和[扎安卓 11](https://lifehacker.com/the-13-best-new-features-of-android-11-1844019029) 和:

或者，嘿，你也可以去 [看看](https://www.android.com/android-11-ar-statue) 雕像。