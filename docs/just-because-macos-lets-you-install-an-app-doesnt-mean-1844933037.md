# macOS 让你安装一个应用不代表它不是恶意软件

> 原文：<https://lifehacker.com/just-because-macos-lets-you-install-an-app-doesnt-mean-1844933037>

只要 macOS 让你装个 app，应该就安全了吧？这是苹果看门人和 [公证服务](https://developer.apple.com/documentation/xcode/notarizing_macos_software_before_distribution) 的点，早在二月份就开始在 macOS Catalina 强制执行。从理论上来说，这意味着你在 Mac 上安装的任何应用程序*都应该*已经过苹果的 [恶意组件检测](https://developer.apple.com/documentation/xcode/notarizing_macos_software_before_distribution) 。”但是，如果你认为任何带有 [看门人绿灯](https://support.apple.com/en-us/HT202491) 的应用程序实际上是安全的，那你就错了。

Watch

Objective-See 的 Patrick Wardle [最近的一篇文章描述了](https://objective-see.com/blog/blog_0x4E.html) ，有一种新的 Mac 攻击正在传播，它使用网关守卫传递有效载荷来分发一种特别流行和有问题的恶意软件:OSX.Shlayer

> *“上周五，twitter 用户 Peter Dantini (@PokeCaptain)注意到 homebrew.sh 网站(不要与合法的 homebrew 网站 brew.sh 混淆)正在举办一场活跃的广告软件活动。如果用户无意中访问了 homebrew.sh，在各种重定向之后，会强烈推荐“Adobe Flash Player”的更新。*
> 
> *[...]有趣的是，Peter 注意到该活动源自 homebrew.sh，利用广告软件的有效负载实际上是完全公证的！😱"*

目前还不清楚这些程序是如何从苹果公司获得公证的，但是愚蠢到试图执行它们的用户不会触发任何关于其内容的警告。如果参选，他们会抛弃 OSX。这是目前 macOS 上最流行的恶意软件之一。

至于恶意软件是如何工作的，简单得令人痛苦。正如这篇卡珀斯基 [的博文](https://securelist.com/threats-to-macos-users/93116/#malicious-and-unwanted-programs-for-macos) 所描述的:

> *“值得注意的是，从技术角度来看，Shlayer 并没有什么特别之处。它的主要可执行文件是一个只有四行代码的 Bash 脚本。它所做的只是解密并运行它带来的另一个文件，然后下载、解密并执行另一个文件，这完全相同。最后，这个各种恶意软件的嵌套玩偶安装了几个广告软件程序，隐藏得很好，并注册在启动时运行。”*

如果你认为你被感染是因为你的 Mac 表现异常——你得到奇怪的弹出窗口，你的搜索结果指向奇怪的网站，或者你被提示安装一些你不想要的新的和奇怪的应用程序——你有可能感染了老 OSX。Shlayer(或者谁知道还有什么)。抓取类似免费版 [Malwarebytes](https://www.malwarebytes.com/mac) 的东西，运行它，清理你的系统。

为了避免将来发生这样的事情，你要重新提高警惕，在网络世界中导航。你永远不要下载任何含有“Adobe”、“Flash”和“Player”字样的东西，尤其是当你被诱骗“更新”这个应用程序的时候。当网站提示时，你也不应该安装任何视频播放器或编解码器，除非是*你*启动的。就像，去寻找并下载 [VLC](https://lifehacker.com/the-best-hidden-features-of-vlc-1654434241) 是可以的，因为你需要一个伟大的球员，然后去寻找一个。当一个网站*想让你*点击【接受】、【下载】或类似的东西，这*不是*可以的。

不要安装你不认识的应用。不要执行你不认识的文件。不要提取。你不认识的 DMG 文件。不要让未知程序将自己安装为 Safari 扩展，引诱你给它们新的“辅助功能”权限，或者在你的 Mac 上做其他你不喜欢做的事情。苹果的看门人可以稍微收紧一点，但能让垃圾远离你的 Mac 的最好的看门人是你的大脑。