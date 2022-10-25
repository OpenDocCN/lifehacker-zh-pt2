# 我无法加载 Gmail，这快把我逼疯了

> 原文:[https://life hacker . com/I-cant-get-Gmail-to-load-and-its-driving-me-crazy-1834641808](https://lifehacker.com/i-cant-get-gmail-to-load-and-its-driving-me-crazy-1834641808)

当老板说“我有问题”时，我的耳朵会竖起来。Lifehacker 没问题；我们还没有被 [帕姆](https://skillet.lifehacker.com/throw-out-old-canisters-of-pam-immediately-1834614281) 炸飞。然而， [梅丽莎](https://lifehacker.com/im-melissa-kirsch-lifehacker-editor-in-chief-and-this-1829150849) 无论怎么努力都无法加载她的 Gmail 这个问题已经困扰她几个月了。这是一个让我“嗯嗯”的怪癖，因为我从来没有加载 Gmail 的问题。

Watch

梅丽莎没有给我写电子邮件，但为了保持读者提问的传统，在 Lifehacker 的技术建议专栏 中，以下是她在我们的一个 Slack 频道中对我说的一些话:

> “这对我来说是个现实问题。除了 Gmail，我在任何网站上都没有问题，而且这种情况已经持续了几个月。我谷歌了好几次，都没找到什么好的信息。”

别担心，梅丽莎。我有一些想法。本专栏的其余部分将带我们进行一次故障排除之旅。对于为什么 Gmail——只有 Gmail——没有真正为你工作，我没有任何具体的建议。然而，在这种情况下，我会使用一些技巧来找出问题的根源。

### 尝试新的浏览器

你没有提到你用的是什么浏览器。(我可以问，但我会把你的懈怠信息当作普通读者在[Tech 911 mailback](mailto:david.murphy@lifehacker.com?subject=Tech%20911)中提出的问题。)所以，我的第一个故障诊断步骤将是加载一个不同的浏览器，如 Chrome、Firefox、Edge、Safari，甚至是最近使用起来很有趣的基于 Chromium 的 Edge。如果备份浏览器能让你完美访问 Gmail，那太好了！我们正在缩小范围。

### 检查有问题的“有用”应用程序

如果无论你用什么浏览器都无法访问 Gmail，那么系统层面的问题可能是原因。这可能是你的操作系统出了问题(也许是你的 [主机文件](https://en.wikipedia.org/wiki/Hosts_(file)) )，也可能是你安装的某个应用程序出于某种原因限制了你的访问。你可能会知道你最近是否安装了任何一种新的反病毒或反恶意软件工具。如果是这样的话，考虑检查一下那个邮箱的设置，看看你能不能把 Gmail 加入白名单；至少，尝试禁用它(暂时！)看看这是否能解决您的问题。如果不是，你的问题可能不是应用程序的错。

如果你最近没有安装任何类似的应用程序，你还是应该浏览一下你电脑上的应用程序，看看是否有你可能不知道的类似应用程序在运行。同样的交易；看看你能把什么列入白名单，并考虑暂时禁用应用程序，看看你的问题是否得到解决。如果是这样，如果你不知道如何让 Gmail 与你目前使用的应用程序兼容，考虑寻找一个新的防病毒或反恶意软件应用程序。

### 重置所有的东西

我尝试的其他步骤包括重置电缆或 DSL 调制解调器，以及路由器(如果单独的话)。虽然我怀疑你的路由器设置发生了变化，导致 Gmail 无法加载，但这是值得考虑的。确保您的路由器更新到最新的固件版本，如果这不能解决任何问题，请考虑从头开始——将设备重置为出厂默认设置，并再次设置您的 wifi。这应该不会花很长时间，而且这将确保一些随机选项不会意外地以某种方式弄乱 Gmail。(我怀疑是这样，但是*故障排除就是*故障排除。)

### 停止使用您的 ISP 的 DNS

你可能还想考虑把你的域名系统换成其他的，因为我假设你还没有使用第三方服务，比如谷歌域名系统 或者 1.1.1.1[。一旦](https://1.1.1.1/) [你在你的电脑上设置了](https://lifehacker.com/how-to-browse-faster-and-more-securely-with-cloudflar-1824256064) ，确保通过在 Windows 命令提示符下键入“ipconfig -flushdns”或 [你正在使用的 macOS 版本的众多命令](https://help.dreamhost.com/hc/en-us/articles/214981288-Flushing-your-DNS-cache-in-Mac-OS-X-and-Linux) 中的一个来清除你的 DNS 缓存。

(您也可以 [配置您的路由器](https://lifehacker.com/how-to-make-your-wifi-router-as-secure-as-possible-1827695547) 使用这些 DNS 服务之一。这是一个稍微复杂一点的过程，但是这将迫使所有连接到它的东西使用更好的 DNS。)

### 如果是你的浏览器有问题怎么办？

让我们从头开始。如果你的备份浏览器加载了你的普通浏览器不能加载的网站，确保你运行的是后者的最新版本(你通常可以通过访问它的“关于”页面来检查，通常是埋在它的帮助菜单 下的 [)。然而，我打赌你的某个扩展把一切都搞砸了。](https://support.mozilla.org/en-US/kb/find-what-version-firefox-you-are-using)

很有可能是某种隐私主题的扩展。仔细检查你使用的所有东西，你应该知道它们是什么，看看你是否能以任何方式将 Gmail 列入白名单。(我经常发现 uBlock Origin 虽然很棒，但在我经常访问的一些网站上，它会把体验搞得一团糟。)如果你不知所措，你还可以进入浏览器的扩展管理器，禁用所有功能。看看是否能加载 Gmail。如果是这样，慢慢地开始一个接一个地启用扩展，在每个扩展之间加载 Gmail，看看哪个负责。

你也可以尝试清除浏览器的缓存和 cookies，看看是否能解决问题。Gmail 和 cookies 也可能存在某种一般性问题，所以进入你的浏览器设置( [，就像这个](https://support.google.com/chrome/answer/95647?co=GENIE.Platform%3DDesktop&hl=en) )，确保你没有意外屏蔽 mail.google.com 的 cookies(或其他任何 Google-y)。为了安全起见，将 mail.google.com 和 www.google.com 列入白名单，看看这能否解决问题。

如果这一切都有点棘手，你可以简单地将你的浏览器重置为默认设置，这也应该可以修复你不小心阻止 Gmail 加载的任何事情。如果你在火狐浏览器上，考虑一下 [也刷新浏览器](https://support.mozilla.org/en-US/kb/refresh-firefox-reset-add-ons-and-settings)——也许你的个人资料有问题。

### 也许其他人也有问题

虽然这不会对你的特殊情况有所帮助，但我敢打赌，我也会推荐给所有人或者只有我 设置书签 [，这是一个很好的工具，你可以用它来确认一个网站是否真的*关闭了*，或者，嗯，问题都在你的肩上。](https://downforeveryoneorjustme.com/)

### 实在不行的话(还可以…)...

我不会推荐它作为一个长期的解决方案，但是在你解决问题的时候， [HTML Gmail](https://mail.google.com/mail/?ui=html) 至少可以让你访问你的收件箱。当然，你也可以将你的 Gmail 与第三方应用[整合；你在谷歌用户界面上失去的，你将会得到...能够发送信息。](https://lifehacker.com/try-mailspring-if-youre-tired-of-terrible-desktop-email-1826216206)

不过，我想这就是我的清单了。希望这些解决方案中的一个能让你回到 Gmail。如果没有，请告诉我！如果你正在阅读这个专栏，并且对我遗漏的内容有很好的想法，请在评论中告诉我！我会转达这些建议。

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>

<small></small>