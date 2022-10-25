# 用 DarQ 在个别应用上强制安卓 10 的黑暗模式

> 原文：<https://lifehacker.com/force-android-10s-dark-mode-on-individual-apps-with-dar-1841577354>

Android 10 的系统级黑暗主题相当不错，但第三方 DarQ 应用可以解锁隐藏设置，使其更加出色。DarQ 可以让你强制应用程序使用黑暗模式，如果它们没有黑暗模式，你可以使用 DarQ 来指定哪些应用程序获得它， [设置黑暗模式计时器](https://lifehacker.com/use-this-hack-to-create-dark-mode-timers-in-android-10-1838101522) ，等等。谷歌将该应用程序从 Play Store 中移除，因为它可以与 Android 软件中通常禁止使用的部分一起使用，所以你需要从第三方 [XDA 实验室应用程序商店](https://labs.xda-developers.com/store/app/com.kieronquinn.app.darq) 安装它。



你还需要一个有根的手机*或*愿意安装一些额外的软件来使用 DarQ 的功能。如果你有一个根电话，只需安装 XDA 实验室的 DarQ，然后跳到下面的“使用 DarQ”部分开始使用它。

### 使用没有根的 DarQ

那些没有手机 root 权限的用户——也不希望这样——仍然可以使用 DarQ，但是我们需要运行一个特殊的 ADB 脚本，授予 DarQ 特殊权限，这样它就可以按预期运行。这实际上比听起来容易。你需要做的是:

1.  使用[XDA](https://forum.xda-developers.com/showthread.php?t=2588979)的这个包在你的电脑上安装 ADB。
2.  使用 USB 电缆将您的 Android 设备连接到您的 PC
3.  从 XDA 论坛下载并解压 DarQ ADB 脚本。T3】
4.  在 DarQ ADB 脚本文件夹中，双击适用于您的 PC 操作系统的应用程序，然后等待脚本运行。

一旦你运行了 ADB 脚本，你现在就可以使用 DarQ 了——至少在你重启或者关机之前。你需要将你的 Android 手机连接到你的电脑，并在每次重启手机后运行 ADB 脚本。

### 使用 DarQ

从手机的应用程序屏幕打开 DarQ 应用程序。主屏幕包括几个用于强制所有应用程序进入黑暗模式的选项:

*   **启用黑暗主题:**开启 Android 10 的系统级黑暗模式
*   **强制黑暗主题:**让所有应用运行黑暗主题，如果可用的话。
*   **自动黑暗主题:**你的手机会在日出或日落时开启/关闭所有应用中的黑暗模式。

如果您更愿意选择特定应用程序始终运行黑暗模式，请点击**“启用应用程序”**，然后点击每个应用程序旁边的切换按钮。达克会处理剩下的事情。

如果已经运行的应用没有自动切换到黑暗模式，你可能需要重新启动它们。也有可能一些应用的启动速度比 DarQ 开启黑暗模式的速度要快；如果发生这种情况，请尝试强制关闭并重新启动应用程序。如果您遇到任何其他问题，请参考 GitHub 上的 [DarQ 常见问题指南。](https://github.com/KieronQuinn/DarQ/blob/master/app/src/main/assets/faq.md)T3】