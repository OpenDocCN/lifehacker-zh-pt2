# 如何检查您的 Windows 7 应用程序是否与 Windows 10 兼容

> 原文：<https://lifehacker.com/how-to-check-if-your-windows-7-apps-are-compatible-with-1841027283>

阻碍人们从 [升级他们(真的)过时的 Windows 7](https://lifehacker.com/quickly-upgrade-windows-7-to-windows-10-for-free-with-t-1840843214) 版本的最大问题之一是应用兼容性。如果你有一些超级特定的应用程序不能在 Windows 10 上运行，这是坚持使用不太安全的操作系统的最好理由。这可能不是 T4 正确的举措，但却是必要的举措。

Watch

但是，如果你*假设*你的应用不能在 Windows 10 中运行，那你就没有帮到自己最大的忙。是时候放手一搏了——不是升级和抱最好的希望，而是试用 Windows 10，看看你的日常应用是否如你所愿。如果他们这样做了，而且你的系统硬件 [足够好运行 Windows 10](https://support.microsoft.com/en-us/help/4028142/windows-10-system-requirements) ，你有义务为你的系统安全切换。

这个计划的关键是找到一种方法来*使用* Windows 10，而不是用 Windows 10 替换你的 Windows 7。虽然有几个选项可以使用，但我将坚持使用一个相当好的选项:免费虚拟机。

(我原本打算写一篇文章，向你展示如何创建一个 Windows 10 的活动 USB 版本，你可以启动并摆弄它，但我根本无法让这个过程工作*。我试过 WinToUSB 我试过鲁弗斯。我试着弄乱各种 BIOS 设置。我最终放弃了，因为如果我花了几个小时来解决这个问题，如果有更简单的方法，我不想向您推荐。)*

### *为什么要有虚拟机，我在哪里可以获得虚拟机？*

*你可以为一系列不同的平台下载一个免费的 Windows 10 虚拟机——VirtualBox、VMWare、Parallels 和 Hyper-V(仅举几个例子)——而且几乎不需要你进行任何设置。这是在你的系统上安装并运行某个版本的 Windows 10 的一种快速、简单的方法，而且你完全不用花钱。有什么不喜欢的？*

*嗯，有一点——性能。如果你仍然坚持使用你第一次安装的 Windows 7，很可能你的系统不是顶级的游戏装备。你需要至少 1-2GB 的内存 [来运行 Windows 7](https://support.microsoft.com/en-us/help/10737/windows-7-system-requirements) ，你可能还需要至少 1-2GB 的内存来运行虚拟化版本的 Windows 10。你还需要额外的 20GB 左右的硬盘空间来存储二级操作系统。希望你有一个相当快的处理器。但即使你没有，那也没关系；只要 Windows 10 *运行*，你就可以检查一个有问题的应用是否会加载。*

*要开始这一旅程，你需要准备两件东西:[**VirtualBox**](https://www.virtualbox.org/)，以及微软的一台用于 VirtualBox 的 Windows 10 虚拟机。现在，微软*使用*为 Windows 10 提供各种有时间限制的虚拟机，但似乎 [他们现在已经削减回 Windows 7](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)(*meh*)。我想你可以抓住其中的一个，简单地在虚拟机内升级到 Windows 10，但这不会比使用微软现有的工具更容易。ISO 和 [自己把那个装在虚拟机里](https://lifehacker.com/how-to-set-up-a-virtual-machine-for-free-1828969527) 。*

*相反，浏览到这个*其他*微软网站，抓取该公司的虚拟机 [Windows 10 企业版](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines) 。不要让名字把你难倒；它会附带许多你不需要的功能。我们所做的只是检查应用程序的兼容性，而不是试图在小型企业环境中部署 Windows。*

*您还需要检查您的 CPU 是否支持虚拟化；如果没有，您可以继续取消(或删除)这些下载。在 Windows 控制面板中调出 System，注意列出的是哪种处理器，并进行快速网络搜索，看看是否可以用它来运行虚拟机。(如果是这样，您可能还需要 [检查您系统的 BIOS](https://bce.berkeley.edu/enabling-virtualization-in-your-pc-bios.html) 以确保您已经启用了所有虚拟化设置，默认情况下可能是关闭的)。*

### *在 VirtualBox 中设置 Windows 10(企业版)*

*一旦你的 16GB 文件下载完成，解压存档。您现在将看到一个以“WinDev”开头、以扩展名. OVA 结尾的文件。双击它以将其加载到 VirtualBox 中。您将会看到一个如下所示的屏幕:*

*点击“导入”开始，在等待系统~~运行~~来导入你下载的虚拟机时，做些别的事情。完成后，您将在 VirtualBox 的主屏幕上看到该列表。通过点击突出显示它，然后点击“设置”*

*这里有很多选项可供你选择。最关键的可以在你的系统选项卡中找到，在这里你可以设置你的虚拟机应该使用多少内存(坚持滑块的绿色部分)和应该使用多少 CPU 核心。这通常是性能的两个最重要的设置，我喜欢在不破坏运行它的系统(我的常规桌面)的情况下尽可能多地给我的虚拟机设置。在一切都变得尽善尽美之前，你可能会尝试一下这些值。*

*您可以更改其他设置，如在您的主机和虚拟机之间设置共享剪贴板，以及文件夹共享。我喜欢开门见山，只需要你点击 VirtualBox 主屏幕上绿色的“开始”按钮。一旦你这样做了，Windows 应该会启动，你可以开始下载(或复制)任何你想在 Windows 10 中测试的应用程序。完成实验后，可以随意删除虚拟机(及其数据)来释放一些空间。*