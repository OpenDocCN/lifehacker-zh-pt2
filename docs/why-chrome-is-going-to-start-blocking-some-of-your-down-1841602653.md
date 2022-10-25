# 为什么 Chrome 会开始阻止你的一些下载

> 原文：<https://lifehacker.com/why-chrome-is-going-to-start-blocking-some-of-your-down-1841602653>

当谷歌 Chrome 在几个月后开始阻止你的下载时，要知道这不是针对你个人的；浏览器只是尽力保护你的安全。你应该*也*知道 Chrome 并不是完美无缺的，你仍然应该运行定期的防病毒和反恶意软件扫描——避免劣质网站和它们的恶意软件。



明白了吗？事情是这样的。谷歌去年 10 月宣布，它正计划通过阻止 HTTP 内容在 HTTPS 网站上加载来解决 chrome 中的混合内容。正如谷歌所描述的:

> HTTPS 页面通常会遇到一个叫做混合内容的问题，即页面上的子资源通过 http://不安全地加载。默认情况下，浏览器会阻止许多类型的混合内容，如脚本和 iframes，但图像、音频和视频仍然可以加载，这威胁到了用户的隐私和安全。例如，攻击者可以篡改股票图表的混合图像来误导投资者，或者在混合资源负载中注入跟踪 cookie。加载混合内容还会导致令人困惑的浏览器安全 UX，页面既不是安全的也不是不安全的，而是介于两者之间。"

你可以用一个 [系列](https://googlesamples.github.io/web-fundamentals/fundamentals/security/prevent-mixed-content/simple-example.html) [的](https://googlesamples.github.io/web-fundamentals/fundamentals/security/prevent-mixed-content/xmlhttprequest-example.html) [演示](https://googlesamples.github.io/web-fundamentals/fundamentals/security/prevent-mixed-content/image-gallery-example.htmlhttps://googlesamples.github.io/web-fundamentals/fundamentals/security/prevent-mixed-content/passive-mixed-content.html) 网站 [谷歌创建的](https://developers.google.com/web/fundamentals/security/prevent-mixed-content/what-is-mixed-content) 来亲眼看看。然而，对你来说最明显的是 Chrome 开始警告并最终阻止来自 HTTPS 网站的不安全 HTTP 下载。警告将从 Chrome 82 开始，计划于 4 月 22 日稳定发布，阻止将从 Chrome 83 开始，包括某些类型的文件。这是来自谷歌的官方时间表:

至于浏览器的移动版本，同样的下载阻止设置也会发生，但会晚一个周期。因此，在这种情况下，Android 和 iOS 版本的 chrome 仍然开始阻止 HTTP 可执行文件在 HTTPS 网站上下载

这是否意味着你可以安全地从 HTTPS 网站下载任何内容(你可以下载的内容)？正如去年号[号](https://www.kaspersky.com/blog/https-does-not-mean-safe/20725/)号写道:

> 但是问题是绿色的锁和颁发的证书对网站本身只字未提。一个钓鱼网页可以很容易地获得一个证书，并加密你和它之间的所有流量。
> 
> 简单地说，绿色锁所能确保的就是没有人能够窥探你输入的数据。但是如果你的密码是假的，它仍然会被网站窃取。
> 
> *网络钓鱼者积极利用这一点:* [*根据网络钓鱼实验室*](https://info.phishlabs.com/blog/quarter-phishing-attacks-hosted-https-domains) *的数据，如今四分之一的网络钓鱼攻击都是在 HTTPS 网站上进行的(两年前这一比例还不到 1%)。此外，* [*超过 80%的用户相信*](https://info.phishlabs.com/blog/quarter-phishing-attacks-hosted-https-domains) *仅仅是一个小小的绿色锁和网址旁边的“安全”字样就意味着网站是安全的，他们在输入自己的数据之前不会想太多。”*

和往常一样，您仍然有责任确保您不会从粗略的地方下载粗略的东西，将它们安装在您的 PC 上，并看着攻击者夺取您的数字生活的控制权。这意味着你会希望你的浏览器有通常的保护——当然是一个坚固的 [广告拦截器](https://github.com/gorhill/uBlock) 或 [两个](https://www.eff.org/privacybadger)——并且开启谷歌的安全浏览设置:

除此之外，确保你正在运行一个可靠的防病毒程序——即使是一个 [像样的免费软件](https://lifehacker.com/why-you-should-use-windows-defenders-ransomware-prevent-1837311176) 也比没有好——并在你的系统上运行定期的 [反恶意软件扫描](https://lifehacker.com/use-these-antivirus-and-anti-malware-apps-instead-of-av-1841264690) 。如果你不确定你已经下载了一个特定的文件，在一个 [沙箱](https://lifehacker.com/how-to-safely-test-software-without-messing-up-your-sys-1680608496) 或 [虚拟机](https://lifehacker.com/how-to-set-up-a-virtual-machine-for-free-1828969527) 中运行它，这样它就不会扰乱你系统的其余部分。最重要的是，停止访问可疑网站。