# 借助 Plex 媒体服务器，在任何地方流式播放您的媒体收藏

> 原文：<https://lifehacker.com/use-a-plex-media-server-to-stream-your-media-collection-1832992483>

我们可能处于云流媒体和订阅服务的时代，但媒体所有权(包括数字和物理)仍然存在。也就是说，能够从一个地方整合和流式传输您的电影、音乐和其他媒体收藏，比在多个硬盘驱动器、设备和物理副本堆栈上拥有一个碎片化的库要方便得多。



这就是拥有 Plex 媒体服务器的便利之处。Plex 已经出现了一段时间，但如果你不熟悉，这项服务可以将任何具有足够电源和存储空间的设备转变为联网的媒体服务器，供你远程访问。您甚至可以与朋友和家人共享访问权限，创建自己的私人媒体网络。

这听起来可能是一个复杂的项目，但是如果你有合适的工具，它实际上是非常容易的。我们将本指南整合在一起，以帮助您完成主要步骤和决策。我们将重点关注媒体服务器设置的三个方面:服务器设备、媒体文件以及可用于定制您的体验的各种应用程序和附件。

### 挑选服务器设备

将作为 Plex 媒体服务器工作的设备数量惊人，但是选择适合您设想的设置的设备需要更多的考虑，而不是简单地将外部硬盘插入您的 PC 并声称它是好的。

理想情况下，您的服务器将 24/7 全天候打开并连接到您的家庭网络，因此请寻找设计为始终打开的设备/组件(下面我们将详细介绍几种)。同样，你需要考虑马力。对于那些希望将访问扩展到多个用户的人来说，你需要更强大的设备，因为更多的人访问服务器需要更多的处理能力和网络带宽。如果你计划播放 4K·UHD 和 HDR 的视频内容或高保真音频文件，这就变得尤为重要。然而，更大的功率将需要更昂贵的设备/部件，而且还需要更多的功率来运行。另一方面，你可能不希望有一个超级强大的设备作为你的服务器。

至于网络需求，我们建议您尽可能通过以太网将服务器连接到家庭网络。如果你通过 WiFi 连接，你至少需要使用 802.11n 路由器，或者最好是 802.11ac 路由器。

有关 Plex 服务器要求的更多信息，请参考 [Plex 的支持页面](https://support.plex.tv/articles/200375666-plex-media-server-requirements/) 。

#### **NAS**

网络连接存储( [NAS)在硬件方面是您最简单的选择](https://lifehacker.com/should-i-use-a-diy-pc-for-my-nas-or-buy-an-enclosure-1678991505) ，但也是最弱的。不过，较小的马力也有它的好处，因为 NASs 的功耗要求较低，可以全天候工作。如果你购买一个预制的 NAS，将会有 [最小的设置](https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599) ，尽管如果你想要对过程有更多的控制，你可以构建你自己的。代价是 DIY NAS 服务器需要更复杂的软件设置，因为它们默认没有图形用户界面，而现成的设备通常预装了软件。

#### **迷你电脑**

虽然比 NAS 更贵，但购买或构建迷你 PC 是下一个最容易的选择，并且可能是大多数人在成本、功率和易用性之间的中间“最佳点”。对于预制选项，网上有大量的 [NUC 版本](https://www.amazon.com/s?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/use-a-plex-media-server-to-stream-your-media-collection-1832992483&asc_source=&i=electronics&k=NUC&ref=nb_sb_noss&tag=kinjalifehackerlink-20) ，而那些喜欢自己构建的人可以使用 [树莓派](https://thepi.io/how-to-set-up-a-raspberry-pi-plex-server/) 来查看项目。

#### **塔式电脑**

无论你是购买一台预建的电脑还是自己建造一个强大的高端设备，这都将是最昂贵的选择，并且需要最大的功率消耗。然而，这将是最适合多用户支持和大文件转码的(如 4K 视频或高保真音频)。

你也没有*有*去造一台新的个人电脑。从技术上讲，使用你现在的电脑，甚至是你闲置的旧电脑都是可能的。请记住，服务器需要打开并连接到网络才能访问，媒体播放会占用系统资源。因此，如果您是唯一将访问文件的人，并且能够确保当您想要远程连接时电脑将会打开，我们建议您仅使用您的日常电脑。

Plex 支持 Windows、macOS 和 Linux PCs。

#### **其他设备**

由于 Plex 的媒体服务器软件可以在多种设备和操作系统上运行，因此有一些其他设备可以配置为 PMS，尽管这不是它的主要使用案例。

例如，在我们的测试中，我们使用了一台 [Nvidia Shield Pro 作为我们的服务器](https://shield.nvidia.com/blog/how-to-setup-plex-media-server) 。使用 Shield 有一些限制，但它是我们最容易使用的选择，因为 Plex 媒体服务器软件是预装在 Shield Pro 上的，其 500GBs 的内部存储可以单独容纳任何媒体库的相当大一部分。

Plex [下载页面](https://www.plex.tv/media-server-downloads/) 包含支持的操作系统和设备的完整列表。

### 挑选硬盘

服务器构建的第二部分是选择存储媒体的硬盘。上面的几个选项可以使用内置硬盘作为介质驱动器，但我们建议使用支持 USB 3.0、自带外壳和电源(如果可能)的外置 NAS 认证硬盘。

对于 1TB 的服务器，我们使用了 500GB 的外部驱动器和 Nvidia Shield Pro 的内部 500GB 存储，对于一个大型音乐收藏和十几部蓝光质量的电影来说，空间绰绰有余，但你可以轻松地将硬盘存储容量增加四到五倍。

### 设置服务器

1.  准备好您的服务器设备。如果您正在构建自己的服务器，请务必遵循上面链接的指南，该指南将带您完成所需的任何硬件组装或软件安装，并帮助您将服务器连接到网络。如果您使用的是预建的设备，请像设置任何其他 PC 一样设置它，打开它，然后按照首次使用说明进行操作。
2.  将服务器连接到家庭网络后，从 [plex 的下载页面](https://www.plex.tv/media-server-downloads/#plex-media-server) 为您的设备下载并安装 Plex 媒体服务器。如果你正在使用 Android/Android TV 设备作为你的媒体服务器，你可以从 Googlee 下载 [Plex 媒体服务器 Android 测试软件](https://play.google.com/apps/testing/com.plexapp.mediaserver.smb)
3.  如果你还没有建立 [Plex 账户](https://support.plex.tv/articles/200878643-sign-in-to-your-plex-account/) (安卓版 Plex 使用你的谷歌账户)。
4.  [在您将要访问服务器的设备上安装 Plex 应用程序。](https://www.plex.tv/media-server-downloads/#plex-app) 这是一个不同于媒体服务器软件的应用程序，你可以通过它连接到你的服务器并观看你的媒体。它可用于众多智能电视、Roku 和其他流媒体设备，以及 Windows、Mac、Linux、iOS、Android、Android TV、Xbox One、PlayStation 4 和其他各种设备。

### 传输媒体

设置好服务器后，现在是时候将您的音乐、图片、视频和任何其他媒体移动到服务器上了。如果您使用外置硬盘作为介质驱动器，并且您要移动的介质在 PC 上，只需插入硬盘并手动移动文件。您还可以使用 FTP 客户端通过 [将文件从一台设备无线移动到另一台设备。【T2](https://lifehacker.com/what-s-the-best-way-to-share-large-files-with-friends-1486810038)

如果您希望备份您的物理媒体收藏，您可以使用几乎任何桌面 CD 或 DVD 驱动器来翻录音频 CD，并且只要您的 PC 上有正确的软件和 DVD 或蓝光驱动器，您就可以翻录电影。 [MakeMKV](https://www.makemkv.com/) 是抓拍电影的绝佳选择。

其他指南可能会建议使用 BitTorrent 客户端或类似软件等应用程序来下载媒体，但如果你不小心，这可能会成为一个法律泥潭，所以在这里要聪明，礼貌，合法。遵循你所在地区的版权法，不要去盗版或非法分发内容。在下一节中，我们将指出几种合法的(在某些情况下是免费的)观看和录制内容的方法，并支持您的服务器库。

### 应用程序、附加组件和额外的丛功能

所有 Plex 用户都可以免费使用几个很酷的功能，这些功能可以扩展您的图书馆并整合其他应用程序/服务，使您的服务器成为一体化的流媒体解决方案。

#### **新闻和网络电视**

Plex 为用户提供来自各种来源的 [免费直播和精选新闻流](https://www.plex.tv/tv/news/) ，包括美国广播公司、美联社、路透社等。除了这些免费的新闻内容，Plex 还包括一个免费的由 Pitchfork 和 the New Yorker 等网站提供的流行网络系列 的 [图书馆。](https://www.plex.tv/tv/web-shows/)

#### **播客**

您可以从您的 Plex 服务器 下载、存储和 [流媒体播客，而不是使用智能手机的存储来下载播客。用户可以直接在 Plex 应用程序中搜索和订阅节目，软件会自动更新并下载最新的剧集。](https://www.plex.tv/music/podcasts/)

#### **虚拟现实模式**

如果你有一个兼容的 VR 耳机，你可以在 VR 模式下 [观看或收听你所有的媒体。](https://www.plex.tv/your-media/virtual-reality/)

#### **Plex Pass 和免费 OTA 电视**

Plex 的基本服务器功能是免费的，但该服务提供了高级 Plex Pass 会员资格，增加了大量的额外待遇，如指标跟踪和带宽统计，更好的文件元数据匹配，以及潮汐音乐订阅折扣等额外待遇。幸运的是，与其他媒体服务相比，Plex Pass 订阅非常实惠，并提供灵活的三种价格选择:每月 4.99 美元，每年 39.99 美元，或一次性购买 119.99 美元，终身访问。([)Plex 还提供 30 天免费试用，如果你好奇的话](https://www.plex.tv/ad/facebook-free-trial-plex-pass/) )。

Plex Pass 用户还可以使用高清 OTA 天线从大气中抓取免费的高清电视信号。你甚至可以在节目播出时录制节目。Plex 的界面甚至会自动填充节目信息以创建指南/时间表。我们使用一个 [Mohu ReLeaf](https://www.amazon.com/Mohu-Paper-thin-Reversible-Performance-MH-110599/dp/B00HSMK59E/ref=sr_1_1_sspa?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/use-a-plex-media-server-to-stream-your-media-collection-1832992483&asc_source=&crid=SJ4XF3I022NF&keywords=mohu releaf&psc=1&qid=1551464454&s=electronics&sprefix=MoHu relea,electronics,220&sr=1-1-spons&tag=kinjalifehackerlink-20) 和一个 [HD Home Run](https://www.amazon.com/SiliconDust-HDHomeRun-Connect-HDHR5-4US-Reusable/dp/B07B86FZ4R/ref=sr_1_3?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/use-a-plex-media-server-to-stream-your-media-collection-1832992483&asc_source=&crid=PK4C35MNYMD9&keywords=hdhomerun quatro&qid=1551464404&s=electronics&sprefix=HD home,electronics,208&sr=1-3&tag=kinjalifehackerlink-20) 在我们的 Plex 服务器上创建了一个临时的多用户电视服务，不需要有线电视或网络电视服务。

你不会获得频道的广度、点播内容或有线电视或 OTT 直播电视服务(如 Sling TV)的额外功能，但本地频道、体育节目，甚至少数有线频道可能会在你所在的地区提供。你可以使用这个方便的 [在线工具](https://nocable.org/hd-antenna-coverage-map) 来查看有哪些频道。