# BitTorrent 初学者指南

> 原文：<https://lifehacker.com/a-beginners-guide-to-bittorrent-285489>

从你的极客室友(他们在晚上的所有时间都在占用你的互联网连接)到你的勒德派家庭成员，几乎每个人都知道现在的 BitTorrent 是什么。他们可能无法描述它是如何工作的，甚至无法合法地使用它，但他们知道它的存在。(如果你是一个有点极客的人，你可能也知道对等网络甚至可以驱动像 [Windows 操作系统更新](https://lifehacker.com/windows-10-uses-your-bandwidth-to-distribute-updates-d-1721091469) 、、 [Chromebook 更新](https://support.google.com/chrome/a/answer/3168106?hl=en) 和 [Android 应用](https://www.androidpolice.com/2018/10/24/hands-google-play-peer-peer-app-sharing-files-go/) 安装这样的过程。)



即使你不关心 BitTorrent 是如何工作的(你应该！)，我们很乐意分享大量关于如何在下载和上传文件时最大化您的体验的技巧。(至少，我们有很多想法，关于你应该使用哪些应用程序来使用*到* Bittorrent，以及如何保持安全。)

首先，让我们谈谈技术——简单地说，我们保证。

### **什么是 BitTorrent？**

BitTorrent 不是一个程序。这是一种使用分布式点对点文件共享系统下载文件的方法。您用来通过 BitTorrent *协议*下载文件的程序称为 BitTorrent 客户端。

BitTorrent 协议的独特之处在于，它将文件共享分配给所有已经下载或正在下载文件的用户。因为 BitTorrent 将文件分解成数百个小块分发，所以在开始共享之前，您甚至不需要下载整个文件。一旦你有了文件的一部分，你就可以开始与其他用户分享。这就是 BitTorrent 如此快速的原因；用户可以在下载完文件后就互相分享文件(而不是等到整个下载完成)。

如果您仍然困惑，让我们尝试一个更简单的方法。正如 [Sampathkumar](https://medium.com/@sampathkumar27896/how-bittorrent-works-79a64d22709c) 在媒体上展示的那样，这是从网站下载普通文件的简化版:

当你从 BitTorrent 下载一些东西时，它看起来有点像这样:

好处？如果一大群 BitTorrenters 中的一个系统很慢，那也没什么——如果幸运的话，会有其他计算机以更快的速度向你发送你正在寻找的文件。如果你只是从一台*慢速服务器下载文件，你会被卡住；由于 BitTorrent 试图一次将(理想情况下)来自许多人的文件拼凑在一起，因此您将有大量内置的备选方案——并且您自己将有助于满足其他人的请求。*

### **如何使用 BitTorrent 找到并下载文件**

现在你已经对 BitTorrent 背后的术语和过程有了更好的了解，让我们开始使用它吧。

#### **首先，你需要下载一个 BitTorrent 客户端**

没有 BitTorrent 客户端，您无法参与对等协议。有许多 BitTorrent 客户端可供选择— [*许多*](https://en.wikipedia.org/wiki/Comparison_of_BitTorrent_clients) 。我们最喜欢的包括:

*   [**qBitTorrent**](https://www.qbittorrent.org/)—Windows/Mac(uTorrent 的开源免费变种)

*   [**大洪**](https://deluge-torrent.org/)**—Windows/Mac(同样开源，同样免费，并且支持 [大量插件](https://dev.deluge-torrent.org/wiki/Plugins) 用于定制其操作)** 
*   **[**传输**](https://transmissionbt.com/)——主要针对 Mac，但也有“早期预览”的 Windows 版本。(非常受欢迎的客户端，而且非常容易使用。)** 
*   **[**Tixati**](https://www.tixati.com/)—Windows(简单*和* [skinnable](https://github.com/theLMGN/matches) ！)**

**为了使用 BitTorrent 应用程序下载任何东西，你首先必须找到并下载一个. Torrent 文件，然后用你的 BitTorrent 客户端打开它。种子文件**不包含您的文件**。相反，它包含的信息告诉您的 BitTorrent 客户端在哪里可以找到也在共享和下载文件的对等方。** 

**正如 BitTorrent 博客 所描述的:**

> ***“内甲”。torrent”文件是一组帮助您的 BitTorrent 客户端查找和下载数据的信息。这些信息是一组文件，包括名称、大小和文件夹结构。以及关于文件的信息。torrent '文件还包含一个追踪器列表。***
> 
> **追踪器可以被认为是一台或一组帮助识别特定数据位置的计算机。当对内容的请求发出时，比如说 FADER 101 捆绑包的最新一期，跟踪器可以帮助将寻找它的人连接到可以找到它的位置。"**

**你可以*也可以*使用所谓的 [磁铁链接](https://lifehacker.com/what-are-magnet-links-and-how-do-i-use-them-to-downloa-5875899) ”来启动 BitTorrent 下载。这里的区别是你不是直接从服务器上下载一个. torrent 文件；相反，磁铁链接包含所有你需要找到的信息。来自其他 BitTorrent 对等方的 torrent 文件。这是一种去中心化的方法，让你不必下载一个. torrent 文件就可以开始(并且只要求网站发布吸引人的链接，而不是托管，这也帮助了网站。种子文件本身)。**

**正如 [比特评论维基](http://wiki.bitcomet.com/peers_seeds_torrent_tracker_dht_peer_exchange_pex_magnet_links) 所描述的:**

> ***“[磁铁链接]可以减少种子索引网站的负载，也可能提供一个更好的机会保持种子活着，因为一旦。torrent 文件在 DHT 网络上，理论上它不再需要在网站上下载；你所需要的只是一个磁铁链接。如果原始网站关闭或不再提供种子，链接更有可能在互联网上传播。torrent 文件托管在备用站点上以供下载。***

#### **你在哪里找到种子？**

**这就是我们进入道德灰色地带的地方。让我们现实一分钟:大多数人使用 BitTorrent 下载版权材料。无论我们多么自欺欺人地说我们都在下载 Linux 发行版和 [屏保](https://electricsheep.org/) ，盗版和 BitTorrent [携手并进](https://www.wired.com/story/how-bittorrent-spurred-the-streaming-revolution/) 。(是的，我们很清楚还有很多其他地方可以下载非法内容:新闻组、 [文件托管网站，如 Mega](https://lifehacker.com/google-one-is-now-open-for-everyone-but-is-it-a-good-d-1826049257) 等等。)**

**无论你在寻找什么内容，我们建议不要采用“谷歌搜索它的名字加上‘BitTorrent’这个词”的方法，除非你真的想找像 [这样的普通 Linux 发行版](https://distrowatch.com/dwres.php?resource=bittorrent) 。如果你试图免费获取你最喜欢的电视节目的最新一集，你会发现一个*吨*的列表——以及许多垃圾网站试图利用你对免费内容的兴趣。你最终可能会以 BitTorrenting 一个你一点也不期望的文件而告终。或者更糟，恶意软件。**

**找到列出你可能感兴趣的各种种子的伟大网站并不困难。也不难找到列出这些种网站 的网站 [。无论你喜欢 BitTorrent，我建议你小心对待。如果你只是在这个广阔的下载世界中迈出第一步，坚持使用社区中那些人的推荐，他们可能比你更了解什么是合法的(什么是非法的)。](https://www.reddit.com/r/trackers/)**

#### ****下载种子****

**当你通过 BitTorrent 找到一个要下载的特定项目时，你会想要检查一个统计数据:它有多少种子，或者有多少其他人有你想要下载的任何内容的完整副本。如果这个数字为零，不要放弃希望；让你的种子流运行一段时间(一天，一周，无论什么)，你可能会运气好，让一些种子加入进来。根据你想买的东西的年龄和总体受欢迎程度，你也可能会手头拮据。当有疑问时，瞄准有很多种子的种子。**

**你所要做的就是下载并运行一个. Torrent 文件，或者点击一个磁铁链接——如果后者不起作用，你可以手动导入它，然后将你的 BitTorrent 客户端设置为默认应用程序，以处理这些类型的链接。**

**很简单，对吧？但是，在开始 BitTorrent 冒险时，您需要记住一些额外的因素:**

*   **您使用了多少带宽？每个 BitTorrent 客户端，即使是半好的，也应该有一些方法来限制你的下载和上传速度。如果你在工作时间与他人分享你的网络连接，或者你不希望你的文件分享影响你的其他活动，设置合理的限制是至关重要的。你可能想限制你的上传速度超过你的下载速度；虽然这使你成为一个混蛋，但从分享的角度来看，你的 ISP 可能支持比下载速度低得多的上传速度。

    如果你支付的是“150Mbps 互联网”， [例如](https://www.cabletv.com/xfinity/internet) ，这实际上意味着你的上传上限仅为 5Mbps 而不是 150Mbps。通过将零碎的文件扔给急切的 BitTorrent 客户端来填充管道，这样就不会有任何空间留给你其他需要带宽的活动了。**
*   **你应该使用 VPN 吗？如果你下载的所有东西都是合法的，那就没问题。如果你下载的东西可能会惹恼版权所有者，如果你没有使用 VPN 来隐藏你的所作所为，你只会要求你的 ISP 给你一封措辞严厉的信——或者更糟。不要使用免费的 VPN。花钱买 [一个很棒的 VPN](https://lifehacker.com/how-to-choose-a-vpn-1831320407) ，它会隐藏你正在做的任何事情。**
*   **你播种了多久？虽然你保持一个很高的 BitTorrent 比率(你下载的数量与你上传给别人的数量之比)是高尚和伟大的，但回想一下第一点。如果您一直在播种文件，您可能会影响自己的网络性能。考虑一下你*是否真的*想让你的 BitTorrent 客户端在你启动 Windows 时启动(并开始自动播种你下载的任何东西)。否则，想想你觉得舒服的时间长度。当你下载的种子达到那个点时，从你的 BitTorrent 客户端删除它。如果你不再需要你下载的东西，不要忘记把它从你的硬盘上删除。(自定义客户端下载种子的位置可以让您更容易记住这一步。)**

**这篇文章最初发表于 2007 年 8 月 3 日，并于 2019 年 7 月 11 日更新，以提供更全面的最新信息。**