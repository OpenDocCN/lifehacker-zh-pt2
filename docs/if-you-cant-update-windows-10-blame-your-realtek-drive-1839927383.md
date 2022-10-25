# 如果你不能更新 Windows 10，那就怪你的 Realtek 驱动程序

> 原文：<https://lifehacker.com/if-you-cant-update-windows-10-blame-your-realtek-drive-1839927383>

这里有一个好消息:如果你有一段时间没有更新你的 Realtek 蓝牙驱动程序，或者甚至不知道这是一件事，你终于可以更新到 Windows 10 版本 1909-截至我们发表这篇文章时，该操作系统的最新和最大的迭代。



据 [哔哔声电脑](https://www.bleepingcomputer.com/news/microsoft/microsoft-removes-windows-10-1909-realtek-driver-update-block/) 报道，微软已经移除了阻止你升级到这一版本，甚至是 Windows 10 版本 1903 和 1809 的障碍，原因是你的旧 Realtek 驱动程序导致新版本操作系统上的设备连接出现问题。

不管那个问题是什么，现在已经用 Realtek 的驱动程序的更新版本解决了。理论上，你*应该*能够通过 Windows Update 本身更新到这些软件的最新版本——1 . 5 . 1012 版或更高版本。您可以通过打开设备管理器，展开蓝牙部分，右键单击并选择“属性”，然后单击驱动程序选项卡来查看您正在运行的内容:

如果您运行的是较旧的驱动程序，并且没有可通过 Windows Update 获得的更新，您可以尝试手动安装 Realtek 的蓝牙驱动程序。这看起来是一个非常复杂的过程，但是你会没事的。正如微软 [对](https://support.microsoft.com/en-us/help/4529832/updating-to-windows-10-version-1903-on-devices-with-some-driver-versio) 的描述:

> 1.  *Download two drivers of Realtek Bluetooth radio station to your preferred folder:* [*driver 1*](http://download.windowsupdate.com/d/msdownload/update/driver/drvs/2019/01/f2748416-7753-49c6-9185-56f4986f490b_e98e0d664b7e874011b8e3752046ca61f3475295.cab) *,* [*driver 2*](http://download.windowsupdate.com/c/msdownload/update/driver/drvs/2018/11/068de0d6-6ac2-473a-8cbd-bd449cd5c97c_942eec5828662eecc6b98cc2706658bf2433717c.cab) **Note** We suggest downloading them to your **document** folder.
> 2.  *Open the **file browser** . If there is no file browser icon in the taskbar, select the search box, enter **file browser** and select it.*
> 3.  *In the **file browser** , go to the **document** folder or the folder where you downloaded the driver.*
> 4.  *找到并双击或双击名为 **068 德 0d 6-6a C2-473 a-8 CBD-BD 449 CD 5c 97c _ 942 EEC C5 828662 eecc 6b 98cc 2706658 BF 2433717 c . cab**T3】*
> 5.  *Select **Ctrl** + **A** This should select all files*
> 6.  *Right-click or long-press any file and select **to extract** .*
> 7.  *Select **New Folder** button and rename it **Realtek Bluetooth** .*
> 8.  *Select **and select** button.*
> 9.  *In the **file browser** , select the **back** button to go to the location where you downloaded the driver.*
> 10.  *Find and double-click or double-click the name **f2748416-7753-49c6-9185-56f4986f490b _ e98e0d664b7e874011b8e3752046ca61f3475295.cab***
> 11.  *Select **Ctrl 【T92】 This should select all files***
> 12.  *Right-click or long-press any file and select **to extract** .*
> 13.  *If you are in a folder named **Realtek Bluetooth** , then select **New Folder** button and type **Realtek Bluetooth 2** .*
> 14.  *Select **and select** button.*
> 15.  *In the search box of the taskbar, enter **device manager** , and then select **device manager** .*
> 16.  *Find **Bluetooth** and expand it.*
> 17.  *Find the Realtek device, right click or long press.*
> 18.  *Select **to update the driver** from the context menu.*
> 19.  *Select **to browse my computer for driver software** button.*
> 20.  *It should default to your **document** folder. If this is where you save the driver, then just select **and the next** button. If you don't save the driver to your **document** folder, select **Browse** button and find the folder where you downloaded the driver, then select **OK***
> 21.  *Now you should be able to find the updated drivers and install them. Wait for this operation to complete, and select **to close** .*

一旦你做到了这一点，当你等待 Windows 10 更新到最新版本时，请随意思考提神饮料。然而，我不会开始倒它，直到你确认更新已准备好下载和安装；微软表示，在你更新完蓝牙驱动程序后，Windows update 可能需要 48 小时左右才能发布。