# 阻止一些网站上的 JavaScript，以防止恼人的电子邮件跟踪

> 原文:[https://life hacker . com/block-JavaScript-in-your-browser-to-prevent-noised-em-1843186321](https://lifehacker.com/block-javascript-in-your-browser-to-prevent-annoying-em-1843186321)

JavaScript 是大多数网站和网络应用在 上运行的关键元素之一，但也是最容易被利用的元素之一。它不仅用在 [分析工具、广告、浏览跟踪器](https://lifehacker.com/the-best-browsers-for-ad-blocking-that-arent-chrome-1835130559) 中，黑客还经常使用 JavaScript[部署恶意软件](https://lifehacker.com/how-to-avoid-the-new-astaroth-malware-thats-hitting-win-1842509944) ，它让你 [在某些情况下很容易被跟踪](https://lifehacker.com/dont-use-tor-right-now-if-youre-working-from-home-1842318515) ，它甚至可以意外泄露重要数据。

Watch

事实上， [最近的一项研究发现](https://medium.com/@thezedwards/the-2020-url-querystring-data-leaks-millions-of-user-emails-leaking-from-popular-websites-to-39a09d2303d2) 仅在 2020 年，运行 JavaScript 的热门网站就向广告商和其他分析公司泄露了超过一百万封用户电子邮件。这些网站包括华盛顿邮报、Mailchimp、Wish，甚至最近推出的视频流媒体服务 [Quibi](https://lifehacker.com/everything-you-need-to-know-about-quibi-1842710665) 。更糟糕的是，许多网站都是在不知情的情况下这样做的，甚至破坏了他们原本应该保护用户数据安全的其他安全措施。

### 你应该在浏览器中禁用 JavaScript 吗？

你可能不需要。一些浏览器和隐私插件会在默认情况下直接阻止 JavaScript 运行，而大多数其他现代浏览器都包含应用户请求限制或阻止 JavaScript 的选项。

虽然完全禁用所有 JavaScript 理论上可以防止依赖 JavaScript 的数据泄露和潜在的恶意软件攻击，但这也将使许多网站更难使用，甚至完全阻止它们加载，例如谷歌地图。

幸运的是，这里有一个折中的方法，即手动允许 JavaScript 只在某些网站上运行，并在您不确定时阻止 JavaScript 运行。

### 如何更改浏览器的 JavaScript 设置

并非所有的浏览器都包含相同的 JavaScript 设置，因此您可用的确切选项会因您使用的浏览器而异。

有些 [注重隐私的浏览器](https://lifehacker.com/the-best-privacy-and-security-focused-web-browsers-1672758270) ，像 Brave，在加载新页面时会问你是否要运行 JavaScript，而 Tor 默认屏蔽所有 JavaScript，没有例外。

然而，对于大多数其他浏览器，您需要手动更改 JavaScript 设置。

### **铬合金**

1.  打开网址`chrome://settings/content/javascript`
2.  取消选择**“允许”**开关以阻止所有 JavaScript。
3.  您可以将网站添加到阻止/允许列表，以创建当前设置的例外。
4.  退出并重启 Chrome。

### **边缘**

1.  使用地址栏转到`edge://settings/content/javascript`
2.  禁用**“允许”**切换以阻止所有 Javascript
3.  然后，您可以将特定网站添加到阻止/允许列表中，以创建当前设置的例外。
4.  您需要重新启动 Edge 以使设置生效。

### **火狐**

1.  在 Firefox 中，转到`about:config`
2.  如果您收到警告消息，称这可能会使您的保修无效，请忽略它，然后单击**“我接受风险”**继续。
3.  使用搜索栏查找 `javascript.enabled`
4.  双击 *javascript.enabled* 使其列为**【禁用】**关闭所有 javascript。
5.  重启火狐浏览器。

如果你不想完全禁用 JavaScript，你可以使用 Firefox 插件，比如 [禁用 JavaScript](https://addons.mozilla.org/en-US/firefox/addon/disable-javascript/?src=search) 来允许/阻止特定网站加载。

### 歌剧

1.  使用地址栏打开`opera://settings/content/javascript`
2.  关闭**“允许”**以禁用所有网站的 JavaScript。
3.  可以将网站添加到阻止/允许列表中，以创建当前设置的例外。
4.  关闭并重新启动 Opera 以使更改生效。

### **狩猎之旅**

1.  打开 Safari
2.  转到**首选项>安全**
3.  取消选中**“启用 JavaScript”**
4.  关闭菜单，然后重新启动 Safari。

### Vivaldi

Vivaldi 没有专门的 JavaScript 设置，它只允许你在每页的基础上阻止 JavaScript。

1.  点击地址栏左侧的挂锁**“站点信息”**图标，然后点击**“站点设置”**
2.  向下滚动直到找到**“JavaScript”**选项，然后从右边的下拉菜单中选择**“阻止”**。根据需要，对每个想要阻止 JavaScript 的站点重复上述步骤。