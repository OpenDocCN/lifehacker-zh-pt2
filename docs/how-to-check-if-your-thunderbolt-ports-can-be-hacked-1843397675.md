# 如何检查你的 Thunderbolt 端口是否可以被黑客攻击

> 原文:[https://life hacker . com/how-to-check-if-your-thunderbolt-ports-can-hacked-1843397675](https://lifehacker.com/how-to-check-if-your-thunderbolt-ports-can-be-hacked-1843397675)

如果你有一台带有 Thunderbolt 端口的电脑，你可能会面临被称为“Thunderspy”的严重固件缺陷的风险。安全研究员比约恩·鲁滕伯格 发现的 [漏洞，影响所有支持 Thunderbolt 线缆的 Thunderbolt 端口和 USB-C 或 DisplayPort 端口。它让黑客可以完全访问您计算机上的所有内容，即使存储在加密的硬件上。有人不仅可以在几分钟内窃取你的所有数据，而且执行的 Thunderspy 攻击也是不可追踪的。你甚至不会知道黑客攻击发生了。](https://thunderspy.io/#intro)

Watch

这是一个严重的漏洞，但只有当攻击者能够物理接触到你的机器并有足够的时间打开它并实施攻击时，它才是可利用的。虽然这听起来很难实现，但 Ruytenberg 和其他研究人员详细描述了 9 种真实世界的场景，黑客可以在不到 5 分钟的时间内轻松进行 Thunderspy 攻击，其中包括“邪恶女仆”方法，即有人闯入酒店房间，在电脑主人不在的情况下应用 Thunderspy。

然而，有些硬件是安全的。

只要没有通过 Bootcamp 安装 Windows 或 Linux，MacOS 电脑就是安全的，缺乏 Thunderbolt 支持的 Windows PCs 也是如此。还有一小部分最近的计算机配备了英特尔的特定安全系统，称为内核直接内存访问保护(内核 DMA)，可以防止 Thunderspy 攻击。你可以 [在这里](https://blogs.intel.com/technology/2020/05/more-information-on-thunderspy/#gs.5rsrl2) 阅读更多关于内核 DMA 的内容。

不幸的是，内核 DMA 是在 2019 年才推出的，这意味着大多数具有符合 Thunderbolt 标准的 USB 和 DisplayPort 插头的计算机都存在风险。

担心的用户可以使用免费的开源诊断应用程序检查他们的机器是否容易受到攻击，如果你有危险，它可以立即通知你。

### 如何安装和使用 Spycheck

1.  在这里 下载 Spycheck [(适用于 Windows 和 Linux)。](https://thunderspy.io/#intro)
2.  解压文件。
3.  在解压后的文件夹中找到并运行“Spycheck”应用程序。
4.  选择您的语言(默认为英语)，然后点击**“下一步”**
5.  点击**“接受”**同意 Spycheck 许可协议。
6.  从列出的选项中选择您电脑的端口配置。点击**“下一步”**运行检查。
7.  下一个屏幕将显示测试结果。
8.  点击**“退出”**关闭应用。

如果 Spycheck 说你有风险，你需要确保你的硬件是安全的——无论是数字上还是物理上。

虽然普通用户不太可能成为直接目标，但在公共场合，您仍然应该练习数据安全。很多都很基本:

*   看好你的物品，不要无人看管。
*   永远不要让陌生人使用你的设备。
*   如果你决定让你信任的人暂时借用你的设备，确保 [创建一个客人档案](https://lifehacker.com/how-to-set-up-guest-mode-on-your-android-1835913254) 供他们使用，而不是你的主账户。
*   最后，如果您要赠送或出售您的旧硬件，请确保通过执行工厂重置来擦除存储在其上的任何数据。