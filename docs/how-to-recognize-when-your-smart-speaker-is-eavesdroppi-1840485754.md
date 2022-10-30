# 如何识别你的智能音箱在偷听

> 原文：<https://lifehacker.com/how-to-recognize-when-your-smart-speaker-is-eavesdroppi-1840485754>

并非所有东西都必须成为其他东西的平台，在你的智能家居中尤其如此。虽然你可以用技能、动作和应用程序来补充你的智能扬声器——我们主要谈论的是亚马逊的 Echo 和谷歌的家用设备——但你应该三思而后行。任何一家公司尚未纠正的漏洞都可能让你遭受恶意开发者的网络钓鱼或窃听。



虽然这次 [激光攻击](https://lifehacker.com/how-to-protect-your-smart-speaker-from-a-laser-attack-1839642064) 并不稀奇，但安全研究实验室的研究人员已经证实，与亚马逊和谷歌的扬声器如何处理语音命令有关的 [几个月前的漏洞](https://srlabs.de/bites/smart-spies/) 仍有待修复。因此,“诈骗”应用程序(两家公司似乎都难以捕捉)可以从不知情的用户那里窃取重要的安全信息。

下面是 SRLabs 的 [描述](https://srlabs.de/bites/smart-spies/) 一个应用如何利用漏洞:

> *1。创建一个看似无害的应用程序，其中包含由“start”触发的意图，该意图将接下来的单词作为槽值(转发给应用程序的可变用户输入)。此意图的行为类似于回退意图。*
> 
> *2。亚马逊或谷歌会在语音应用发布前审查其安全性。我们在此审查后更改功能，这不会提示第二轮审查。特别是，我们将欢迎消息改为假的错误消息，让用户认为应用程序还没有启动。(“这项技能目前在你们国家是没有的。”)现在用户假设语音 app 不再监听。*

> *3。通过让语音应用程序“说出”字符序列“↑”，在错误消息后添加任意长的音频暂停(U+D801，点，空格)。因为这个序列是不发音的，所以说话者在活动时保持沉默。让应用程序多次“说”字符会增加这种沉默的时间。*
> 
> *4。最后，过一会儿结束沉默，播放一条钓鱼消息。(“您的设备有一个重要的安全更新。请说开始更新，然后输入您的密码。).用户在“开始”后说的任何话都会被发送到黑客的后端。这是因为之前的意图类似于回退意图，现在将用户输入的密码保存为一个槽值。"*

在另一种攻击媒介中，开发人员可以通过提交常见的单词作为触发器来创建窃听例程，例如“address 结合一个虚假的“停止”声明，像你的说话者说“再见”，并使用之前的“隐藏”字符技巧延长说话者保持活跃的时间。如果一个人在这段时间的某个时刻说了一个触发词，说话者会记录下他所说的话，并发送给开发者。

如果这很难理解，这里有一个利用的视频:

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-A3n-0AbXznc&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-A3n-0AbXznc&start=0) 

同样的黑客风格在谷歌设备上略有不同，但也更强大，因为不需要触发词(并且“窃听”期可以永远持续下去):

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-X2gddqD1wUI&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-X2gddqD1wUI&start=0) 

### 如何为你的智能音箱补充技能

虽然亚马逊和谷歌据称正在加紧审查过程，以捕捉试图利用你的设备的技能、行为和其他集成，但这并不顺利。正如 [ThreatPost](https://threatpost.com/alexa-google-home-eavesdropping-hack-not-yet-fixed/151164/) 所写的，利用这些漏洞的被移除的应用可以被重新提交(甚至被批准)。这一点，以及整个诱饵和开关方面——合法的技能得到认可，却被更具恶意的代码所取代——本身就是有问题的。

我们的建议？坚持使用已知开发人员的技能和行动，这些技能和行动已经被其他人审查过了。例如，从 [一个有大量评论的 ESPN 技能](https://smile.amazon.com/ESPN/dp/B074JCPM4M?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-recognize-when-your-smart-speaker-is-eavesdroppi-1840485754&asc_source=&sa-no-redirect=1&tag=kinjalifehackerlink-20) 中获取你的运动分数，而不是从某个随机用户上周创造的“运动技能”中获取。你可以把它加入书签，以后再回来查看，看看其他用户是否觉得它合法。

最重要的是，*时不时看看你的智能音箱*。不要仅仅假设一个响应的结束——无论是通过“叮”声还是其他信息——意味着你的说话者已经完成了对命令的处理。知道你的设备的 [物理](https://smile.amazon.com/gp/help/customer/display.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-recognize-when-your-smart-speaker-is-eavesdroppi-1840485754&asc_source=&nodeId=G201601790&tag=kinjalifehackerlink-20) [信号](https://support.google.com/googlenest/answer/7073219?hl=en) 是什么，当你激活第三方技能时，看看它，而不是吼它。如果你的设备以某种奇怪的方式保持活跃，这是一个很好的线索，你正在使用的技能或行动可能需要额外的调查。

最后，修剪你的 [技能](https://smile.amazon.com/gp/skills/your-skills?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-recognize-when-your-smart-speaker-is-eavesdroppi-1840485754&asc_source=&ie=UTF8&ref_=sv_a2s_4&tag=kinjalifehackerlink-20) 和 [动作](https://support.google.com/googlenest/answer/7126338?co=GENIE.Platform%3DAndroid&hl=en) 。如果您不记得上次在智能扬声器上使用第三方应用程序或服务是什么时候，请取消它访问您的设备(或关联帐户)的能力。不要让未使用的集成堆积起来，因为它所需要的只是一个转换它的焦点，在你的数字生活中引起一些不愉快。