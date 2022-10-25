# 已经在您的无线路由器上禁用 UPnP

> 原文：<https://lifehacker.com/disable-upnp-on-your-wireless-router-already-1844012366>

如果你有很多设备的话，在路由器上转发端口以便设备可以与外界通话可能会令人头疼，所以像 UPnP 这样的技术听起来如此方便是有道理的。这个自动过程假设当内部程序请求访问时，将您的网络暴露给互联网是安全的——这通常是正确的，除非是一个恶意软件发出请求。

Watch

看到问题了吗？一般来说，攻击者会找到创造性的方法来利用过度信任的 UPnP 协议来执行各种有趣的操作，包括对您的网络进行端口扫描以寻找其他攻击媒介。

没有真正的理由让你运行 UPnP。这种便利不值得你为网络安全冒险。如果一个应用程序不工作，就像你最喜欢的 BitTorrent 下载工具， [转发 po rts](https://help.bittorrent.com/support/solutions/articles/29000033439-optimizing-your-internet-connection-connection-guide-) 并不是一个困难的过程。烦人，当然，但是比依赖 UPnP 安全多了。

如果你需要更多的说服力， [Ars Technica](https://arstechnica.com/information-technology/2020/06/upnp-flaw-exposes-millions-of-network-devices-to-attacks-over-the-internet/) 对一种全新的概念验证攻击进行了健康的报道，这种攻击利用 UPnP 中的另一个漏洞，在易受影响的设备之外创建了一个巨大的分布式拒绝服务(DDoS)网络。好玩！

丹·古丁写道:

> 该漏洞通过滥用 UPnP 订阅功能来工作，当某些事件发生时，例如播放视频或音乐曲目，设备使用该功能从其他设备接收通知。具体来说，CallStranger 发送伪造 URL 的订阅请求来接收结果“回调”。"
> 
> 为了执行 DDoSes，CallStranger 发送了一系列假冒互联网上第三方网站地址的订阅请求。当攻击与其他设备一起执行时，冗长的回调会用垃圾流量的洪流轰炸网站。在其他情况下，接收回调的 URL 指向内部网络中的设备。这些响应可以创建一个类似于服务器端请求伪造的条件，这使得攻击者能够攻击网络防火墙后面的内部设备。"

### 所以，已经禁用了 UPnP

确保你的网络不参与僵尸网络的最简单的方法是在你的路由器上禁用 UPnP。这很容易做到，但是这个选项——如果有的话——很可能被隐藏在一个高级设置菜单下。例如，在典型的 TP-Link Archer A20 上，您会发现它位于:**高级> NAT 转发> UPnP** 。如果你以前对路由器配置有所了解，这是有意义的，但可能不是普通用户首先会考虑的地方。

即使是在像 Google Nest Wifi 这样更友好的路由器上，你也必须挖掘一点才能找到 UPnP 设置(再次通过 Nest Wifi 的高级设置):

从好的方面来说，如果网络中的任何硬件或软件需要端口发挥作用，您现在还将知道在路由器上向哪里转发端口。通常，路由器的 UPnP 设置位于其端口转发设置的附近，设置端口转发所需要的只是您要转发的设备的 IP 地址*到*，以及所需的端口范围。( [很容易](https://lifehacker.com/know-your-network-lesson-4-access-your-home-computers-5831841) 算出来！)

一旦你做了调整，如果有的话，使用一些在线工具来检查你的网络的安全性是值得的。我推荐在 ShieldsUp 试试“ [”即时 UPnP 曝光测试](https://www.grc.com/default.htm) ！！，以及 F-Secure 的 [路由器检查器](https://www.f-secure.com/en/home/free-tools/router-checker) ，看看你的网络是否向世界开放了比它应该开放的更多的端口。