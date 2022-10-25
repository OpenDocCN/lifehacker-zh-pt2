# Safari 现在是阻止第三方追踪的最佳浏览器

> 原文：<https://lifehacker.com/safari-is-now-the-best-browser-for-blocking-third-party-1842489581>

昨天发布的 Safari 13.1 引入了更严格的第三方 cookie 阻止功能，防止网站识别 Safari 用户并跟踪他们的网络活动。这意味着 [苹果的默认网络浏览器](https://www.apple.com/safari/) 现在是阻止第三方追踪器的最佳选择，也是第一个彻底阻止第三方 cookies 的浏览器——击败了 Chrome。

Watch

你可以在 [最新的 WebKit 开发者博客](https://webkit.org/blog/10218/full-third-party-cookie-blocking-and-more/) 中读到这些变化，但这篇文章是为 web 开发者写的，比你可能需要的技术含量高一点。以下是重要的一点:Safari 的 ITP(智能跟踪预防)现在默认情况下会阻止所有第三方 cookies。ITP 在 2017 年推出时允许一些例外，但网站能够利用这些例外根据被阻止的内容来识别用户，并跟踪他们的活动。这些例外还使得根据用户当前在其他地方登录的其他网站来对用户进行指纹识别成为可能，即使他们启用了 Safari 最严格的隐私设置。

现在，ITP 将阻止所有第三方跟踪和禁用这些变通办法。虽然仍会存储一些信息，但网站访问您的 cookie 存储的方式已经改变，任何可写脚本存储的数据将在七天后自动删除。

对于 Safari 用户来说，这些都是重要的变化和好消息，希望更多的公司会跟随苹果的脚步。谷歌表示，它将在 2022 年前在 Chrome 上推出类似的变化，但其他浏览器，如 [【勇敢】](https://lifehacker.com/get-paid-to-watch-ads-in-the-brave-web-browser-1834332279) 和 Tor，尽管在用户匿名方面拥有 [的出色声誉](https://lifehacker.com/the-best-privacy-and-security-focused-web-browsers-1672758270) ，但仍允许某些 cookie 例外。

公平地说，大多数浏览器[都可以通过](https://lifehacker.com/the-best-browsers-for-ad-blocking-that-arent-chrome-1835130559) [扩展](https://lifehacker.com/how-to-make-ublock-origin-even-better-at-ad-blocking-in-1839964889)[高级设置](https://lifehacker.com/how-to-enable-dns-over-https-in-your-web-browser-1841909057) ，以及其他软件 [如 VPN](https://lifehacker.com/how-to-find-a-trustworthy-vpn-1833045522)来增强安全性，但说到开箱即用的跟踪设置，Safari 似乎是浏览器的最佳选择(目前)。