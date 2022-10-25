# 树莓派 4 最有趣的怪癖

> 原文：<https://lifehacker.com/the-raspberry-pi-4s-most-interesting-quirks-1835871780>



Raspberry Pi 4 Model B 终于来了， [一款 35 美元的设备](https://gizmodo.com/the-new-raspberry-pi-is-basically-a-35-desktop-compute-1835804060) ，它将许多有用的技术集成在一块电路板上，你可以拿在手中。它甚至可能是你的下一台廉价电脑，假设你能忍受狂热爱好者在早期测试中确定的一些权衡。



这个小小的工具为许多人的 [聪明的黑客项目](https://lifehacker.com/top-10-raspberry-pi-projects-for-beginners-1791002723)——包括 [宿舍聚会](https://lifehacker.com/how-to-build-a-party-mode-in-your-dorm-room-1828555615)——提供了动力，在其第四代版本中获得了许多重大升级。理论上，规格令人印象深刻:1.5 GHz，四核，ARM Cortex-A72 处理器；高达 4GB 的内存(将价格提高到 55 美元)；千兆以太网；无线-交流；以及每秒向 4K 显示器推送 60 帧(或每秒向*两个*连接的 4K 显示器推送 30 帧)的能力。

理论上这一切都很好，但是这些变化实际上意味着什么呢？这是我们目前所知的:

### 它变热了

如果你以前玩过树莓派——特别是如果你一直试图尽可能提高它的性能——你可能会遇到 [一些过热问题](https://www.techrepublic.com/article/raspberry-pi-overheating-heres-how-to-stop-it-says-microsoft/) 。树莓 Pi 4 也没什么不同；事实上，它更热。正如加雷思·哈勒菲克里为 [中型](https://medium.com/@ghalfacree/benchmarking-the-raspberry-pi-4-73e5afbcd54b) 所写的:

"...仅仅几分钟后，整个电路板摸起来都很温暖。开始负重，那种温暖变得不舒服；虽然在没有额外冷却的情况下使用主板仍然是完全可能的，但那些希望将主板放入机箱的人会发现，为了避免热节流，需要主动冷却。”

他拍摄了树莓 Pi 4 *和其 2018 年的前身树莓 Pi 3 Model B+的一些可爱的热镜头，我们在下面发表了这些照片。注意你放手指的地方。*

### 它吸收更多的能量

这是一个显而易见的。树莓 Pi 4 改用 USB-C 供电——这是必要的，因为它现在空闲时大约消耗 3.5 瓦，在受胁迫时大约消耗 7.6 瓦。相比之下，树莓 Pi 3 型号 B+在空闲时消耗约 1.9 瓦，在充电时消耗约 5 瓦。

好消息是什么？即使它一年中的每一天每天 24 小时都以最高速度运行，树莓派 4 [也只会让你](https://twocents.lifehacker.com/calculate-the-energy-cost-of-your-appliances-with-this-1694662735) 多花大约 3 美元来运营。

### 它可以处理 4K 显示器，但是...

Raspberry Pi 4 更令人大开眼界的功能之一是其双 HDMI 配置，如上所述，在 4K 显示器上支持每秒 60 帧，在两个 4K 显示器上支持每秒 30 帧。

一想到一台微型单板计算机可以处理 1650 万像素，我就感到震惊，但不要让这个规格欺骗了你。Raspberry Pi 4 可能能够处理 4K 显示器，但这并不意味着它可以很好地运行 4K 视频，甚至 1080p 视频。从 Avram Piltch 在 [汤姆的硬件](https://www.tomshardware.com/reviews/raspberry-pi-4-b,6193.html) :

> “在网上冲浪、看静态图像和享受 4K 的所有额外屏幕空间时，视频播放是树莓派 4 的致命弱点，至少在撰写本文时是这样。无论是尝试播放 4K 的视频还是使用下载的文件，无论是在 Raspbian Buster 还是运行 Kodi 媒体播放器的操作系统 LibreElec 上，我们都没有获得流畅、可行的 4K 体验。包括《钢铁之泪》在内的几个 H.264 编码视频根本无法播放，或者显示为一堆杂乱的颜色。甚至 Kodi 的人推荐给我测试的水母视频样本也是静止的，没有任何运动。显然，为了让 Raspberry Pi 4 能够播放 4K 视频，在操作系统和软件方面仍需要进行大量的优化。
> 
> 不幸的是，在这一点上，即使是 1080p 的 YouTube 视频流也是一个挑战。以 1080p 分辨率运行的《奇异事物》全屏视频预告片显示出明显的抖动。然而，当我在一个较小的窗口中观看相同的剪辑时，播放很流畅。同样的问题发生了，甚至当我把视频流的分辨率降低到 480p 时。
> 
> 如果你的屏幕分辨率为 1920 x 1080 或更低，离线播放 1080p 视频效果很好。我用 VLC 播放器观看《复仇者联盟》最后阶段的下载预告片时，非常流畅。"

### Raspberry Pi 4 处理常见任务的能力如何？

运行大量的综合测试来比较设备是有用的，但很难解释使用设备进行日常任务(视频编码、图像处理、网页浏览等)的感觉。

除了之前的热测试之外，Halfacree 还对 Raspberry Pi 4 进行了一些真实世界的测试，以让您更好地了解实际使用它的感觉(并为其硬件升级提供背景)。

虽然他没有说明他正在处理的文件的大小，我很想知道，但他进行了一个快速的文件压缩测试，并将 Raspberry 4 与现有的所有其他版本的 Raspberry Pi 进行了比较(如果我是正确的)。如你所料，最新最棒的单板电脑版本超越了它的前辈:

当 Halfacree 通过图像编辑测试运行 Raspberry Pi 4 时，这正是你可能使用 35-55 美元的微型电脑执行的操作，性能改善并不十分极端。从他的测试中更能说明问题的是——如果你知道你的 Raspberry Pi 规格的话——当你在你的设备中安装足够的内存时，你能获得多大的性能提升，至少如果你打算处理高分辨率文件的话。

虽然与旧版本的 Raspberry Pi 相比，Raspberry Pi 4 的 1GB 版本仍然很稳定，但如果你打算将这款设备保留一段时间，你还不如花大价钱购买 4GB 版本。皮尔奇写道，拥有一点额外的内存也无妨，尤其是当你打算同时运行多个浏览器标签时。

“我一直关注着 Gnome 系统监视器，我注意到，即使只打开了一两个标签，我也使用了超过 1GB 的内存。然而，在配有 4GB 内存的 Pi 4 上，我可以一次运行 15 个标签，并在它们之间来回切换。”

提升到 4GB 也有助于 Raspberry Pi 4 碾压 [速度计 2.0](https://browserbench.org/Speedometer2.0/) ，这是一个模拟 web 应用程序响应性的综合测试(换句话说，你可能会对谷歌文档等网站有什么样的体验)。

### 树莓 Pi 4 如何修复以前的 Pi 问题

我在 Halfacree 的测试中捕捉到的另一个有趣的花絮是，Raspberry Pi 4 修复了一些令人讨厌的问题，这些问题抑制了组件的性能，而这些组件在以前的 Raspberry Pi 计算机上应该要快得多。典型的例子:千兆以太网。

虽然随着 Raspberry Pi 3 B+的推出，Raspberry Pi 获得了千兆以太网连接，但其性能受到了设备设计的瓶颈( [共享以太网/USB 总线](https://raspberrypi.stackexchange.com/questions/45130/why-do-the-usb-ports-and-ethernet-port-share-the-same-controller/45131#45131) )。这在 Raspberry Pi 4 上是固定的，因为 Halfacree 测量的最大以太网吞吐量为 943 Mbps，而在 Raspberry Pi 3 B+上仅为 237 Mbps。

同样，Raspberry Pi 4 上的 USB 速度也得到了巨大的提升，这要归功于前面提到的 USB 瓶颈的消除以及从较慢的 USB 2.0 端口升级到 USB 3.0。既然 Raspberry Pi 4 能够让 USB 3.0 大放异彩，它确实做到了——至少，当 Halfacree 连接 SSD 并运行一些读写测试时。