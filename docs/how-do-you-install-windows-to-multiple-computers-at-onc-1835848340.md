# 如何一次给多台电脑安装 Windows？

> 原文：<https://lifehacker.com/how-do-you-install-windows-to-multiple-computers-at-onc-1835848340>

在本周的 [**Tech 911**](https://lifehacker.com/c/tech-911) 建议专栏中，一位 Lifehacker 读者想要自动化一个 otherwis e 耗时又烦人的过程:安装一个全新的 Windows(大概是， Windows 10)。有什么问题吗？他们不想只在一个系统上安装操作系统。

Watch

Lifehacker 读者**比利**写道:

> “我如何从一个中心点在其他八台电脑上安装 Windows？”

我怀疑大多数人家里都没有八个 Windows 系统，它们都需要一个全新版本的操作系统。然而，你可能有两台:一台台式机和一台笔记本电脑。你的配偶可能有两台:另一台台式机和一台笔记本电脑。也许你的孩子也有台式机或笔记本电脑。

电脑越来越多，如果你是一个(不值得羡慕的)负责管理家里所有系统的更新、故障排除和重新安装的人，那么有一天你会想把所有事情都一起做的想法并不疯狂。

最简单的方法是使用[**Windows Media Creation Tool**](https://www.microsoft.com/en-us/software-download/windows10)在一个(或几个)闪存驱动器上安装一个 Windows 10 映像，并使用这些映像来安装操作系统。除非你说的是另外八台相距甚远的电脑，否则在一台电脑上安装操作系统，同时在另一台电脑上运行基本的配置步骤，应该不会造成太大的负担。

假设所有这些系统都是相同的，您还可以设置和配置*一个*(不激活 Windows)[镜像驱动器](https://lifehacker.com/back-up-and-clone-your-hard-drive-with-macrium-reflect-1825289970) ，然后将该镜像克隆到其他系统的驱动器上。我没有做过这个过程，但我知道您必须运行 Windows 的' [Sysprep](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/audit-mode-overview) 工具—可通过审计模式获得—以首先 [概括映像](https://www.tenforums.com/tutorials/3020-customize-windows-10-image-audit-mode-sysprep.html) (这将允许您为每台机器拥有一个唯一的计算机安全标识符，或" [SID](https://blogs.technet.microsoft.com/markrussinovich/2009/11/03/the-machine-sid-duplication-myth-and-why-sysprep-matters/) )。然后你需要 [捕捉图像](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/capture-and-apply-windows-using-a-single-wim) 并使用它在你的其他系统上克隆 Windows。

我可能会做的是直到该段的“捕捉图像”部分的所有事情。然后，我会使用类似 Clonezilla 的工具—[](https://clonezilla.org/clonezilla-live.php)**【Clonezilla Live】，技术上来说—对驱动器进行镜像，并将该镜像克隆到您的其他系统上。我相信，当你打开这些系统时，你就可以启动普通版本的 Windows 10 了。(至少，这是 Josh 尝试并记录过程时的经历。)**

**同样，由于只有八个系统需要处理，您在这方面花费的时间可能等于(或大于)通过闪存驱动器进行手动安装的时间。但是让我们继续。还有另外两种选择，你可以试着从*的一个集中点*(我猜是另一台电脑)在其他系统上安装 Windows。**

**Clonezilla 有 [一个服务器版](https://clonezilla.org/clonezilla-SE/) 你可以玩(作为 Live CD)，你可以用它把 Windows 安装到联网系统上。如果我是正确的，Live CD 只适用于一对一的安装，而不是一对多。我假设您对前一种设置没有问题，因为如果您希望将 Windows 并发部署到多个系统，您需要在 Linux 桌面上安装和配置 Clonezilla 的服务器版。(你还需要确保你的客户端机器支持通过 BIOS 进行 [网络引导](https://networkboot.org/fundamentals/) ，否则整个过程就白费了。)**

**如果你有困难，或者你想要替代方案，你可以尝试使用[](https://fogproject.org/)**或 [**克隆策略**](http://clonedeploy.org/) 。我喜欢 CloneDeploy，尤其是因为它的文档 [很容易理解——你需要做一些阅读来正确地设置一切。您还可以使用 Live CDs 或闪存驱动器来设置您的客户端(接收 Windows 的系统)，如果网络引导过程(PXE)过于混乱，这将非常有用。](http://clonedeploy.org/docs/)****

****就是这样。这是一个复杂的过程，但对于一个人来说，通过一点点研究(和反复试验)就可以完成。完成所有这些工作后，抵制在简历的技能部分添加“专业 IT 人员”的冲动，尽管这可能很诱人。****

* * *

*****<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>****

****<small></small>****