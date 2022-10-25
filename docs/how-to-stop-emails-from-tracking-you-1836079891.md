# 如何阻止电子邮件跟踪你

> 原文：<https://lifehacker.com/how-to-stop-emails-from-tracking-you-1836079891>

电子邮件跟踪可能是一种糟糕的做法。我想不出更好的方式来描述最新的报道，硅谷时尚 [超人](https://gizmodo.com/silicon-valley-s-hottest-email-app-raises-ethical-quest-1836051629)——一个月 30 美元的电子邮件服务——记录电子邮件收件人打开邮件的次数。



你可能会想:“拜托，这没什么大不了的。你在看一封邮件。谁在乎？”我第一次看到新闻的时候也是这个立场。我收到很多电子邮件，如果有人在邮件上贴了一个跟踪像素来看我是否看了一眼，这并不会真的冒犯我。然而，当我深入挖掘时，很容易看出为什么超人的跟踪技术如此糟糕:它计算打开的次数*和*提供电子邮件被打开的位置列表。

在这个例子中，[InVision 公司合作与社区副总裁迈克·戴维森完美地总结了](https://mikeindustries.com/blog/archive/2019/06/superhuman-is-spying-on-you) 超人的问题:

> *前男友是写绝望邮件的超人用户。主题:“我一直在想我们”。他把它寄给了他的前搭档。她早上 9 点到洛杉矶市中心上班的时候就会读这本书。她会在晚上 7 点和朋友在帕萨迪纳吃晚饭前再读一遍。她凌晨 1 点在圣莫尼卡的家里又读了一遍。周末，她去了趟纽约，又读了一遍。两次。她决定不回复这封邮件，因为她的前任曾经跟踪过她，她不想再进一步交流了。但由于跟踪像素，她的电子邮件总是在交流，分享她不想发送的信息，甚至不知道她在发送。她没有回复，但她的前任仍然知道她看了他的邮件五次，包括很可能在她的床上。他知道她去了纽约。*

呃。

令人欣慰的是，该公司已经在位置追踪方面扭转了方向。在这种做法传遍互联网后不久写的一篇博客文章中，创始人兼首席执行官 Rahul Vohra 表示，位置跟踪正在消失——更好的是，Superhuman 正在删除它之前收集的与电子邮件打开相关的任何位置数据。他在 [中写道](https://blog.superhuman.com/read-statuses-bdf0cc34b6a5) :

> “看了评论后，我开始明白确实有涉及位置跟踪的噩梦场景。我应该指出，我们故意不显示城市——我们只显示州或国家——但是一个坚定的攻击者仍然可以滥用这些信息。
> 
> 对此我非常抱歉。当我们建造超人时，我们只关注客户的需求。我们没有考虑潜在的坏演员。我真诚地为没有更全面地考虑这件事道歉。"

这当然很好，但是你不应该指望公司~~公开指责~~做正确的事情。控制你的在线隐私是你的责任，你可能还没有真正考虑过你的电子邮件中那些你看不到的东西——以及它们会泄露你的哪些信息。

### 如何防止公司跟踪你的电子邮件活动

制止大多数电子邮件跟踪行为的最快最简单的方法是**阻止你的电子邮件应用程序自动加载图像**。当他们这样做的时候，打开一封电子邮件也会加载公司嵌入其中的任何微小的追踪像素。根据您的提供商如何处理电子邮件中的图像，这可能会透露一点(您的 IP 地址)或不多(图像只是被加载)，从而给公司提供不同程度的有关您的信息。(例如，Gmail 通过代理服务器加载图像，因此公司可以看到你打开了图像，但无法推断出你的位置。)

在基于浏览器的 Gmail 版本上，这很简单，只要进入其 [设置](https://mail.google.com/mail/u/0/#settings/general) ，向下滚动到“图像”行，选择“显示外部图像前询问”

如果您使用的是 Android 版本的 Gmail，也可以设置此选项；不幸的是，iOS 用户总是会在 Gmail iOS 应用程序上自动加载图像。

(如果你切换到 iOS 的默认邮件应用，并通过这种方式接收 Gmail 帐户的邮件，你可以通过进入**设置**应用> **邮件**，取消选中“邮件”部分下的“加载远程图像”来关闭自动图像加载。)

无论你是在 [Outlook](https://support.office.com/en-us/article/block-or-unblock-automatic-picture-downloads-in-email-messages-15e08854-6808-49b1-9a0a-50b81f2d617a) 、 [雅虎邮箱](https://help.yahoo.com/kb/SLN5043.html) 、 [雷鸟](https://support.mozilla.org/en-US/kb/remote-content-in-messages) 、 [Windows Mail](https://answers.microsoft.com/en-us/windows/forum/all/windows-10-mail-automatically-downloads-images/7a5b63be-a208-4356-a420-cb11033b61da) 、 [Mail](https://support.apple.com/guide/mail/change-viewing-preferences-cpmlprefview/mac) (macOS)、 [Mailbird](https://support.getmailbird.com/hc/en-us/articles/220107267-Always-Show-Remote-Images) 还是其他什么，花点时间浏览一下你的应用程序设置和文档，看看你是否或者如何禁用图片当然，当你想让看到图像时，这将增加一个额外的步骤——当你加载这些图像时，它不会停止跟踪像素——但它至少会让你对这个过程有更多的控制。至少，这比什么都没有强。

当然，你也有一些处理这种困境的选择。如果您想手动或自动查看电子邮件中的图像，但不触发跟踪像素，请考虑使用浏览器扩展。(这一步显然对桌面或移动应用不起作用。)

超人本身推荐两个扩展: [**丑邮**](https://uglyemail.com/) 和[**pixel block**](https://chrome.google.com/webstore/detail/pixelblock/jmpmfcjnflbcoidlgapblgpgbilinlem)(或者[**pixel block 2**](https://chrome.google.com/webstore/detail/pixelblock-2/eaheehidcidghlmmpdogfhgmibpelndm))。丑陋邮件适用于 Firefox 和 Chrome，而 Pixelblock 只适用于 Chrome。两者都可以完全免费使用，但它们只能在 Gmail 上使用——向那些还没有搭上谷歌列车的人道歉。

你可以尝试使用一个更通用的(开源的)扩展，比如 [**uMatrix**](https://github.com/gorhill/uMatrix) ，它会阻止*所有不在你的白名单上的*。这有点复杂，但如果你不介意做一些工作来阻止任何基于网络的电子邮件提供商的跟踪像素，这是一个强大的选择。你也可以试着在扩展中设置过滤器，比如[**uBlock Origin**](https://github.com/gorhill/uBlock)，但是这也需要一些跑腿的工作——你必须在阻塞 之前知道 [要阻塞什么，这感觉像是一个无休止的任务。](https://medium.com/@chadloder/how-to-disable-superhumans-email-tracking-pixel-ba4f9ccdf731)

虽然你有相当多的技术工具可以用来防止电子邮件跟踪，你也应该使用常识。如果你不想让公司跟踪你，首先，不要打开邮件。如果电子邮件中有分散的链接，你点击它们，假设公司 [现在知道你做了那个](https://www.reddit.com/r/privacy/comments/9m3478/how_to_block_email_link_tracking/) (显然，你打开了电子邮件)。

### 测试您的隐私调整

一项非常有用的服务是名副其实的 [**电子邮件隐私测试器**](https://www.emailprivacytester.com/) ，它可以让你一窥不同的电子邮件追踪方法在你的应用程序或浏览器上是否有效。用它给自己发一封电子邮件——从技术上来说，首先是一封确认邮件，然后让你给自己发一封充满不同跟踪方法的测试邮件。

您可以使用该网站尝试一系列不同的跟踪技术，包括图像和 [链接预取](https://www.reddit.com/r/privacy/comments/7awtww/email_leakage_of_personal_information/dpdtt8y/) (仅举两例)。一旦你给自己发了一封测试邮件，打开你的电子邮件应用并打开它。你要做的就是这些。(如果你找不到所说的测试邮件，一定要先检查你的垃圾邮件文件夹。)

然后，您可以在电子邮件隐私测试网站上看到跟踪结果:

如果你看到很多红色，也许是时候调整你的电子邮件设置，给自己一些额外的隐私了。