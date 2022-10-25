# 如何用 Mozilla 的免费火狐“VPN”保护你的浏览

> 原文：<https://lifehacker.com/how-to-secure-your-browsing-with-mozillas-free-firefox-1838062102>

毫无疑问，在我看来，Mozilla 正在努力——非常努力地——寻找 Firefox 网络浏览器未来的各种盈利方式。我仍然很高兴该公司决定提供免费的 VPN 服务(实际上是一个 [网络代理](https://news.ycombinator.com/item?id=20928445) 而不是其他任何东西)，给你一个简单的方法“屏蔽你的 IP 地址，防止网络上的第三方追踪者，”正如 Mozilla [所说](https://blog.mozilla.org/blog/2019/09/10/firefoxs-test-pilot-program-returns-with-firefox-private-network-beta/) 。

Watch

同样值得注意的是，Mozilla VPN 的诞生(该公司的第二个产品，尽管它是第一个免费的)也复活了该公司的测试试点计划，该计划之前负责许多有用的附加软件和体验: [标签休眠](https://lifehacker.com/test-out-firefoxs-new-tab-snoozing-feature-with-its-tes-1792714295) 、 [侧视图和 Firefox 颜色](https://lifehacker.com/how-to-get-firefoxs-new-side-view-and-color-changing-fe-1826616996) 、 [注释](https://lifehacker.com/sync-your-to-do-list-across-firefox-browsers-and-androi-1827513237) 和 [锁箱](https://lifehacker.com/the-ios-lockbox-app-lets-firefox-users-pull-up-their-pa-1827494462)

Mozilla 的“VPN”很容易上手。拉起你的火狐浏览器，访问 [这个页面](https://private-network.firefox.com) ，会提示你安装火狐专网扩展。安装完成后，您需要登录您的 Mozilla 帐户才能使用它，如果您还没有 Mozilla 帐户，也可以创建一个。这将激活浏览器角落里的一个小图标，你可以随时点击这个图标点击“VPN”。

我喜欢 Mozilla 服务的一点是，它似乎不会以任何方式降低你的浏览性能。不管我的“私人网络”是开着还是关着，我都有很好的[【fast.com】](https://fast.com)结果——没有任何减速报告。虽然该服务保护你的*实际* IP 地址的身份，但它将 Cloudflare 用作中间人服务，这意味着你很可能会连接到离你住处不远的 Warp 服务器。正如一位 [评论者](https://news.ycombinator.com/item?id=20935147) 所描述的(我自己也验证了):

> *...我刚刚测试了 Firefox 扩展，CF-Connecting-IP 和 X-Forwarded-For 都设置为 Cloudflare IP 地址，所以用户的 IP 地址是隐藏的。CF-IPCountry 包含 Cloudflare IP 地址的位置。*

> *这些请求似乎是通过最近的 Cloudflare 数据中心[1]路由的，因此该服务可能会通过这些代理 IP 地址泄露用户的粗略位置。”*

你将无法选择使用哪个服务器来假装你在不同的国家浏览网页——对你来说没有绕过网飞的限制——但至少当你在公共 wifi 连接上浏览网页时，火狐“VPN”仍然是一个有用的工具。如果你将这一点与火狐的 [新功能](https://lifehacker.com/how-to-enable-firefoxs-more-secure-dns-over-https-featu-1837986733) (仍在测试中)结合起来，你将坐在一座相当高的隐私山上。我建议两者都尝试一下，如果没有别的原因，仅仅是因为它们很容易设置，可以给你带来可观的收益。

不，中介 Cloudflare 并没有因此而收集您的数据。正如 [公司对](https://www.cloudflare.com/mozilla/firefox-private-network-privacy-notice/) 的描述:

> *“当请求发送到 Cloudflare 代理时，Cloudflare 将观察您的 IP 地址(称为源 IP 地址)、您正在访问的互联网属性的 IP 地址(称为目的 IP 地址)、源端口、目的端口、时间戳和 Mozilla 提供的表示您是 Firefox 专用网络用户的令牌(统称为“代理数据”)。所有代理数据将在 24 小时内删除。”*

> *...此外，根据 Mozilla 的指示，Cloudflare 不得使用其处理的任何数据，除非是为了提高服务的性能以及在出现问题时协助调试。”*