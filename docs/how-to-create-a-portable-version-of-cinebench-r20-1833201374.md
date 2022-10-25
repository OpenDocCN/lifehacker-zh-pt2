# 如何创建便携式版本的 Cinebench R20

> 原文：<https://lifehacker.com/how-to-create-a-portable-version-of-cinebench-r20-1833201374>

我很高兴读到上周 Cinebench R20 的发布。这是我说过的最令人讨厌的话之一，但这仍然是事实。这款免费的基准测试应用非常适合测试你的电脑，如果你想知道它的运行速度(以及它与其他系统相比的表现)。

Watch

也就是说，以前版本的 Cinebench (R15)附带了一个方便的 OpenGL 测试，您也可以使用它来评估系统的 GPU。这在 R20 中有所体现，它主要关注的是让你的 CPU 遭受痛苦。两个应用之间的分数是不可比的，因为它们使用不同的工作负载来测试你的系统。

当我最近在我的系统上运行这两个应用程序时，我的系统在 Cinebench R20 上的排名肯定高于 R15，但这很容易解释。旧的 Cinebench R15 将我的 CPU 与旧的处理器进行了比较，当时，我的系统还不算太差。然而，新版本有一个扩展的列表可供选择——当新的 AMD Threadripper 芯片让我老化的英特尔酷睿 i7-4790K CPU 相形见绌时，我注意到了这一点。

虽然我还没有找到一个巨大的用户 Cinebench R20 分数提交的公共数据库——就像这个方便的[Cinebench R15](https://us.rebusfarm.net/en/tempbench?view=benchmark)——如果你想将你的系统的性能 与其他系统(包括类似配置的系统)进行比较，你可以进入大量的 [论坛线程](https://linustechtips.com/main/topic/62476-post-your-cinebench-r2015r1152003-scores-over-1000-submissions/) 。

### 创建便携版的 Cinebench

Cinebench R20 的一个缺点是，它的开发者马辰决定通过微软的和苹果的 应用商店[提供该应用。虽然这不是要处理的最大问题，但这确实意味着您不能只下载可执行文件或。ZIP 文件，自己安装 app 你必须通过应用程序商店，这可能不是你喜欢(或想要)的获取应用程序的方式。](https://www.maxon.net/www.maxon.net/cb_r20_dl_ap)

没多久别人 [就黑进了一个便携版](https://www.techpowerup.com/253317/maxon-releases-cinebench-r20-benchmark) 的 Cinebench R20，没多久*的*让 Cinebench 的 [向那些提供下载的人发送法律威胁](https://www.techpowerup.com/253402/maxon-sends-legal-threats-to-pc-enthusiast-websites-hosting-portable-cinebench-r20-downloads) 。虽然您应该跟随他们的脚步，不要列出您为公共消费创建的可移植版本，但没有什么可以阻止您为自己创建一个在自己的系统上使用的版本。

我把重点放在这个应用程序的 Windows 版本上，因为我怀疑大多数 Mac 用户并不介意苹果的应用程序商店，因为 Windows 用户更喜欢微软的替代产品。是的，你必须从微软商店*下载到*创建一个便携版本(除非你使用像 [Adguard](https://store.rg-adguard.net/) 这样的网站来获取链接)，这击败了绕过微软商店的点，但至少你将能够在其他系统上使用你的便携版本。

下载应用程序后，启动它并打开 Windows 的任务管理器。寻找 Cinebench 列表，但不要右键单击它。如果您这样做，大多数选项将灰显。取而代之的是，左键点击列表左侧的箭头，这将弹出另一个 Cinebench 的*提及，位于第一个的下方。右键单击并选择“打开文件位置”*

现在你会发现自己在一个“bin”文件夹中，这个文件夹有一个很长的名字(以“MAXON”开头)).右键单击左侧边栏中的“bin”文件夹，选择“复制”，然后将该文件夹粘贴到 PC 上的其他位置。你现在有了一个便携式版本的应用程序，可以安装在任何你想要的 Windows 系统上，我通过卸载 Cinebench R20 的 Windows 应用程序版本并从新复制的“bin”文件夹中启动 Cinebench 可执行文件来进行测试。效果非常好。