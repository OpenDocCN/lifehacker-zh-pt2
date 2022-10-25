# 如果你在家工作，现在不要使用 Tor

> 原文:[https://life hacker . com/don-use-tor-right-now-if-you-work-from-home-1842318515](https://lifehacker.com/dont-use-tor-right-now-if-youre-working-from-home-1842318515)

随着越来越多的人呆在家里， [远程工作以避免新冠肺炎疫情](https://lifehacker.com/be-prepared-to-work-from-home-during-the-coronavirus-ou-1842088431) ，网络安全已经成为更高的优先事项。使用尊重用户隐私并保证数据安全的 web 浏览器是远程办公的必需品，但是你现在应该避免使用 Tor web 浏览器，尽管这是匿名化你的网络活动的最好方法之一。

Watch

[根据 Tor 开发团队](https://blog.torproject.org/new-release-tor-browser-906) 的说法，一个漏洞意外地允许 Javascript 在网页上运行，即使用户已经明确禁用了它或者打开了浏览器最严格的设置(通过 T5】ZDNet)。禁用和阻止 Javascript 是 Tor 的关键功能之一，但这一故障破坏了它的安全性，并使浏览器对依赖其匿名性的用户具有潜在的危险，因为公司、政府实体甚至黑客都可以使用 Javascript 来找到 IP 地址。

补丁目前正在开发中，但是还没有具体的发布时间表。与此同时，有一个潜在的“核心选项”将强制停止 Tor 中的所有 Javascript 功能。这将导致一些网站不可用，即使尝试修复后，Javascript 错误仍有可能发生，但值得考虑:

*   打开 Tor，然后在地址栏中键入`about:config`，按回车键。
*   按 CTRL+F 并搜索`javascript.enabled`
*   双击**“JavaScript . enabled”**行，将“值”列更改为**“假”**不幸的是，如果它已经被设置为“假”和/或 Javascript *在做出改变后仍然*运行，这不会解决问题。

Tor 用户也应该考虑在等待补丁时使用备用浏览器。

很少有人能比得上 Tor 的匿名级别，但 [Brave 是隐私的绝佳选择，Firefox 是紧随其后的](https://lifehacker.com/the-best-privacy-and-security-focused-web-browsers-1672758270)(Tor 和 Brave 都是基于 Firefox 构建的)。甚至维瓦尔第、Edge 和 Opera 也有它们的好处——只是如果你试图阻止广告 、数据追踪器，并保持你的身份模糊，请避免使用 Chrome。

我们还有 [寻找 VPN](https://lifehacker.com/how-to-find-a-trustworthy-vpn-1833045522) 、 [密码管理器](https://lifehacker.com/the-five-best-password-managers-5529133) 和 [反恶意软件](https://lifehacker.com/use-these-antivirus-and-anti-malware-apps-instead-of-av-1841264690) 的指南，所有这些都可以帮助您在等待冠状病毒时保护您的设备和数据安全。说到这里， [不要下载新冠肺炎追踪器应用程序](https://lifehacker.com/these-bogus-coronavirus-trackers-could-infect-your-comp-1842293731) 要当心 [利用当前全球形势的众多网络诈骗](https://lifehacker.com/how-to-avoid-coronavirus-scams-1842268661) 。