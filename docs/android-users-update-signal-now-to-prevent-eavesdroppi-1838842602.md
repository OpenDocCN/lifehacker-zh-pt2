# 安卓用户:现在更新信号，防止窃听

> 原文：<https://lifehacker.com/android-users-update-signal-now-to-prevent-eavesdroppi-1838842602>

根据谷歌 Project Zero 团队 9 月底的一份错误报告，Android 上流行的秘密消息应用 Signal 的一个问题允许任何攻击者基本上窃听一个人的设备(通过音频，而不是视频)。



正如项目零 [描述的](https://bugs.chromium.org/p/project-zero/issues/detail?id=1943) :

> *“在 Android 客户端中，有一个方法 handleCallConnected 使调用完成连接。在正常使用期间，它在两种情况下被调用:当用户选择“接受”时被叫方设备接受呼叫，以及当主叫方设备接收到指示被叫方已经接受呼叫的呼入“连接”消息时。*
> 
> 使用经修改的客户端，当来电正在进行中但尚未被用户接受时，可以向被叫方设备发送“连接”消息。这使得呼叫被应答，即使用户没有与设备交互。

这对任何受影响的人来说都是一个非常不幸的经历，但是我们有一些好消息。首先，如果你是 iOS 用户，这个 bug 根本不会影响你。第二，对于 Android 用户来说，这个问题已经有了解决方案；你只需更新 [**信号**](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms&hl=en_US) app，如果它还没更新的话。为此，在你的设备上打开 Play Store 应用程序，点击左上角的汉堡图标，点击“我的应用程序&游戏”，然后更新。

你要确保你运行的应用程序版本至少是 4.47.7，你可以打开设置，点击“应用程序和通知”，点击信号(或查看全部...应用程序，如果它不在列表的顶部)，点击高级，并向下滚动到屏幕底部以检查应用程序的版本号。