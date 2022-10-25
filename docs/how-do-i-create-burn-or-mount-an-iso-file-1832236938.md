# 如何创建、刻录或挂载？ISO 文件？

> 原文：<https://lifehacker.com/how-do-i-create-burn-or-mount-an-iso-file-1832236938>

几年前，我终于做出决定，在组装新电脑时不再购买光驱，因为我已经不记得上次需要将光盘放入电脑是什么时候了。是的，有一天我可能还是会买一个 4K 播放器——一旦下一个 PlayStation 5 或 Xbox 什么的出现——但是我们现在生活在一个流媒体和可下载的世界里。制作一个可启动的 USB 驱动器很容易，甚至比从光盘安装东西(如 Windows 10)还要快。



然而，整个世界还没有远离光盘。而在这里为我们讲述更多相关问题的是本周的[**Tech 911**](https://lifehacker.com/c/tech-911)life hacker 读者 **Jim** :

> 我最近在 abandonware 网站上偶然发现了乐高象棋视频游戏，并下载了该游戏的软件包。它附带了四个 ccd、cue、img、sub 类型的文件。Img 看起来像是肉，因为它有 579 MB。下载本身被称为 ISO，所以我相信接下来我需要创建一个文件的实际 ISO。对于我可以使用的最新的、无膨胀软件的 windows 10 实用程序，有什么建议吗？

所以，你实际上并没有提到你打算用你想制作的 ISO 做什么——是将它刻录到物理光盘上，你当然可以这样做，还是你只是将它保存起来，并在需要时将其挂载到虚拟驱动器上。不管怎样，你都有很多选择，所以让我们从头开始。

通常，我希望光盘映像以. BIN 和. CUE 文件的形式出现。就你而言，既然你已经。CCD，。提示，。IMG 还有。子文件，这告诉我，整个软件包是使用一个名为 [**CloneCD**](https://www.redfox.bz/en/clonecd.html) 的 Windows 应用程序创建的。如果你打算烧掉你的。IMG 文件复制到物理光盘，我建议使用 CloneCD 来确保副本是完美的。该应用程序的试用/免费版本应该是你所需要的。

同样，如果您想将下载的文件挂载为光盘，可以安装 [**虚拟克隆驱动**](https://www.redfox.bz/en/virtual-clonedrive.html) (Windows)。对您的操作系统来说，这就像您在操作系统中拍打物理磁盘一样。这可以让你免去摆弄实际刻录过程的麻烦(这可能包括购买新的硬件和/或光盘)，并且安装游戏应该会快得多。

我会探索后者，因为你可以使用像[**ImgBurn**](http://www.imgburn.com/)(Windows)这样的工具来抓取并转换你的虚拟光盘为一个更通用的 ISO 文件，然后你可以在 Windows 或 Mac 系统上使用。(这可能对你的游戏不起作用，因为它可能只适用于 Windows，但这只是一个一般的观察)。

到目前为止，我一直在列出 Windows 应用程序，但对于那些在 Mac 上阅读本文的人来说，你应该能够使用 [**家酿**](https://lifehacker.com/how-to-make-your-own-bulk-app-installer-for-os-x-1586252163) 公式 [ccd2iso](http://rive.google.com) 将你所拥有的转换成 iso 文件。然后，您可以使用类似于 [**刻录**](http://burn-osx.sourceforge.net/Pages/English/home.html) 的应用程序将它刻录到光盘上，或者使用“磁盘工具”直接挂载它。

你也可以在 Windows 10 中直接安装 ISOs 这是转换你的图像的另一个原因，如果不为别的，只为处理更少的文件和一点额外的便利。

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>*</small> 

* * *

<small>*<small>更多来自 Lifehacker，一定要在 Instagram 上关注我们</small>*[*<small>@ lifehackerdotcom</small>*](https://www.instagram.com/lifehackerdotcom/)*<small>。</small>T15】*</small>

<small></small>