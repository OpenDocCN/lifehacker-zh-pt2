# Android 用户:现在检查一下，看看流氓应用程序是否能控制你手机的摄像头

> 原文:[https://life hacker . com/Android-users-check-now-to-see-if-a-rogue-app-can-cont-1839966895](https://lifehacker.com/android-users-check-now-to-see-if-a-rogue-app-can-cont-1839966895)

根据 Checkmarx 安全研究人员的调查，一些 [Android 设备可能有一个未修补的安全漏洞](https://www.checkmarx.com/blog/how-attackers-could-hijack-your-android-camera) ，一个应用程序可以在你不知情的情况下使用你设备的摄像头和麦克风记录你。

Watch

谢天谢地，到目前为止还没有利用 漏洞进行攻击的报道。尽管如此，Checkmarx 的研究人员仍然能够成功地创建和执行可以远程记录电话的命令；捕获照片、视频和音频。从照片中访问 GPS 元数据；甚至检查手机是否朝下——这意味着黑客有一天可能会为运行设备默认相机应用程序的未打补丁版本的设备创建自己的聪明攻击。

谷歌和三星今年早些时候发布了受影响智能手机的补丁，但 Checkmarx 的报告表明，许多其他 Android 智能手机仍可能受到影响。幸运的是，有一些方法可以检查你的设备是否被打了补丁。

### 检查 Pixel 手机上的漏洞

Pixel 用户可以轻松检查补丁:只需打开你设备的设置，然后进入**应用&通知>查看所有应用>相机>高级>应用详情**即可打开应用的谷歌 Play 商店页面。如果该应用程序自 2019 年 7 月以来一直在更新，你就没事了。

### 检查其他 Android 设备上的 bug(手动)

如果你不确定你的智能手机制造商是否发布了修复该漏洞的手机相机应用程序更新，一种方法是尝试自己利用该漏洞(由 Ars Technica 负责)。

你需要:

*   一台 PC(这将在 Windows、Mac 和 Linux 上运行)。
*   你的安卓设备。
*   一根 USB 线来连接它们。

一旦你有了这些材料，下面是你需要做的:

1.  首先，你需要在你的电脑上安装和配置 ADB 工具。在 XDA 开发者论坛 上可以找到为你的电脑操作系统安装 ADB 的所有必要文件和说明 [。](https://www.xda-developers.com/install-adb-windows-macos-linux/)
2.  ADB 安装和配置完成后，用 USB 线将您的 Android 手机插入 PC。接下来，我们将尝试使用代码来强制手机在不访问手机相机应用程序的情况下拍摄视频和照片。
3.  打开 PC 的命令终端。**在 Windows 上:**按“Windows 键+R”，然后键入“cmd”并点击“运行”**在 Mac 上:**按“Command+Space”打开 Finder，然后输入“终端”，双击终端图标运行。
4.  在命令提示符窗口中，一次运行一个命令:

`adb shell am start-activity -ncom.google.android.GoogleCamera/com.android.camera.CameraActivity —ezextra_turn_screen_on true -a android.media.action.VIDEO_CAMERA —ezandroid.intent.extra.USE_FRONT_CAMERA true`

然后:

`adb shell am start-activity -ncom.google.android.GoogleCamera/com.android.camera.CameraActivity —ezextra_turn_screen_on true -a android.media.action.STILL_IMAGE_CAMERA —ez android.intent.extra.USE_FRONT_CAMERA true —eiandroid.intent.extra.TIMER_DURATION_SECONDS 3`

打开手机的相机应用程序，进入你的照片/视频库，检查命令是否有效。如果你发现一个新的照片或视频，那么你的设备上就有 bug。

如果你有一段时间没有更新你的设备的相机应用程序，尝试通过谷歌 Play 商店检查更新。一旦你安装了你的手机的默认相机应用程序可用的任何东西，再次尝试上述 ADB 命令。如果它们仍然工作，您应该尽快向设备制造商报告该问题。此外，远离未知的相机、视频或音频记录应用程序，因为这是黑客最有可能将恶意代码植入你的设备并拍摄几张照片的方法。