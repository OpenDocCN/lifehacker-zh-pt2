# 如何防范新的 macOS 安全漏洞

> 原文：<https://lifehacker.com/how-to-protect-yourself-from-the-new-macos-security-vul-1835845551>

Mac 用户注意了:据报道，最近披露的 macOS Gatekeeper 中存在的一个漏洞——也被称为“Cavallarin”漏洞——已被广告软件创作者利用。正是在这样的时候，我们想起了保护你的 Mac 免受此类问题影响的最佳建议:当有疑问时，从 Mac 应用商店或受信任的第三方来源安装应用程序，而不只是你在互联网上找到的任何旧东西。



### 卡瓦拉林漏洞利用的工作原理

macOS Gatekeeper 会检查所有安装的应用程序，以确认它们是 Apple 认证的应用程序。如果应用程序没有收到苹果的“全部清除”，看门人将停止安装并通知用户。你仍然可以安装你的应用程序，你只需要明确地确认安装——换句话说，一个“你真的想这样做吗？”检查苹果的部分。

安全研究人员菲利普·卡瓦拉林(因此该漏洞名称的“卡瓦拉林”部分)发现，看门人对“可信”应用程序的标准 [有一个严重的缺陷](https://www.fcvl.net/vulnerabilities/macosx-gatekeeper-bypass) ，允许不可信的应用程序欺骗看门人给他们一张免费通行证。由于 Gatekeeper 将来自外部驱动器和网络共享的安装列入白名单，因此攻击可能是这样进行的:

> *“攻击者创建一个 zip 文件，其中包含一个指向她/他控制的自动挂载端点的符号链接(例如 Documents->/net/evil . com/Documents)，并将其发送给受害者。*
> 
> *受害者下载恶意存档文件，提取它并跟随符号链接。*

> 现在，受害者处于攻击者控制的位置，但受到网守的信任，因此任何攻击者控制的可执行文件都可以在没有任何警告的情况下运行。寻路器的设计(例如隐藏。应用程序扩展，隐藏标题栏的完整路径)使得这种技术非常有效，很难发现。"

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-m74cpadIPZY&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-m74cpadIPZY&start=0) 

卡瓦拉林在几周前发现了旁路，并给了苹果 90 天的时间来修复它。苹果公司没有回应，因此卡瓦拉林在 5 月 24 日披露了这一漏洞。即使在公开披露之后，苹果仍然没有解决这个问题，现在 [Intego](https://www.intego.com/mac-security-blog/osx-linker-new-mac-malware-attempts-zero-day-gatekeeper-bypass/) 的恶意软件研究团队已经看到了网守漏洞利用的初步迹象出现在网上。

Intego 跟踪了 4 个在 7 月 6 日上传到 Virustotal 的恶意软件样本，每个磁盘镜像都指向同一个链接服务器上的潜在恶意应用程序。后来确定这些是早期测试——针对现在称为“OSX/链接器”的恶意软件 Intego 团队怀疑它们是由 OSX/Surfbuyer 恶意软件背后的同一批开发人员进行的。

虽然“测试”在这一点上听起来不太可怕，但 Intego 安全分析师 Joshua Long 指出，这一漏洞的性质为更糟糕的情况敞开了大门:

> *...因为。磁盘映像中的应用程序是动态链接的，它可以在服务器端随时更改，而根本不需要修改磁盘映像。因此，相同的磁盘映像(或从未上传到 VirusTotal 的更新版本)可能后来被用来分发一个在受害者的 Mac 上实际执行恶意代码的应用程序。*

### 如何防止 Mac 上潜在的 Cavallarin 漏洞

在这一点上，最简单的预防方法是首先坚持使用苹果认证的应用程序，并对你从陌生来源下载的应用程序保持合理的怀疑。目前还不清楚苹果在 macOS 中修补这个漏洞可能需要多长时间。

Intego 的 premium[virus barrier X9](https://www.intego.com/mac-protection-bundle)和 [Flexivity](https://www.intego.com/business/flextivity-secure) 反病毒程序已经将操作系统/链接器威胁添加到它们的注册表中，并且您还可以使用免费的[virus barrier scanner](https://www.intego.com/virusbarrier-scanner)来检查您的系统是否存在与该漏洞相关的任何已知威胁。这些将在检测到的威胁下显示为“OSX/链接器”Intego 要求被感染的用户通过他们的 [在线提交表格](https://support.intego.com/hc/en-us/requests/new) 与他们联系。

您还可以为您的系统研究其他预防方法，但这些方法风险更大，因为它们需要禁用和编辑关键的 macOS 安全措施。您可以 [查阅 Intego 关于 Cavallarin exploit](https://www.intego.com/mac-security-blog/osx-linker-new-mac-malware-attempts-zero-day-gatekeeper-bypass/) 的博客文章了解更多信息，但我们建议您只是练习更安全的在线习惯。如果您对将要安装到您的计算机上的内容有任何疑问，请在继续之前对其进行快速病毒扫描。