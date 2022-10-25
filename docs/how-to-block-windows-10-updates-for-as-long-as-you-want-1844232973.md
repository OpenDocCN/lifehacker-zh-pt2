# 如何随心所欲地屏蔽 Windows 10 更新

> 原文：<https://lifehacker.com/how-to-block-windows-10-updates-for-as-long-as-you-want-1844232973>

我一般不建议推迟太久的系统更新，但是有很好的理由让你对 Windows 10 的主要功能更新保持警惕。微软在提供不会破坏你的系统的完美更新方面的记录是不稳定的(说得好听点是)，给主要的 Windows 更新一点时间是值得的——以防万一微软需要修复一两个关键问题。



Windows 10 Home 上的大多数人可以总共按五次 Windows Update 中的“暂停更新 7 天”按钮——在你的操作系统强制安装重大更新之前，给你 35 天的自由。I 如果你想直接结束，点击“高级选项”可以让你手动选择一个 35 天后的日期。(或者更少——我是 Windows 的内部人员，而我们只限于七天。)

如果你需要更多的时间——因为你持怀疑态度，你有一些硬件会对 Windows 更新产生重大问题，或者你对 [微软将你 365 天的延迟](https://gizmodo.com/microsoft-kills-one-of-its-best-windows-10-update-looph-1844180993)减少到 35 天感到恼火——你必须求助于第三方应用程序。我推荐[**Spydish**](https://github.com/builtbybel/spydish)*(*[*virus total report*](https://www.virustotal.com/gui/file/d93aabde231211ec16044742ad9a7174007c1749a42d9081fbafe8e9572e2359/detection)*)*，如果你正在寻找来微调 Windows 10 的许多政策并配置你的隐私设置，而不需要在上百个不同的菜单中导航，这是一个非常有用的小应用。

一旦你启动应用程序，你首先要点击大的“分析”按钮，看看 Windows 10 的各种政策是如何在你的系统上配置的。

向下滚动左侧边栏，直到看到更新标题，然后选择“阻止主要 Windows 更新”选项我怀疑这只适用于 Windows 10 Pro 和企业版，当你悬停在项目*和*上时，你会得到工具提示，事实上它基本上自动化了 [这个注册表黑客](https://www.bleepingcomputer.com/news/microsoft/this-registry-trick-lets-you-block-major-windows-10-updates/) 。

如果你是一名 Windows 10 家庭用户，并且你发现这并不奏效，你可以尝试其他工具。我刚刚在 Windows 10 Home 上测试了 [**Wu10Man**](https://github.com/WereDev/Wu10Man) ，并启用了它的所有设置(包括通过 hosts 文件阻止 Microsoft Update 域，这触发了 Microsoft Defender 警告)成功了:我无法下载和安装*任何* Windows 更新

如果连都不适合你，还有 [和其他很多应用](https://www.thewindowsclub.com/free-update-blocker-tools-to-stop-automatic-windows-10-updates/) 你可以试试。我没有亲自测试过它们，所以我提供了这样的建议:选择那些更像便携式应用程序而不是你必须安装的程序。首先，你会给自己一点额外的保护，以防潜在的问题。第二，确保你备份了你的系统——如果你喜欢的话，甚至 [创建了一个系统还原点](https://lifehacker.com/the-complete-guide-to-windows-system-restore-its-bette-5466794#:~:text=If%20you're%20using%20Windows,longer%20than%20a%20few%20seconds.)——以防任何对这些应用程序的调整都会严重破坏你的系统。

第三，也是最重要的一点，一旦你觉得安装 Windows 10 更新是安全的，不要忘记关闭这些应用程序或恢复它们所做的任何更改。这并不是要阻止更新永远安装下去——同样，除非你有一些专门的硬件，如果你执行更新，这些硬件绝对不能工作。为了你现在的稳定性，你只是延迟了这些更新；为了你的长期安全，你应该安装一次你有一个合理的保证他们不会冲洗你的系统。