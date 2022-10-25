# 如何简化混乱的无线网络设置

> 原文：<https://lifehacker.com/how-to-streamline-a-messy-wireless-network-setup-1841491088>

毫无疑问，无线网络很复杂。对于一些人来说，他们很容易发现自己的家庭设置像个科学怪人，因为他们一直在添加设备、接入点、路由器和交换机，谁知道还有什么东西在努力让他们的家周围有一个像样的连接。突然，他们发现自己有很多设备都可以很好地运行，但他们的无线体验仍然有问题。



本周，Lifehacker 读者 **Phil** 将描述他在家里的复杂设置，我们将帮助他——和你——处理一些硬件膨胀问题。他写道:

> *我的情况是在新设备投入使用后让事情运转起来:*
> 
> 1.  我们的家配备了以太网线路，我在家里插了三个 Apple Airport Extremes。它们都使用相同的 SSID 和密码。
> 2.  *ATT 无线公司在调制解调器中嵌入了无线路由器；不需要或不使用他们的无线网络。*
> 3.  *现在用的是频谱，而他们的棱 TM1602A MTA 只有一个调制解调器。我们尝试将调制解调器连接到千兆位交换机上(我们有三个连接到以太网线路和安全摄像头)。*
> 4.  但是由于某种原因，这并没有奏效。技术人员说机场的极端情况将不得不重新配置(？).他不想把这个变量带入等式，主动提出安装一个阿斯基 Wave 2 无线路由器——这样做的结果是我的 Airport Extreme 又工作了。
> 5.  *我试着替换了一个门户无线路由器，因为我喜欢它们的“浪子”功能——但是当我的 Airport Extreme 网络出现时，我无法查看我们的 Logitech Alert 摄像头(如果我不在家，就可以在本地网络上查看)。呃。*
> 6.  然而，我想放弃他们的无线路由器和每月 5 美元的费用。没有多余的无线路由器，是什么阻碍了我们的 Airport Extreme 网络正常工作？
> 
> 请提出任何想法。

在我开始研究这个之前，我正在绞尽脑汁。以下是我会做的，这也是对任何希望以最佳方式配置家庭网络的人的一个好建议。

首先，我会扔掉你从 ISP 那里得到的调制解调器。很有可能你正在为它 支付租赁费，而购买你自己的调制解调器应该在一年后收回成本(然后为你省钱)，如果是这样的话。我和许多其他人，像 [摩托罗拉 MB7621](https://smile.amazon.com/MOTOROLA-MB7621-Approved-Spectrum-Downloads/dp/B077BL65HS?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-streamline-a-messy-wireless-network-setup-1841491088&asc_source=&sa-no-redirect=1&tag=kinjalifehackerlink-20) ，应该可以兼容 Spectrum 的网络，服务速度高达 400Mbps。如果你为千兆服务付费，你幸运儿你，你将需要 Netgear CAX80(无论何时推出)。

从那里，你会想要采取你的机场极端之一，并连接到你的新调制解调器。这将是您网络的主要“路由器”，您用来扩展无线信号的任何其他设备都将是您的“接入点”我这样说是为了让这篇文章简单明了*和*提醒你，你只希望你的网络上有一个设备作为路由器。您连接到网络的其他“路由器”应该停用其路由功能，这样您就不会因为多个防火墙和多个路由器(包括您正在使用的其他路由器)给设备分配 IP 地址而造成内部混乱。

对于 AirPort Extreme，您可以打开“AirPort 实用工具”,进入设备的配置屏幕，并在其网络选项卡 上将“路由器模式”设置为“关闭(网桥模式)】 [。请记住，您只希望在两种机场极端情况下这样做。这两个 AirPort Extreme 应该通过以太网连接到您用作主路由器的单个 Airport Extreme。(我想，这台 AirPort Extreme 可能就在你的电缆调制解调器旁边。)](https://apple.stackexchange.com/questions/154066/configuring-airport-extreme-with-existing-router)

如果你愿意，你可以保留鼓励你购买的任何其他路由器。像以前一样，如果您想将其用作主路由器，请确保连接到它的任何其他“路由器”都作为接入点运行——桥接模式，适用于您的 AirPort 极端情况。如果你想把你的 AirPort Extreme 作为主路由器，你需要把这个神秘的另一个路由器 [变成一个接入点](https://lifehacker.com/how-to-extend-your-wi-fi-network-with-an-old-router-915783308) (如果它还没有你可以设置的“接入点模式”，应该在它的用户指南中详细说明)。然后通过以太网电缆将其连接到主路由器。

这一过程很容易被混淆，因为你也可以*将接入点无线连接到路由器——为连接到接入点的有线设备提供一种访问网络其余部分的方式(或为接入点提供一种扩展 wifi“泡泡”的方式)。这分别称为无线网桥或无线扩展器。如果可以的话，抑制住这样做的冲动，因为这将比你通过以太网将接入点硬连接到路由器慢——听起来你似乎可以做到这一点。*

当我们聊天时，我还建议你给你的每个无线网络(从你的各种无线接入点-你的 AirPort Extremes)一个单独的 SSID。这有违常规，但我喜欢更好地控制我的设备所连接的内容。例如，我将我的无线交流设备放在我的 5GHz 网络上，其他任何不需要那么高速度(或需要稍微长一点的范围)的设备都是 2.4GHz。至少，考虑在你的房子周围设置“Phil_24”和“Phil _ 5”wifi 网络，因为在你的三个机场极限上为你的 2.4GHz *和* 5GHz wifi 网络设置单独的 SSID 可能会变得难以使用。

你还需要确保不同机场的 wifi 网络都使用不同的频道。虽然他们*应该*自动设置，但你很可能需要 [手动设置](https://lifehacker.com/which-wifi-channels-should-i-use-for-my-wireless-networ-1832788063) 。

<aside data-commerce-source="inset" class="sc-16a0mhj-2 gAjHzr">[![Image for article titled How to Streamline a Messy Wireless Network Setup](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/dont-buy-a-new-wifi-router-until-you-check-these-three-1837477352)</aside>

哦。我差点忘了你在问题中隐藏的一个细节。不要将交换机直接连接到电缆调制解调器。几乎在所有情况下，你的家庭网络应该是这样的:**电缆调制解调器>路由器> >其他一切。**将您的路由器视为网络的主网关守卫和控制器。不要在它和它与您的电缆调制解调器之间的甜蜜、纯粹的连接之间放置任何东西，因为如果您的电缆调制解调器只能将一个 IP 地址分配给一个连接的设备(应该是您的路由器，然后它会神奇地为您网络中的所有其他设备分配自己的 IP 地址),这将会导致各种各样的痛苦。(因此它的名字叫做“路由器”。它传送数据。明白了吗？)

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>*</small> 

<small></small>