# 如何修复 Windows 10 关机延迟 Bug

> 原文：<https://lifehacker.com/how-to-fix-the-windows-10-shutdown-delay-bug-1835840316>

尽管最近包含了新的 [自动故障排除和解决问题的工具](https://lifehacker.com/solve-windows-10-issues-automatically-with-the-new-reco-1835377734) ，但 Windows 10 的 [版本 1809 更新](https://lifehacker.com/the-best-new-features-in-windows-10s-may-2019-update-1834927597) 引入了相当多的 bug。一个最新的(也是更烦人的)怪癖是阻止你的电脑及时关机或进入睡眠状态。

Watch

### 是什么导致了这个错误

该漏洞是由 Windows 10 的 USB Type-C 连接器系统软件接口(USCI)引起的，该接口处理 USB Type-C 设备的所有连接。在 Windows 10 版本 1809 上，当 PC 关闭或进入睡眠模式时，USCI 似乎需要多花 60 秒来处理断开连接。

虽然令人讨厌，但较长的关机时间似乎是唯一的负面影响；关机和睡眠模式延迟似乎不会导致 USB 连接设备出现任何故障。

### 怎么修

微软 [已经确认](https://techcommunity.microsoft.com/t5/Microsoft-USB-Blog/FAQ-Why-does-my-USB-Type-C-capable-system-take-longer-than/ba-p/718602) 存在 bug，但是还没有发布更新或者补丁来解决。与此同时，你有一个简单的解决方案来加速你的系统缓慢关机:在关闭你的电脑或使其进入睡眠模式之前，断开你的 USB Type-C 设备。

如果你不确定 USB Type-C 是什么，你会想要寻找至少有一个连接器的电缆，如下所示:

USB Type-C 设备的一些示例包括:

*   较新的 Android 智能手机、平板电脑和笔记本电脑，包括所有谷歌 Pixel 手机和 Chromebook Pixel
*   任天堂 Switch
*   新款 macbook

*   一些外置硬盘和固态硬盘

大多数 USB Type-C 设备只需通过 USB 连接充电，并且可以毫不费力地拔出。其他设备(如 Android 设备或外部驱动器)可能正在与您的电脑之间传输数据或发送视频/音频，因此在断开它们之前，您需要确保它们没有在做任何重要的事情。简单的事情，但是如果你因为某种原因不得不快速关闭你的系统时，很容易忘记。(否则，准备再等 60 秒。)