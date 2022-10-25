# 检查您的华硕电脑是否受到“影子锤子”恶意软件攻击的影响

> 原文:[https://life hacker . com/check-if-your-ASUS-computer-is-the-affected-by-1833580162](https://lifehacker.com/check-if-your-asus-computer-is-among-those-affected-by-1833580162)

如果你有一台华硕电脑，你会想检查你的设备是否受到最近“影子锤子”恶意软件攻击的影响。

Watch

你可能已经看过关于恶意软件 的令人担忧的头条新闻，但是对于那些不了解最新情况的人来说，这里是交易。最近一轮恶意软件通过利用华硕为其产品部署软件更新的方法，已经侵入了超过 57，000 台华硕电脑和笔记本电脑。这个数字来自于在线安全公司卡巴斯基 [最近发布的概述](https://securelist.com/operation-shadowhammer/89992/) ，该公司一直在调查此次攻击。该报告详细调查了攻击是如何进行的，以及为什么这些方法会引起如此多的关注。

卡巴斯基的报告还包括该公司为华硕用户开发的一个工具，用于检查他们的设备是否受到恶意软件部署的影响。只需几秒钟就能看到你的设备是否在攻击中受到了的攻击。

1.  点击卡巴斯基 [SecureList 文章](https://securelist.com/operation-shadowhammer/89992/) 中的“用工具下载档案”链接，下载“shadowhammercheck.zip”
2.  将文件解压缩到您喜欢的位置
3.  打开解压后的“shadowhammercheck”文件夹，运行 shadowhammercheck
4.  该程序将在你的电脑上进行测试，并几乎立即给你结果。

华硕还发布了一款诊断工具，供用户检查他们的电脑是否感染了恶意软件，它的工作方式类似于卡巴斯基的工具。

1.  从华硕下载“ASDT_v1.0.10.zip”
2.  解压缩文件
3.  打开文件并运行“ASDT.exe”
4.  将弹出一个诊断对话框

你也可以使用卡巴斯基的在线 Shadowhammer 工具来检查你的系统是否在目标列表中，但是你需要知道你电脑的 MAC 地址。

1.  打开命令行终端。按下 **Windows 键+R** ，搜索“cmd”，并点击 enter。
2.  在命令行中，键入**“ipconfig/all”**并点击**回车**
3.  你会得到几行信息。找到所有写着**“物理地址:**的行，然后记下物理地址行后面的十六进制数字串——这些串就是您的 MAC 地址。你可以在上面的截图中看到一个例子。
4.  记下每个 MAC 地址
5.  接下来，打开 [卡巴斯基的影锤诊断](https://shadowhammer.kaspersky.com/) 页面，将每个 MAC 地址复制到搜索栏，点击**“立即检查”**对每个 MAC 地址重复上述步骤。

如果你的任何 MAC 地址返回肯定，你需要采取行动，找到并消除恶意软件，第一步是为自己配备一个可靠的防病毒程序。

事实上，即使一个应用程序或网站没有表明你在的“目标名单”上，运行一次全面的防病毒扫描也无妨(以防万一)。虽然有很多 [优秀的高级选项](https://www.tomsguide.com/us/best-antivirus,review-2588.html) ，但也有很多有能力的 [免费杀毒和反恶意软件程序](https://www.tomsguide.com/us/best-free-antivirus,review-6003.html) ，包括 Windows Defender，可以帮你清除任何影锤的痕迹。

你还会想把 [华硕的【Live Update app 更新到最新版本(V3.6.8 或更高版本)](https://www.asus.com/support/FAQ/1018727/) ，第一时间关闭了允许影子锤子利用的安全漏洞。就像安装一个反病毒/反恶意软件解决方案一样，这个 u pdate 强烈推荐给那些没有被 Shadow Hammer 攻击的用户。