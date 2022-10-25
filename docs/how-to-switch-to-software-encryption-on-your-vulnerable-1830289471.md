# 如何在易受攻击的固态硬盘上切换到软件加密

> 原文：<https://lifehacker.com/how-to-switch-to-software-encryption-on-your-vulnerable-1830289471>

荷兰拉德布大学的研究人员发现了几个使用基于硬件的加密的固态硬盘的严重安全问题——这些漏洞允许攻击者在不需要解密密码的情况下访问硬盘的“加密”内容。

Watch

首先，这里列出了受影响的驱动器:

*   关键的 MX100、MX200 和 MX300 内部固态硬盘

*   三星 T3 和 T5 外置固态硬盘

*   三星 840 EVO 和 850 EVO 内置固态硬盘

你可以阅读 [一份研究人员发现的详细报告，其中列出了每个硬盘型号](https://www.ru.nl/english/news-agenda/news/vm/icis/cyber-security/2018/radboud-university-researchers-discover-security/) 的具体漏洞。

然而，乐趣并没有就此结束。运行受影响驱动器之一的用户可能会认为微软的 BitLocker 工具(Windows 10 Pro 的标准配置)会通过其基于软件的加密来解决问题。BitLocker 甚至可能会说，上述列表中的一个 SSD 是加密的。事实证明，事实并非如此。

相反，当 BitLocker 注意到 SSD 提供基于硬件的加密时，它会默认使用这种加密，而不是 BitLocker 的软件加密。如果你使用的是上述驱动器之一，BitLocker 会假设你的驱动器是加密的，而实际上它是非常容易受到攻击的(如果有人可以物理访问它)，这就大大降低了你的安全性。

三星和 Crucial 都发布了固件更新来解决固态硬盘的这些问题——你应该现在就安装它们——但即使是三星 [也建议](https://www.samsung.com/semiconductor/minisite/ssd/support/consumer-notice/) 用户也使用第三方软件加密他们的数据。我们对此有一些建议，但首先，这里是如何检查您的固态硬盘使用的加密类型:

### 如何检测您的驱动器是否在 Windows 上使用硬件或软件加密

首先，打开提升的命令提示符。你可以在 Windows 任务栏的搜索框中输入“cmd ”,但不要按 enter 键。等待“命令提示符”出现在搜索结果中，然后右键单击它并选择“以管理员身份运行”应该会打开一个名为“管理员:命令提示符”的命令提示符窗口

在提升的命令提示符窗口中，键入`manage-bde.exe -status`并按 Enter 键。

你将会看到一个你系统的驱动器列表和它们使用的加密类型(如果有的话)。如果您正在使用上述任何受影响的驱动器，并且它被列为使用软件加密，那么您就没有潜在的安全风险。然而，如果它们中的任何一个使用了硬件加密，那么你就容易受到攻击。在这种情况下，我们需要将加密方法更改为实际可行的方法。

### 如何强制 BitLocker 的软件加密

[微软表示](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/ADV180028) 虽然 BitLocker 默认依赖于驱动器的硬件加密，但也有可能强制驱动器使用 BitLocker 的软件加密。为了改变加密方法，你不必重新格式化你的驱动器，也不必重新安装任何应用程序(尽管 Radboud 研究人员的原始报告中有矛盾的信息)。

首先，您需要 [更改 BitLocker 的组策略设置。](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/jj679890(v=ws.11)#configure-use-of-hardware-based-encryption-for-fixed-data-drives) 要打开组策略编辑器，在任务栏搜索框中键入“组策略”，然后单击组策略编辑器。在编辑器中，转到**计算机配置>管理模板> Windows 组件> BitLocker 驱动器加密。**

在**固定数据驱动器下，**双击**“为固定数据驱动器配置使用基于硬件的加密”，**，然后单击**“编辑”**将选项设置为**“禁用”**，然后点击**应用**。对操作系统驱动器和可移动数据驱动器文件夹中名称相似的选项重复这些步骤。

接下来，我们必须通过禁用和重新启用 BitLocker 来解密和重新加密驱动器。在 Windows 资源管理器中，打开**“这台电脑”，**右键点击驱动器，点击**管理 BitLocker**将弹出一个控制面板窗口，列出您系统的驱动器，以及打开或关闭 BitLocker 的选项。

根据驱动器上存储的数据量，解密过程可能需要几个小时才能完成。重新启用 BitLocker 后，将使用 BitLocker 的软件加密对驱动器进行加密。与前一步一样，这可能需要一段时间，具体取决于驱动器的大小，但一旦完成，您的驱动器将得到完全和适当的保护。

### 使用第三方软件

如果你不信任 BitLocker，没有 BitLocker，或者不是 Windows 用户，但仍在寻找加密受损的 Samsung 或关键硬盘的方法，最好的选择是使用第三方软件加密。

有许多第三方替代品可用。Radboud 的研究人员建议消费者使用已经流行多年的免费开源加密软件。也有优秀的付费产品，如 [文件夹锁](https://download.cnet.com/Folder-Lock/3000-2092_4-10063343.html)(40 美元)，以及 [AxCrypt](https://www.axcrypt.net/) (免费，高级版 36 美元，商务版 90 美元)，这些产品通常提供客户支持、Mac 支持，以及物有所值的特殊功能或额外安全插件。