# 救命啊！在最近的操作系统更新后，Windows 将无法正确启动

> 原文：<https://lifehacker.com/help-windows-wont-boot-correctly-after-a-recent-os-upd-1842509510>

在今天这一期的[**Tech 911**](https://lifehacker.com/c/tech-911)——life hacker 的技术支持专栏一周以来一直关注你在家工作的问题——我们将讨论一个老话题:微软 Windows。具体来说，当每次你试图启动操作系统时，Windows 开始抛出令人讨厌的错误信息，会发生什么？如果你试图在一天中登录并在关键的截止日期前完成工作，而你又没有真正的 IT 部门来帮忙，这可能是最糟糕的情况。

Watch

在我们扔给你一个数字救生圈之前，让我们从 life hacker reader[**patch kek**](https://lifehacker.com/1842437421)那里了解一下细节。

### 问问题:

> 我有一台 Windows 10 台式机。几周前，windows 进行了一次更新，几天后，当我开机时，我得到消息“windows 没有正确加载”蓝屏，有几个选项。我试过的那些都不太好用，直到我发现了“恢复到以前的日期”选项。效果很好。计算机恢复正常运行。不幸的是，每隔几天我还是会收到 windows 不能正常加载的屏幕。我在苹果电脑上运行 Windows 10。我想彻底擦干净窗户，然后重新装上。也许我感染了病毒或病毒？谢谢！！

### h umble a nswer:

不管怎样，你并不孤单。微软最近一直在 Windows 10 更新方面遇到问题，有时会给用户带来更多他们无法解决的问题。你有可能在这个阵营中，但好消息是，你被病毒或一些粗略的恶意软件攻击的可能性非常小。这只是一个 Windows 问题——我敢肯定，当你遇到这个问题时，听起来不会很安慰，但至少比“你的系统被感染了”(我希望)稍微安慰一些。

一般来说，我喜欢在出现问题的第一个迹象时就弃船，这可能会比我重新安装 Windows 和所有应用程序花费更长的时间来排除故障，结果好坏参半。我怀疑这可能是这里的情况。既然你是在 Mac 电脑上启动 Windows，我就不会因为让你暂时停止工作而感到困扰，因为如果你绝对需要在电脑上做一些事情，你总是可以使用 macOS。

不过，在我们使用核能之前，让我们先做几件事。首先，如果你能引导*进入*窗口——听起来你能——我不确定你能卸载什么来帮助你。上一次可能会影响你的 Windows 10 重大更新是 1909 年[11 月](https://support.microsoft.com/en-us/help/4529964/windows-10-update-history) 的大更新。从那时起，已经有了一些零碎的更新，但我想不出有什么问题。哦，除了 KB4535996，连微软都建议用户卸载。

所以，让我们从这里开始。拉起 **Windows 更新**，点击**查看更新历史**，点击**卸载更新**，看看能不能卸载 KB4535996。如果可以，太好了！如果没有，就没有故障排除技术。

当你在这里的时候，也许可以检查一下是否有其他可以安装的 Windows 更新。这是一个漫长的过程，但是也许已经有东西可以修复你的 Windows 系统正在努力解决的任何问题。由于你在 Mac 上使用 Boot Camp 运行 Windows，请打开苹果软件更新，并确保没有任何新的驱动程序或更新需要安装。

最后，尝试重新安装 Boot Camp 的 [Windows 支持驱动](https://support.apple.com/en-us/HT204923) ，这可能会神奇地治愈导致你的系统启动时蓝屏的任何原因。不能保证这就能解决问题，但是在你采取更激烈的措施之前，这是值得探索的。

在 Windows 中，您还可以打开提升的命令提示符(在开始菜单中搜索“命令提示符”，右键单击它，然后选择“以管理员身份运行”)。在那里，尝试运行一个简单的“chkdsk /f”来确认您的文件系统没有任何问题。您还可以尝试使用“chkdsk /r /f”来进行更彻底的分析和修复过程，但是这将花费更长的时间。如果您的硬盘出现故障，并且这是 Windows 问题背后的原因，也有可能您无法从 chkdsk 获得任何其他信息。你会想用 [和其他一些技巧](https://lifehacker.com/how-to-check-if-your-hard-drive-is-failing-1835065626) 来确认你没事(或者走向灾难)。

您也可以在同一提升的命令提示符下运行“sfc /verifyonly ”,然后运行“sfc /scannow”。如果第一个命令在 Windows 系统文件中发现任何损坏，第二个命令应该可以修复它们。

完成后，请考虑打开 Windows 疑难解答。拉起老派的控制面板(通过开始菜单)并选择故障排除。然后，点击“修复 Windows Update 的问题”，看看实用程序找到了什么(如果有的话！)

最后，点击开始菜单，点击电源图标，按住键盘上的 Shift 键，然后点击重启。这应该会引导你进入 Windows 10 的 [高级启动](https://www.dell.com/support/article/en-us/sln317102/booting-to-the-advanced-startup-options-menu-in-windows-10?lang=en) 选项菜单。点击疑难解答，点击高级选项，并尝试使用启动修复选项，看看是否可以解决您的 Windows 问题。

如果所有其他方法都失败了，那么擦除和恢复可能是您的最佳选择。将你所有重要的 Windows 10 文件保存到闪存盘或者 [云存储](https://lifehacker.com/google-one-is-now-open-for-everyone-but-is-it-a-good-d-1826049257) ，然后启动 macOS，使用 Boot Camp Assistant[移除你的 Windows OS](https://support.apple.com/guide/bootcamp-assistant/remove-windows-from-your-mac-using-boot-camp-bcmp59c41c31/mac) 。使用微软的 [媒体创作工具](https://www.microsoft.com/en-us/software-download/windows10) 下载一个新的、新鲜的。ISO 的 Windows 10，然后使用 [Boot Camp](https://support.apple.com/guide/bootcamp-assistant/get-started-with-boot-camp-on-mac-bcmp712cfeb8/6.1/mac/10.15) 在 Mac 上重新安装那个。一旦 WIndows 启动并运行，首先确保你已经安装了苹果的任何更新(前面提到的 Windows 支持驱动程序和苹果软件更新)，然后安装微软提供的所有 Windows 更新，*然后*一旦你确认一切正常，就开始将你的文件和应用程序 [放回你的系统](https://lifehacker.com/the-best-way-to-quickly-install-apps-on-a-new-windows-p-1836244140) 。

不用担心；这比听起来花费的时间要少得多。

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>*</small> 

<small></small>