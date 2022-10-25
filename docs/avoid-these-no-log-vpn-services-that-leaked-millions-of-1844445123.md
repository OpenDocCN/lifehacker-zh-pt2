# 避免这些泄露数百万用户数据的“无日志”VPN 服务

> 原文:[https://life hacker . com/avoid-these-no-log-VPN-services-that-leaved-millions-of-1844445123](https://lifehacker.com/avoid-these-no-log-vpn-services-that-leaked-millions-of-1844445123)

我希望我们不需要 VPN，但它们可能是平衡数据安全早餐的必要组成部分。互联网服务提供商、政府、广告商甚至个人 都渴望知道你在网上做什么，他们可以找到方法轻松跟踪你的浏览数据。VPN 通过代理服务器使你的连接变得模糊，从而使这变得更加困难(但并非不可能)。他们不能对所有人隐藏你，但他们是一个有价值的隐私工具——只要他们不是泄露你数据的人。

Watch

网络安全公司 Comparitech [报道](https://www.comparitech.com/blog/vpn-privacy/ufo-vpn-data-exposure/) 由于安全性差，UFO VPN 的用户信息数据库每天都在泄露数据。该公司于 7 月 1 日向 UFO VPN 报告了这一泄漏事件。Comparitech 表示，该数据库包含:

> *   Account password
> *   VPN session secret and token
> *   IP addresses of users and VPN servers to which they are connected
> *   Connection timestamp
> *   Geographical label
> *   And device and operating system features.
> *   Looks like the URL of the domain from which the advertisement is injected into the web browser of the free user.

这些数据大部分存储在容易阅读的明文文件中，然而数据库没有被保护或加密。它甚至不需要密码就能进入。受影响的账户数量未知，但有可能*所有* UFO VPN 用户至少有部分数据被泄露；该数据库每天暴露超过 2000 万个用户日志。更糟糕的是，UFO VPN 与许多其他统称为 Android VPN 的应用程序共享相同的 [代码库和设置](https://www.androidpolice.com/2020/07/19/flash-vpn-ufo-vpn-and-five-other-services-leaked-1-2tb-of-private-information/)——一些应用程序拥有多达一百万个独立安装。Android Police 报告的这些附加应用包括:

*   快速虚拟专用网
*   免费 VPN
*   超级 VPN
*   Flash VPN
*   安全 VPN
*   兔子 VPN

### 如果你的信息被泄露了该怎么办

如果您使用过这些 VPN，至少要更改您的帐户信息。更新使用相同密码的任何其他帐户— [获取唯一密码](http://And seriously, stop re-using passwords.) ，并为任何服务打开双因素身份验证。使用 [我被要求检查](https://lifehacker.com/how-to-make-sure-your-passwords-havent-been-stolen-1837305758) 是否有任何进一步的危害，并在必要时更新您的密码。

我不怪任何人在这次惨败后离开 UFO VPN。这种泄露将用户置于危险之中，并破坏了对他们的信任，坦率地说[整个 VPN 市场](https://lifehacker.com/heres-another-reason-using-a-free-android-vpn-is-a-terr-1842793803) 。许多虚拟专用网做出了和 UFO 虚拟专用网一样的“无日志”承诺，现在完全有理由怀疑他们是否在说真话。比以往任何时候都更值得[花时间去寻找一个你信任的 VPN](https://lifehacker.com/how-to-find-a-trustworthy-vpn-1833045522)。

但是不要认为这意味着 VPN 是一个失败的事业。正如我前面所说的，它们是好的数据安全策略的一部分。为了尽可能实现最高级别的安全，你需要的不仅仅是一个 VPN——甚至是一个值得信赖的 VPN。

显然我们是加密密码管理器 的 [大粉丝，但是你也可以用合适的网络浏览器](https://lifehacker.com/the-five-best-password-managers-5529133) 和/或 [浏览器插件](https://lifehacker.com/how-to-make-safari-even-more-secure-with-ghosterylite-1830072506)[来增强隐私。如果你的浏览器](https://lifehacker.com/the-best-privacy-and-security-focused-web-browsers-1672758270) 或 [设备的操作系统](https://lifehacker.com/how-to-turn-on-dns-over-https-for-all-apps-in-windows-1-1843544589) 支持，你也可以通过 HTTPS 启用 [DNS，因为也有助于隐藏你的网络流量，防止外人窥视。虽然没有一个系统是万无一失的，但是一个经过深思熟虑的这些策略的组合可以让从数据泄露中恢复变得更加容易。](https://lifehacker.com/how-to-enable-dns-over-https-in-your-web-browser-1841909057)