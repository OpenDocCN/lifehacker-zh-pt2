# 如何解决旧路由器的安全漏洞

> 原文：<https://lifehacker.com/how-to-address-security-bugs-in-your-old-router-1840264553>

如果一个 n 攻击者设法访问你的 D-Link 路由器的登录屏幕，并且你的路由器足够旧，他们就有可能控制路由器，给它注入代码，并用它来攻击其他连接的系统和设备。最棒的是。D-Link 完全知道这些问题，但它不打算修复受影响的路由器，因为它们太旧了。

Watch

这是无线网络世界的一个普遍问题。虽然 D-Link 为我们提供了最新的例子，但旧路由器中未打补丁的漏洞会影响任何制造商的设备。

关于 D-Link 的问题，我们通过 [ThreatPost](https://threatpost.com/d-link-wont-fix-router-bugs/150438/) 得到了提醒，该漏洞适用于以下任何一款 [D-Link 路由器](https://webcache.googleusercontent.com/search?q=cache:rJnlpjUXpSAJ:https://us.dlink.com/en/security-bulletin/dir-866-dir-655--dhp-1565-dir-652-unauthenticated-rce+&cd=2&hl=en&ct=clnk&gl=us) :

*   DIR-866
*   DIR-655

*   DIR-1565

*   DIR-652
*   磷酸二铵-1533
*   DGL-5500
*   DIR-130
*   DIR-330
*   DIR-615
*   DIR-825
*   DIR-835
*   DIR-855L
*   DIR-862

### 你的路由器易受攻击。现在怎么办？

这些公告是否足够可怕，以至于你应该打开储蓄罐，用你的假期基金去买一个新的路由器？我对此持观望态度。

如果你还在使用过时的 wireless-n 路由器，比如 D-Link 的 DIR-615，可能是时候升级到更现代的了。你可以花不到 60 美元 买到一个很棒的无线交流路由器 [，它应该会给大多数新的智能手机和笔记本电脑带来更强的无线连接。(如果你支付的网速很慢，这在你的日常生活中可能没多大关系，但至少你可以在潜在的更大范围内获得可靠的浏览体验。)](https://www.amazon.com/dp/B079JD7F7G/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-address-security-bugs-in-your-old-router-1840264553&asc_source=&linkCode=xm2&tag=kinjalifehackerlink-20)

我建议购买一个相当新的路由器，以确保其制造商在未来几年内继续支持它。为了帮助你做出明智的决定，研究制造商的报废政策，如果他们提供这些政策的话(例如 [D-Link](https://www.dlink.com/en/eol-policy) )。这一点很重要，因为你不希望因为“升级”到旧路由器而再次陷入同一条船上——处理公司不会修补的漏洞

### 但是我不想买新的路由器

如果你的旧路由器没有给你带来任何痛苦，并且你发现你的无线连接是你所需要的一切你住的地方，保持安全的最好方法是确保你使用你能找到的最新固件 [为你的路由器](https://lifehacker.com/how-to-make-your-wifi-router-as-secure-as-possible-1827695547) 。你甚至可以考虑像 [DD-WRT](https://dd-wrt.com/) 或 [OpenWrt](https://openwrt.org/) 这样的第三方固件，如果这些可以堵住你的制造商拒绝修复的任何安全漏洞的话。

你也要确保你的路由器的基于网络的管理屏幕，如果有的话，用一个强密码保护——一个你不与其他服务一起使用的密码。而且这个我怎么强调都不为过:*在你的路由器*上关闭 [*远程管理*](https://eu.dlink.com/uk/en/support/faq/routers/wireless-routers/dir-series/dir-878/how-do-i-enable-remote-management-for-my-router) *。不是所有的路由器都有这个功能，如果有的话，默认情况下也不会启用，但是你不应该使用它。*

同样，如果您的路由器使用 UPNP，允许您通过 SSH 远程访问它，或者有某种内置的 FTP 服务器，您可能也应该关闭这些服务。WPS 也是如此，还有任何一种基于云的管理。确保你的 wifi 密码使用 WPA2 加密。如果你还在使用 WEP，或者你的路由器甚至没有*提供* WPA2，是时候改变这种情况了(或者升级)。

除此之外，确保你在浏览网页时运用了常识。我怀疑你在脸书上与朋友聊天时会遇到利用路由器漏洞的代码，但也许花时间搜索粗略的网站来寻找被黑的游戏或应用程序并不是一个好主意。保持连接设备的固件、软件和病毒/恶意软件扫描更新，以防万一，但这应该是你无论如何都要做的事情，无论路由器是否易受攻击。

记住，你可以把你的旧路由器变成一个接入点 ，在你的房子里获得更好的 wifi 覆盖，所以这不像买一个新路由器意味着你的旧路由器要被扔进天上的大回收站。即使你不需要或不想建立一个二级接入点，当一个新的路由器意外死亡时，有一个备份也无妨。