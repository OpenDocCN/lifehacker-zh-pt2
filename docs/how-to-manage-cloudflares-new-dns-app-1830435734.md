# 如何管理 Cloudflare 的新 DNS 应用程序

> 原文：<https://lifehacker.com/how-to-manage-cloudflares-new-dns-app-1830435734>

[Lifehacker's Complete Guide to Android](https://androidos.kinja.com)) : title[![](../Images/e2dcc498f7314a475ad7b9879a9d5584.png)](https://androidos.kinja.com)[Lifehacker's Complete Guide to Android](https://androidos.kinja.com)Don't get overwhelmed by Android's many (many!) settings and apps. Master your Android phone or tablet with our ample collection of guides, tips, and tricks.

免费 DNS 提供商 Cloudflare 最近发布了一款全新的应用程序，用于 [**iOS**](https://itunes.apple.com/us/app/1-1-1-1-faster-internet/id1423538627?mt=8) 和[**Android**](https://play.google.com/store/apps/details?id=com.cloudflare.onedotonedotonedotone&hl=en_US)，【1.1.1】，这使得通过 [该服务的高速服务器](https://www.cloudflare.com/learning/dns/what-is-1.1.1.1/) ，而不是你的 ISP(可能更慢)服务器来路由你设备的所有 DNS 请求变得非常容易。换句话说，这会让你的网页浏览感觉更快。更好的是，Cloudflare 表示，它不会存储任何关于你正在浏览的内容的数据——这可能与你的 ISP 不同。有什么不喜欢的呢？

Watch

这款应用可以免费安装和使用，但有一个小问题。Cloudflare 首席执行官 Matthew Prince 在 [回复](https://blog.cloudflare.com/1-thing-you-can-do-to-make-your-internet-safer-and-faster/#comment-4190526220) 几天前的一篇博客评论中调侃了这个问题:

> *“不幸的是，iOS 只允许你基于每个 WiFi 网络来设置 DNS 设置。这意味着，您需要为每个 WiFi 网络设置 DNS 设置。而且，即使你这样做了，当你使用你的手机服务提供商时，它也不会覆盖你。此外，虽然 1.1.1.1 速度更快，更尊重隐私，但 iOS 默认不支持加密 DNS(无论是 TLS 上的 DNS 还是 HTTPS 上的 DNS)。支持跨所有网络的 1.1.1.1 *和*添加加密 DNS 支持的唯一方法是设置 VPN 配置文件。我们希望 iOS 和 Android 在未来都能提供更大的灵活性，但就目前而言，这是唯一可行的技术方法。注意:我们只是通过 VPN 代理 DNS 流量。非 DNS 流量不通过 VPN 路由。*

如果你还不明白，问题就在这里:通过运行 Cloudflare 应用程序，它会在你的设备上安装 VPN 配置文件，当你在旅途中时，你就失去了使用*实际* VPN 的能力。如果你一天的大部分时间都在家里或工作中使用 wifi，或者如果你正在通过手机连接浏览网页，这没什么大不了的，但如果你在星巴克消磨时间，比如说，查看你的银行账户余额，我绝对建议你使用 VPN。

我*也*认为 Cloudflare 的应用是你的 iOS 或 Android 设备的必备。(在公司推出 Cloudflare 的时候，我把我的各种设备和电脑切换到了 [Cloudflare 的高速 DNS](https://lifehacker.com/how-to-browse-faster-and-more-securely-with-cloudflar-1824256064) 。)如何最好地平衡 VPN 的安全性与新 DNS 服务的速度和隐私？你有两个选择:

### 在 Cloudflare 的应用程序和您的 VPN 之间切换

我使用 NordVPN，这意味着每当我想触发它时，我必须启动一个小的 iOS 应用程序并选择一个服务器。由于 Cloudflare 的 1.1.1.1 应用程序也是独立的软件(有一个开/关开关)，所以在需要时使用其中一个并不困难。

我可能会默认让 Cloudflare 的应用程序一直处于启用状态，并且只需记住，在启用我的实际 VPN 之前，我必须关闭它——我并不经常需要它。

### 在您的设备上手动设置 Cloudflare 的 DNS

你不需要使用 Cloudflare 的应用程序来从免费的公共 DNS 解析器中获益。如果你在 iOS 上，你必须为你想使用 Cloudflare 的 DNS 的每个 wifi 网络设置一个手动 DNS 条目——当你在蜂窝网络上浏览时，你将无法使用它。尽管如此，除了 [安全 DNS 传输](https://www.cloudflare.com/ssl/encrypted-sni/) 之外，您将在最常用的 wifi 网络上获得 Cloudflare 服务的基本优势，并且您将能够在需要额外安全的任何时候使用您单独的 VPN。

一些 Android 用户的情况稍微好一点。如果你不在 Android 9 Pie 上，你必须做和你的 iOS 同行一样的事情——修改你连接的每个 wifi 网络的 DNS 设置。

Android Pie 用户——例如 Pixels、Essentials 和一加智能手机的所有者——可以利用谷歌新的私有 DNS 功能，通过 Cloudflare 路由所有 DNS 查询(在 wifi 和蜂窝连接上)。额外的好处是，这还可以加密您的 DNS 查询，使它们保持私密，正如 Cloudflare 所描述的:

> *“这项新功能简化了在 Android 上配置自定义安全 DNS 解析器的过程，这意味着您的设备和您访问的网站之间的各方将无法窥探您的 DNS 查询，因为它们将被加密。这背后的协议，TLS，也是你在 HTTPS 访问网站时在地址栏看到的绿色锁图标的原因。同样的技术也可用于加密 DNS 查询，确保它们不会被篡改，不会被 ISP、移动运营商和您与 DNS 解析器之间的网络路径上的任何其他人所理解。这些新的安全协议被称为 HTTPS DNS 和 TLS DNS。”*

### 我可以信任 Cloudflare 吗？

当你把你的流量路由到其他地方——无论是第三方 DNS 解析器还是 VPN 服务——都不能保证另一端的公司不会监视你的所作所为。事实上，有些人已经 [批评 Cloudflare 的应用](https://www.reddit.com/r/privacy/comments/9wmjey/cloudflares_mobile_application_1111_faster_safer/) 在你的设备上存储你的 DNS 请求的临时日志。

如果这让您感到困扰，或者 Cloudflare 本身让您感到困扰，您还有很多其他选择。我推荐调查一个类似于[**DNS claok**](https://itunes.apple.com/us/app/dnscloak-dnscrypt-doh-client/id1330471557?mt=8)(iOS)、[**DNS Changer**](https://play.google.com/store/apps/details?id=com.burakgon.dnschanger)(Android)，或者*其他*[**DNS Changer**](https://play.google.com/store/apps/details?id=com.frostnerd.dnschanger)(Android)的应用，它们给你类似的功能，但是让你使用任何你想要的 DNS 服务。

(我的建议？抓住 [命名工作台](https://code.google.com/archive/p/namebench/downloads) ，看看你附近有什么速度快。如果你对这项服务感到满意，不管是 Cloudflare、Google、OpenDNS 还是其他什么，那就打开吧。)