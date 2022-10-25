# 你终于可以在 Firefox 中加入缩放通话了

> 原文:[https://life hacker . com/you-can-finally-join-zoom-calls-in-Firefox-1843262033](https://lifehacker.com/you-can-finally-join-zoom-calls-in-firefox-1843262033)

Mozilla 的 Firefox 浏览器的一个奇怪之处在于，它允许你通过网络加入 Zoom 通话，不需要下载单独的应用程序，但你不能在通话中说任何话。或者至少，在最新的更新之前你不能。

Watch

没错。如果你最近试图使用你电脑的音频——换句话说，就是它的麦克风——在你通过之前版本的火狐、加入的会议中，你会看到弹出的这条消息:

我说“以前的版本”，因为 Mozilla 已经通过其对音频工作包的新支持在 Firefox 76 中修复了这个问题——这是一种“运行定制 JavaScript 音频处理代码的有用方式”，Mozilla 的 [克里斯·米尔斯和哈拉尔德·基尔希纳](https://hacks.mozilla.org/2020/05/firefox-76-audio-worklets-and-other-tricks/) 写道。正如 Mozilla 在 [一篇开发者文档](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API/Using_AudioWorklet) 中所阐述的:

> 当 Web Audio API 首次被引入浏览器时，它包含了使用 JavaScript 代码创建定制音频处理器的能力，这些处理器将被调用来执行实时音频操作。ScriptProcessorNode 的缺点很简单:它运行在主线程上，因此在它完成执行之前会阻塞其他所有正在进行的事情。这远远不够理想，尤其是对于像音频处理这样计算量很大的东西来说。”
> 
> *“输入 AudioWorklet。音频上下文的音频工作小程序是脱离主线程运行的工作小程序，通过调用上下文的 audioWorklet.addModule()方法来执行添加到其中的音频处理代码。调用 addModule()加载指定的 JavaScript 文件，该文件应该包含音频处理器的实现。注册处理器后，您可以创建一个新的 AudioWorkletNode，当该节点与任何其他音频节点一起链接到音频节点链中时，它将通过处理器的代码传递音频。*

干净利落。对于那些没有技术倾向的人来说，这种实现让你最终可以通过网络加入 Zoom 通话，并使用笔记本电脑的麦克风(或任何连接到电脑的麦克风)，就像你在使用常规的 ol' Zoom 桌面应用程序一样。安装最新版本的火狐浏览器(通过右上角的**汉堡菜单>帮助>关于火狐浏览器**)，现在当你在浏览器中加入一个缩放会议时，你会看到这个:

### 在 Firefox 中找不到 Zoom 的“从你的浏览器加入”选项怎么办？

这里有一个有趣的怪癖。当我测试这一切时，我注意到我复制并粘贴到 Firefox 的常规 Zoom 邀请链接不断告诉我“下载并运行 Zoom”以访问我的会议。在 Firefox 中，我没有看到任何简单加入会议*的方法。*

有两种方法可以解决这个问题。首先，无论是谁主持会议，都需要确保他们已经在 Zoom 的基于网络的设置中启用了“通过网络加入”选项。有，在 Zoom 的网站上；而不是它的桌面应用。让他们 [点击这里](https://zoom.us/account/setting) 并寻找“‘显示从你的浏览器加入’链接”切换。他们会希望实现这一点。

如果你*仍然*没有在你的浏览器中看到加入一个人的缩放会议的选项，还有一个技巧你可以试试:不要点击这个人发送给你的加入会议的链接，手动在 Firefox 中调出[**join . Zoom . us**](https://join.zoom.us)。

你需要输入会议 iD，这是在提供给你的缩放 URL 中“/j/”之后的第一个长串数字，假设你没有收到标准的邀请电子邮件。您还需要输入会议的密码，即 URL 的“pwd=”部分之后的第二个字符块。

做这两件事，你会看到直接加入 Firefox 中的缩放会议的选项。现在你已经更新了 Firefox，你可以在那里说点什么了。