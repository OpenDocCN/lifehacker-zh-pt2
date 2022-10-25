# 为什么我的笔记本电脑需要 30 分钟才能启动？

> 原文：<https://lifehacker.com/why-does-my-laptop-take-30-minutes-to-start-up-1832958231>

你可能会遇到的一个更烦人的情况是台式机或笔记本电脑永远无法加载。它最终会出现，但最确定的迹象之一是，当你的系统启动到 Windows 或 macOS 的时间比以前长得多时，特别是如果你正在等待几分钟而不是几秒钟来开始使用你的电脑。

Watch

Lifehacker 读者**佩吉**也为类似的问题所困扰，她在给 [**科技 911**](https://lifehacker.com/c/tech-911) 的邮件中描述道:

“我的笔记本电脑开机相当快，但运行起来非常慢，而且会持续很长时间。任务管理器告诉我磁盘处于 100%状态。这种情况会持续 30 分钟。我在谷歌上搜索了这个问题，并尝试了第一个建议(大冒险)，即停止 SuperFetch。没用。那么答案是什么呢？(大约 4-5 年前运行 Windows 的戴尔笔记本电脑，全部自动更新。)"

我的第一个想法是，您的系统上有某种应用程序正在挂起或消耗大量的资源。您应该能够很容易地检查这一点——只需通过任务管理器查看是什么占用了您的 CPU 这么多，您将能够通过根据列进行排序来找到它。

如果你不知道是什么在使用你的 CPU，只要右击应用程序，选择“在线搜索”就可以了。一旦你确定了罪魁祸首，你就会对如何处理这个程序有一个更好的想法。无论是什么问题，只要卸载/重新安装它就可以解决，这取决于应用程序。

由于我看不到你的任务管理器，我不能更具体地告诉你该怎么做，尤其是如果这个烦人的应用是你可能不想摆脱的——比如谷歌浏览器，如果那是你的选择。)

总之，奇怪的是，影响你电脑的东西会在你开机后消耗掉 30 分钟左右的时间。我最初的想法是，也许有某种扫描或备份应用程序疯狂运行，但我不能说我曾经注意到 [Windows Defender](https://lifehacker.com/disable-defender-in-windows-10-home-by-installing-anoth-1772447028) 或 [Backblaze](https://lifehacker.com/how-to-back-up-your-files-now-that-crashplan-isnt-an-op-1798320345) 在我自己的系统上失控，这只是两个例子。

考虑运行全面的恶意软件扫描*，以防万一*。虽然我怀疑你被感染了，但确定一下也无妨。获取免费版的 [Malwarebytes](https://www.malwarebytes.com/mwb-download/) ，给你的系统做一次全面的“威胁扫描”幸运的话，你不会发现任何东西——尽管这不会确切地帮助我们找到你的系统为什么慢的原因。

你还应该 [检查 Windows 启动](https://lifehacker.com/how-to-stop-annoying-apps-from-loading-when-windows-boo-1829810394) 时加载的所有程序，并把列表精简到必要的部分。你可以通过任务管理器的启动标签来做到这一点:点击它，按“状态”排序(如果你从来没有这样做过的话，应该对所有的事情都“启用”)，并开始查看当你的计算机启动时启动了哪些程序。你可能不知道其中的大部分，但你总是可以右击“在线搜索”，就像你以前做的那样。

我的建议是禁用任何“助手”应用程序，或者那些位于后台以稍微加快加载另一个应用程序的程序。例如，您可能不需要在系统启动时加载 iTunes 助手工具，也不需要 Adobe 助手。如果你不使用 OneDrive，你也可以放弃它(尽管你可能会在设置中取消选中“当 Windows 启动时自动启动 OneDrive”选项。

你也可以尝试运行一个更核的选项:“TronScript”这是一个社区生成的脚本和行动的组合，旨在清理您的系统。我自己从来不需要使用它，但是考虑到你的情况的复杂性，它可能值得一试。下载 [实用程序](https://old.reddit.com/r/TronScript/comments/asx44a/tron_v1076_20160220_stage_2_fix_definition_updates/) ， [阅读说明](https://github.com/bmrf/tron/blob/master/README.md) ，备份你的关键文件，首先，以防 TronScript 因为某种原因最终弊大于利。

如果我是你，我只会说，“见鬼去吧”，把你的文件备份到别处，然后 [从头开始重新安装 Windows](https://lifehacker.com/the-ultimate-guide-to-reinstalling-windows-from-scratch-1832897572)。当我的电脑给我带来相当大的痛苦时，我通常会选择这个选项。我花了一个小时左右的时间来重新设置所有的东西——以及全新安装的速度——往往比浪费无数个小时试图用大杂烩式的修复来排除系统故障要好。但这只是我。走这条路，我打赌你会解决你的系统给你带来的任何问题。

(假设你的旧笔记本电脑仍然使用硬盘驱动器，而不是固态硬盘，你也可以以便宜的价格购买后者，备份文件，更换驱动器，并在速度更快的固态硬盘上重新安装 Windows 10。 [做](https://lifehacker.com/how-to-migrate-to-a-solid-state-drive-without-reinstall-5837543) 并不是特别难，即使你以前从来没有做过，你也会看到性能有很大的提高。)

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>*</small> 

<small></small>