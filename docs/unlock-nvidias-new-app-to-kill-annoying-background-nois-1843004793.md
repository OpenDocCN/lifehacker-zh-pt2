# 解锁英伟达的新应用程序，消除恼人的背景噪音

> 原文:[https://life hacker . com/unlock-nvidias-new-app-to-kill-nois-background-nois-1843004793](https://lifehacker.com/unlock-nvidias-new-app-to-kill-annoying-background-nois-1843004793)

游戏很棒，尤其是在疫情期间，尤其是现在你可以玩带有实时光线跟踪 的《我的世界》 [的增强版——但你现在可以使用 Nvidia 显卡来创造现实生活中的魔法。看看这个降噪演示，全部由您的 Nvidia GPU 提供支持:](https://kotaku.com/minecraft-gets-graphics-overhaul-later-this-week-on-pc-1842858362)

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1252789873699745792&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1252789873699745792&autosize=1) Watch

Nvidia 最近发布了其新的 [**RTX 语音**](https://www.nvidia.com/en-us/geforce/guides/nvidia-rtx-voice-setup-guide/) 应用程序的测试版，如果你有 Nvidia GeForce 或 Quadro 显卡，值得一试——对不起，Mac 用户。第一，免费；第二，也是更重要的一点，当你试图与他人交谈时，它在清除背景噪音方面做得非常出色。

一个警告？由于该应用程序由您的 GPU 驱动，如果您在玩游戏时使用该应用程序清理语音聊天，您可能会每秒丢失几帧。对于大多数人来说，这不应该是一个问题，但如果你正处于“丝滑流畅的游戏体验”和“看起来像屁股”之间，要知道启用 RTX 语音可能不值得权衡。

### 如果你没有英伟达 RTX 显卡，不用担心

正如许多人已经注意到的，如果你试图在没有新的 RTX 品牌的 Nvidia 卡的系统上安装这个测试版，安装程序就会失效。然而，有一个快速的解决方法。要么使用 [大卫莱克](https://forums.guru3d.com/threads/nvidia-rtx-voice-works-without-rtx-gpu-heres-how.431781/) 的这个变通办法，要么使用 [这个单独的第三方安装程序](https://forums.guru3d.com/threads/nvidia-rtx-voice-works-without-rtx-gpu-heres-how.431781/#post-5781512) 。到目前为止，人们在 10 系列 Nvidia 卡(或更新)上使用它似乎没有问题，但 9 系列卡可能会有问题。

### RTX 之声入门

如果你准备好了，就拿起[app](https://developer.nvidia.com/rtx/broadcast_engine/secure/NVIDIA_RTX_Voice.exe)和 [最新的 GeForce 驱动](https://www.geforce.com/drivers) 。先装后者，再装前者。RTX 之声的安装过程很简单，因为你甚至不需要选择任何选项。同意许可协议，让安装程序运行，一分钟左右你就可以完成了:

当您单击“关闭”时，您将从 Windows 得到一条小消息，告诉您默认的扬声器已经更改。您还会看到 RTX 之声的弹出窗口:

你可以指定你想要使用的输入设备，但是我发现使用“默认”最简单，它使用你通过正常的 Windows 界面选择的任何设备。此外，Nvidia 建议仅对您的输入设备使用噪声抑制，以免加重您显卡的负担:

> 我们建议为您的麦克风打开 RTX 语音，只有在需要时才打开扬声器。虽然质量几乎保持不变，但在某些情况下可能会有微小的差异，而且该解决方案会占用系统资源，如果您不需要，可以避免使用这些资源。”