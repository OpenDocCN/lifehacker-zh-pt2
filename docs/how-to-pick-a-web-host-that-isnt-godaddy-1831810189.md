# 如何挑选一个不是 GoDaddy 的虚拟主机

> 原文:[https://life hacker . com/how-to-pick-a-web-host-that-not-godaddy-1831810189](https://lifehacker.com/how-to-pick-a-web-host-that-isnt-godaddy-1831810189)

我不确定有多少人喜欢 GoDaddy，但有很多人仍然使用 web 注册器和主机，因为他们不知道任何更好的东西。我不能指责他们。我非常确定我用 GoDaddy 注册了我的第一个域名，要么是因为我在一个商业广告上听到了该公司的名字，并在脑海中将其与“如何获得域名”联系起来，要么是我在网上看到了一些交易。(大概就是那个。)

Watch

关于 GoDaddy 有很多*不*喜欢的地方——包括 [它过去在重要事情上的立场](https://www.thedailybeast.com/are-white-supremacist-sites-morally-offensive-to-godaddy)[它如何对待潜在客户](https://www.reddit.com/r/web_design/comments/a562gv/godaddy_is_a_scam/)[整个 SOPA 的事情](https://gizmodo.com/as-if-you-needed-another-reason-to-hate-f-cking-godaddy-5870559) ，以及 [它被抬高的定价模式](https://www.authormedia.com/6-reasons-authors-should-avoid-godaddy/) 。你现在可以在清单上增加一个烦恼了。最近，程序员伊戈尔·克罗明(Igor Kromin)发现 GoDaddy 在他的网站中注入令人讨厌的 Javascript。该代码是该服务的“真实用户指标”功能的一部分，如果该公司的美国数据中心托管着你的网站，你会自动选择使用该功能。

如果 GoDaddy 的代码是无声的，不引人注目的，这是一回事——这不是一个理想的场景，但也不可怕。然而，GoDaddy 很快承认，真实的用户指标可能会给用户带来一些问题，因为该公司在支持页面 上明确指出 [:”...使用的 javascript 可能会导致网站性能下降或网站崩溃/无法运行等问题。”](https://www.godaddy.com/help/why-am-i-signed-up-for-real-user-metrics-31969)

根据克罗明的报告，GoDaddy [决定取消真正的用户指标](https://www.zdnet.com/article/godaddy-javascript-injection-tracks-website-performance-but-might-break-it-too/) ，直到它可以将“功能”转化为实际的选择加入程序——你知道，那种你必须勾选一个框才能接受的东西。现在是重新考虑你和 GoDaddy 关系的好时机。或者，至少，考虑一下你如何使用这项服务。

### **检查你网站的设置很重要**

无论你是坚持使用 GoDaddy 还是完全转移到一个新的主机，GoDaddy 的“选择加入”实践都是一个很好的提醒，定期检查你的网站是否有古怪。制作一个样本页面，看看你的代码。里面有什么看起来奇怪的东西吗？您可能无法逃脱主机的代码插入，但是知道它们是什么、它们在做什么以及它们是否以任何方式影响了您的站点功能是很重要的。

另外，花些时间仔细研究一下你的网站的主机设置。你可能并不完全理解它，你可能真的需要挖掘来发现你在不知不觉中“选择加入”的任何其他项目点击界面中所有的菜单按钮，打开所有的上下文提示，浏览你的主机提供的每一个选项，这样你就不会错过那些烦人的额外功能，否则你可能会禁用它们。就代码注入而言，你也可以尝试为你的网站设计一个强大的内容安全策略，但它不是万能的， [正如一位评论者](https://www.igorkromin.net/index.php/2019/01/13/godaddy-is-sneakily-injecting-javascript-into-your-website-and-how-to-stop-it/#comment-4285084983) 在 Kromin 的帖子中指出的:

> 如果你不信任你的主机，CSP 之类的东西是很好的，但是它是一个响应头，所以服务器提供者可以在发送头到客户端之前将任何脚本添加到 CSP 列表中，从而允许他们想要的任何东西。他们还可以使用 NGINX 或 Apache 轻松地反向代理他们自己的脚本，以便 yoursite(dot)com/inject.js 每次都加载他们自己的脚本。除非你信任你的主机，否则没有头文件可以解决这个问题。

### **考虑切换到不同的网络主机**

你可以随时删除像 [这样的 GoDaddy，一个糟糕的火绒日期](https://lifehacker.com/leave-these-things-out-of-your-tinder-profile-1827515383) ，注册一个给你预制模板玩的网站——像 [Squarespace](https://www.squarespace.com/) 或[Wix](https://www.wix.com/)——只要把你的域名指向他们为你创建的任何地址。这将限制你的创造力*和*你的银行账户，但如果你只是需要一个外观漂亮、功能良好的基本网站，这是一个选择。

至于选择一个让你用你想要的任何东西填充空间的主机，你有大约一百万种不同的选择。我不会假装好像我有一个最好的清单。然而，我在网上看到了一些公司的推荐，比如[【iwantmyname】](https://iwantmyname.com/)[digital ocean](https://www.digitalocean.com/)[Cloudways](https://www.cloudways.com/en/)[甘地](https://www.gandi.net/en/simple-hosting)[blue host](https://www.bluehost.com/)[site ground](https://www.siteground.com/)[InMotion Hosting](https://www.inmotionhosting.com/) [主机](https://www.hostgator.com/) ， [节点主机](https://www.nodehost.ca/) ， [中期](https://www.midphase.com/) ， [场地](https://www.siteground.com/) ...仅举几个例子。

最重要的是，确保您选择的主机和计划符合您的需求。如果你不太确定如何建立一个基本的网站 ，不要选择一个在服务器上给你空间并让你去想怎么做的主机。提供更多手持或预配置内容管理系统的主机可能是更好的选择。

也不要发疯。如果你正在建立一个小型的 Wordpress 网站来存放你的简历和一些图片，你可能不需要购买一个承诺无限存储和带宽的昂贵的软件包。您可能会得到一个更基本的包。

当然，了解一点主机产品背后的技术是有帮助的。你的网站会坐落在一个 [共享服务器](https://en.wikipedia.org/wiki/Shared_web_hosting_service) 和一千个其他的共享服务器上吗？你的网站会在一个 [虚拟私人服务器](https://en.wikipedia.org/wiki/Virtual_private_server) 上运行吗？你认为你有足够的流量来保证一个 [专用服务器](https://en.wikipedia.org/wiki/Dedicated_hosting_service) ？你应该选择一个只为人们使用的带宽付费的云服务器吗？如果你得到的比你需要的多(或少)，在这些设置之间切换有多容易？

如果你发现一个主人有一个甜蜜的服务促销协议，请务必阅读小字。你看到的网站托管的低费用可能只适用于几个月，或者第一年，而实际费用可能比你愿意为一个网站支付的费用要高。不要玩蓝多·卡瑞辛，被一笔变坏的交易骗了。

最后，去找一些评论。不管你是在搜索谷歌。Reddit、 Stack Exchange 或其他任何地方，根据用户的实际体验找到真实、合法的评论，而不仅仅是他们对网络主机产品的粗略浏览。这可能需要一点挖掘，但这是为网站主持人获得一份简历的最好方法之一，而且它也有助于确保你在任何你可能需要知道的关于你的潜在选择的新闻上。如果用户开始评论你的首选主机开始，比方说，注入代码到他们的网站，导致他们崩溃，你可能要调查你的第二选择。