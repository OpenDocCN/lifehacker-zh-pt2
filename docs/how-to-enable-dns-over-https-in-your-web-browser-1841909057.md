# 如何在您的网页浏览器中启用 HTTPS 域名系统

> 原文：<https://lifehacker.com/how-to-enable-dns-over-https-in-your-web-browser-1841909057>

Mozilla 已经开始为所有 Firefox 用户在 HTTPS 推出 DNS，这是一个坚实的安全变化，旨在解决第三方监视你访问的网站的问题。通常，当您在浏览器的地址栏中键入网站并按 Enter 键时，浏览器会使用 DNS 将域名映射到您尝试访问的服务器的实际 IP 地址，即托管您要访问的网站的服务器。



DNS 查询通常是不加密的，这意味着这些请求可能会“泄露”，很容易被第三方截获。这使得从黑客到广告商的每个人都可以很容易地看到你试图访问的网站，即使网站本身是加密的(HTTPS)。正如民主技术中心[所描述的](https://cdt.org/insights/dns-strengthening-the-weakest-link-in-internet-privacy/) :

> 每当你在浏览器中输入一个地址，每当你发送一封电子邮件，每当你点击一个链接，这个过程都会发生。一些网站可能包含嵌入其他域的内容，在这种情况下，页面本身可能会触发额外的 DNS 查询。因此，即使你访问的所有网站的实际内容都是加密的，DNS 解析器(以及任何监控网络的人)也能看到你每次访问的每一个网站。这个记录可以用来推断你在看什么，你在找什么样的信息，你何时以及如何使用互联网，以及其他个人信息。一些 DNS 提供商出售或使用这些信息做有针对性的广告。
> 
> 除了第三方监控和出售您的互联网使用的隐私影响之外，DNS 还存在严重的安全问题。具体来说，DNS 容易受到中间人攻击，在这种攻击中，恶意参与者(不是 DNS 服务)会拦截 DNS 查询并返回不正确的 IP 地址，从而可能将用户定向到有害的站点。这种“欺骗”攻击可以通过使用额外的验证程序来缓解，如 DNSSEC，但许多域不这样做。

启用了 HTTPS 域名解析服务后， [Mozilla 写道](https://blog.mozilla.org/blog/2020/02/25/firefox-continues-push-to-bring-dns-over-https-by-default-for-us-users/) ，你的浏览历史应该对潜在攻击者*和*公司更加隐蔽，他们正试图跟踪你在网上做什么。但是 Firefox 并不是唯一可以通过 HTTPS 处理 DNS 的浏览器。这里有一个快速浏览，看看如何在所有主流浏览器上启用 HTTPS DNS——包括 Mozilla，如果你没有耐心，不想等待推出的话。

### Mozilla Firefox

1.  点击浏览器右上角的汉堡图标，然后点击选项。
2.  向下滚动到“常规设置”部分的“网络设置”，然后单击“设置”按钮。
3.  点击“通过 HTTPS 启用 DNS”并选择一个提供商，如 CloudFlare，或在“自定义”下输入您自己的

### 谷歌浏览器

1.  复制并粘贴到你浏览器的地址栏，点击回车:*chrome://flags/# DNS-over-https*
2.  启用“安全 DNS 查找”标志并重启浏览器
3.  确保你已经 [切换了操作系统的网络设置](https://lifehacker.com/how-to-browse-faster-and-more-securely-with-cloudflar-1824256064) 。你不需要从你的 ISP 自动获得一个 DNS，你需要强迫它使用 Chrome 的 [映射表](https://www.chromium.org/developers/dns-over-https) 中的一个提供商。

### 边缘铬

1.  复制并粘贴到你浏览器的地址栏，然后点击回车:*edge://flags/# DNS-over-https*
2.  启用“安全 DNS 查找”标志并重启浏览器
3.  确保你已经 [切换了操作系统的网络设置](https://lifehacker.com/how-to-browse-faster-and-more-securely-with-cloudflar-1824256064) 。你不需要从你的 ISP 自动获得一个 DNS，你需要强迫它使用一个支持 [DNS 胜过【HTTPS】](https://github.com/curl/curl/wiki/DNS-over-HTTPS)DNS 的提供商。

### 勇敢的

1.  复制并粘贴到你浏览器的地址栏，然后点击回车:*勇敢://flags/#dns-over-https*
2.  启用“安全 DNS 查找”标志并重启浏览器
3.  确保你已经 [切换了操作系统的网络设置](https://lifehacker.com/how-to-browse-faster-and-more-securely-with-cloudflar-1824256064) 。你不需要从你的 ISP 自动获得一个 DNS，你需要强迫它使用一个支持 [DNS 胜过【HTTPS】](https://github.com/curl/curl/wiki/DNS-over-HTTPS)DNS 的提供商。

### 如何查看 HTTPS 上的 DNS 是否正常工作

只需访问 [Cloudflare 的帮助页面](https://1.1.1.1/help) ，它会运行一个快速检查来告诉你你的浏览器是否在 HTTPS 上使用 DNS:

### Safari 怎么样？

抱歉，Mac 粉丝们。苹果尚未在 Safari 中实现这一功能，但我预计该公司会在某个时候实现这一功能。注重隐私的苹果公司没有理由成为唯一一家不在其主浏览器中提供 HTTPS 域名服务的公司。