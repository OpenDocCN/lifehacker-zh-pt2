# 如何立即获得一月份的 Android 安全更新

> 原文：<https://lifehacker.com/how-to-get-the-january-android-security-update-right-no-1831645888>

谷歌 2019 年 1 月 月度安卓派 [安全更新现已发布。与之前的更新一样，它修复了 Android 操作系统中许多可能被黑客和恶意程序利用的潜在安全缺陷。虽然这些修复适用于所有 Android Pie 设备，但一月份的更新也有](https://source.android.com/security/bulletin/2019-01-01) [Pixel 3 和 3 XL 特定的修复](https://source.android.com/security/bulletin/pixel/2019-01-01) ，据报道，这将为视频录制带来更好的音频质量。



这一更新从本周开始向所有设备推广。但是，您可能没有收到通知，您的手机已经准备好更新。如果是这样的话，你实际上可以侧装，自己手动安装更新。这比简单地等待更新通知弹出要复杂得多，但你会立即获得安全修复——如果你是 Pixel 3 用户，还会获得改进的音频录制修复。下面是怎么做的。

## 手动安装 Android Pie OTA 更新

在您实际下载并安装更新到您的手机之前，我们需要在我们将从中传输更新文件的 PC 上进行适当的设置。

1.  [从谷歌开发者网站为你指定的 Android 设备下载合适的 OTA 文件](https://developers.google.com/android/ota) 到你的 PC。
2.  将 [ADB 和 Fastboot 下载到您的 PC](https://developer.android.com/studio/releases/platform-tools) ，然后按照 [我们的 ADP 安装和设置指南](https://lifehacker.com/the-easiest-way-to-install-androids-adb-and-fastboot-to-1586992378#_ga=2.43814561.562174998.1547140413-330282983.1530319322) 为您的 PC 操作系统安装。乍一看，这似乎有点复杂，但实际过程很简单，应该只需要几分钟就可以完成。或者，您可以遵循 ADB 的 X [DA 开发人员页面上的安装方法。过程略有不同，但最终做的是同样的事情。](https://www.xda-developers.com/install-adb-windows-macos-linux/)

在您的电脑上安装和配置 ADB 并下载 OTA 文件后，我们现在可以通过引导您的 Android 设备来开始更新过程。

1.  关闭您的 Android 设备，然后通过同时按住电源按钮和音量降低按钮打开它，以启动到引导程序设置。当 Bootloader 设置出现时，使用音量键在选项之间滚动，直到**“恢复模式”**高亮显示，然后快速按下(但不要按住)电源按钮来选择它。
2.  当你第一次进入恢复模式时，你只会看到一个 Android 吉祥物的图像，在它打开的机箱上有一个红色的错误图标，屏幕上有“No command”字样。看到这种情况时，按住电源按钮一会儿，然后按下音量增大按钮。然后，您将进入恢复模式菜单。
3.  使用音量键，向下滚动到**“从 ADB 应用更新”**并轻触电源按钮选择它。你现在会看到一个黑色的屏幕，在底部有一些微小的文字，但是现在还不会有任何反应。
4.  通过 USB 电缆将您的 Android 设备连接到您的 PC(您的手机充电器应该可以正常工作)。
5.  在你的 PC 上，打开一个命令提示符窗口(在 Windows 上可以是命令提示符或 Powershell，在 macOS/Linux 上可以是终端)，根据你的操作系统键入以下命令:

    Windows:**【ADB side load】**
    MAC OS/Linux:**。/adb sideload"**
6.  键入 OTA 更新的名称。zip 文件并按回车键开始更新。
7.  如果一切都配置正确，您将在 PC 和 Android 设备上看到一个进度条，显示更新的安装进度。
8.  更新完成后，使用 Android 设备的音量键滚动到“重启”，然后用电源按钮选择它。然后，您的设备将重新启动，并应用更新文件正常启动。