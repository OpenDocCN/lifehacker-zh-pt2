# 如何在 Mozilla 之前启用火狐更安全的 HTTPS 域名服务

> 原文：<https://lifehacker.com/how-to-enable-firefoxs-more-secure-dns-over-https-featu-1837986733>

在九月下旬的某个时候，Mozilla 将默认为所有用户启用 [火狐的 HTTPS 域名解析服务](https://blog.mozilla.org/futurereleases/2019/04/02/dns-over-https-doh-update-recent-testing-results-and-next-steps/) 。这就是为什么这很重要:DoH 通过 [隐藏 DNS 请求](https://blog.apnic.net/2018/10/12/doh-dns-over-https-explained/) 来保持你的互联网浏览隐私和安全——来自你的 ISP，来自你系统上的软件(如家长控制应用程序或其他阻止软件)，以及来自任何可能试图查出你在做什么的东西，如你政府的网络浏览审查机制。



一旦更新推出，DoH 将很快成为一小部分 Firefox 用户的默认功能，一旦确认一切正常，DoH 将会在更大范围内推出。对于那些不想等待的人来说，火狐浏览器现在也提供了功能*和*——只需要在设置菜单中做一些调整:

1.  在桌面上打开一个新的 Firefox 标签。
2.  在地址栏中键入“about:preferences#general ”,然后按 Enter 键。
3.  向下滚动到网络设置并点击**“设置”**
4.  向下滚动并勾选**“通过 HTTPS 启用 DNS”旁边的框**
5.  启用后，您可以配置 DNS 提供商设置。单击下拉框并选择**“cloud flare**”以使用默认的 DNS 提供商和设置(我们建议普通用户使用),或者选择“自定义”以手动设置您自己的服务(如果您希望使用单独的服务)。(不管怎样，Cloudflare 和 Mozilla 合作的原因之一是因为 Cloudflare 同意从 Firefox 用户那里收集尽可能少的流量数据。)

以上步骤是火狐开启 HTTPS DNS 的“简易方法”；还有一种更复杂的方法，可以让你在进行的过程中改变设置。

1.  在一个新的 Firefox 标签中，在地址栏中输入“about:config ”,然后按回车键。你会得到一个警告，说更改这些设置可能会使你的保修无效，并使 Firefox 不稳定——这两种情况都是真的——但还是接受这个警告并继续。
2.  查找**“network . TRR . mode”**，将其值设置为以下数字之一: **5:** DoH 被禁用(默认设置)； **3:** DoH 使能，常规 DNS 禁用； **2:** DoH 使能，常规 DNS 保留备用；DoH 和常规 DNS 已启用，但 Firefox 将决定每个网站使用哪个。我们建议现在使用值 2，因为它优先于 DoH，但是如果您愿意，可以随意使用其他值。
3.  接下来，进入**“network . TRR . uri”.**要使用默认的 Firefox DoH 服务，请将 URL 设置为“Mozilla . cloud flare-DNS . com/DNS-query”如果您有不同的服务，请使用它的地址。
4.  最后，找到**“network . TRR . bootstrapaddress”。**输入 DoH 的 DNS 解析器的数字 IP 地址。默认的 Cloudflare/Mozilla 地址是 1.1.1.1，但是如果你使用不同的地址，你需要找到你的特定服务的 IP 地址。
5.  重启 Firefox 以使更改生效，DoH 现在应该被启用了。