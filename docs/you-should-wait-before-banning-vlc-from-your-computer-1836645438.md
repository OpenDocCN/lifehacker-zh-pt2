# 你不需要从你的电脑上卸载 VLC[更新]

> 原文：<https://lifehacker.com/you-should-wait-before-banning-vlc-from-your-computer-1836645438>

今天有消息称，VLC 媒体播放器——非常受欢迎，也是 life hacker 推荐的——据称有一个非常严重的漏洞，可能会允许一个“陷阱”视频，正如 [The Register](https://www.theregister.co.uk/2019/07/23/remote_code_flaw_vlc/) 所说，要么让播放器崩溃，要么执行远程代码。前者？一个烦恼。后者？这是一个巨大的安全问题，我们建议卸载 VLC 来解决这个问题，直到它的创建者 VideoLAN 发布补丁。



但是我们现在还不建议采取这个行动，因为事情还没完。这个问题的错误报告已经在 [开放了四周](https://trac.videolan.org/vlc/ticket/22474) ，但是 VideoLAN 总裁兼首席 VLC 开发者让·巴普蒂斯特·肯普夫今天留下了一系列评论，表明所谓的错误并不像每个人所说的那样严重。他在三条不同的评论中写道:

> *“这不会使 VLC 3.0.7.1 的正常版本崩溃”*
> 
> “如果你是通过一篇声称 VLC 存在严重缺陷的新闻文章得到这张票的，我建议你先看看上面的评论，并重新考虑你的(假)新闻来源。”
> 
> 抱歉，这个错误是不可重现的，而且根本不会让 VLC 崩溃

VideoLAN 也在 Twitter 上谈论这个 bug——或者更确切地说，这个非 bug。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1153715138333220864&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1153715138333220864&autosize=1)  [https://lifehacker.com/embed/inset/iframe?id=twitter-1153715775217254400&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1153715775217254400&autosize=1) 

### 你该拿 VLC 怎么办？

我们已经在本文末尾发布了 VideoLAN 的官方回应，它详细描述了这个潜在的破坏 VLC 的漏洞实际上并不算什么。我保留了我们文章的原文，因为我认为展示我们为什么建议采取比卸载 VLC 并把你的笔记本电脑扔进火里——*或其他任何人建议的更有分寸的回应背后的思考过程是很重要的。*

首先，你可以**从 bug** 的原 filer 下载 [**一个概念验证视频**](https://trac.videolan.org/vlc/attachment/ticket/22474/heap-over-flow.mp4) **，看看它在播放时是否会崩溃你的 VLC。(《纽约时报》报道称，他们的 VLC 版本(3.0.7 版)崩溃了，但我在我的基于 Windows 的 VLC·3.0.7.1 版本上没有遇到任何问题。)这不一定能告诉你你的 VLC 版本是否安全，不会被远程代码执行，但这是一个值得研究的有趣的数据点。**

其次，**如果你在 Mac 上使用 VLC，你完全没问题**。据称，问题中的漏洞只影响 VLC 的 Windows、Unix 和 Linux 版本。同样，这个错误似乎只会影响。MKV 文件——如果你甚至不知道那是什么，或者不看，你没事。

第三，也是最重要的一点，**你必须决定相信谁** : [来自德国计算机应急小组(CERT-Bund)的安全顾问](https://www.cert-bund.de/advisoryshort/CB-K19-0634) ，是他们将整个混乱的局面公之于众，还是否认问题的存在和严重性的 VideoLAN 本身。

我认为水已经够浑浊了，我还不会从我所有的系统中卸载 VLC。然而，你能做的是把它暂停。目前，切换到第二媒体播放器——或者，我敢说，回到 Windows Media Player——并将其设置为媒体文件的默认播放器(开始按钮>键入“默认应用程序”>将你的音乐和视频播放器切换到其他东西)。

关注 VLC 的 [变更日志](https://www.videolan.org/developers/vlc-branch/NEWS) ，等待该公司发布修补该漏洞的新版本播放器——如果它甚至打算这么做的话。如果几个次要版本(或一个主要版本)过去了，一切似乎都很好，考虑回到使用 VLC。

无论如何，请确保您总是下载 VLC 的最新更新(通过“帮助”>“检查更新”)。在设置中启用 VLC 的“激活更新通知”选项也很棒，这样你就可以立即知道该是应用程序的新版本了。

**2019 年 7 月 24 日上午 10:00 更新:** *VideoLAN 发布了一份关于所谓的可怕 bug 的完整解释。一切都好！*

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1153965969456422913&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1153965969456422913&autosize=1)  [https://lifehacker.com/embed/inset/iframe?id=twitter-1153965977182203904&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1153965977182203904&autosize=1)