# 如果你的 Mac 无法更新到 Windows 10 版本 1903，该怎么办

> 原文：<https://lifehacker.com/what-to-do-if-your-mac-wont-update-to-windows-10-versio-1836048960>

在 Mac 上运行 Windows 要比在 Windows 机器上运行 macOS 容易得多，但这并不意味着这种疯狂的混合环境总是完美的。微软最近发布了一个公告，解释了为什么如果你试图在 Boot Camp 版本的操作系统上更新到 Windows 10 (1903)的最新版本 [时可能会遇到一些问题。](http://Editor-in-Chief for Cloud)

Watch

简短的回答？你的 Mac 真的很旧了。正如微软所描述的:

> *“2012 年之前的 Mac 设备或装有旧的 Apple Boot Camp 或 Windows 支持软件驱动程序的新款 Mac 设备具有兼容性[原文如此],无法更新到 Windows 10 版本 1903。具体来说，Windows\system32\drivers 中 MacHALDriver.sys 日期为 2011 年 9 月 24 日 01:57:09 或更早的设备会受到影响。*

当你更新 Windows 10 并看到类似这样的通知时，你就会知道你遇到了这个问题:

要解决这个问题，你有几个选择。首先，你要确定你运行的是最新版本的 macOS，包括 Boot Camp 的更新。(如果你不在 [macOS Mojave](https://lifehacker.com/what-you-need-to-know-before-and-after-installing-mac-1829271754) 上，也许是时候尝试一下了。或者，如果你够大胆，你甚至可以试着跳到 [马科斯·卡特琳娜](https://lifehacker.com/the-safest-way-to-install-the-macos-catalina-beta-1835836662) 。)之后再考虑重装 Boot Camp 自带的 [Windows 支持软件](https://support.apple.com/en-us/HT208495) 。

如果这不能解决问题——鉴于目前为止我看到的关于这个问题的所有讨论，我怀疑这不会解决问题——你*可能*能够干净地安装 Windows 10 版本 1903。使用微软的 [媒体创作工具](https://www.microsoft.com/en-ca/software-download/windows10) 建立一个新的。ISO，看看你能不能用这种方法重新安装一个新的 Boot Camp 版本的 Windows。(当然，你会想在走这条路之前备份你所有的文件，因为你会想安装一个干净的 Windows 10 版本。)

即便如此，这一步 [可能会比其他任何事情引起更多的问题](https://www.reddit.com/r/macpro/comments/bsaour/psa_windows_10_1903_update_may_brick_your_windows/) 。

相反，我建议尝试的是从([镜像](https://mega.nz/#!TrIhmQqA!bPX5u934PCjRHq5TOcpwiPHOV_sMIrUeKGUDVo37pTY) )非官方来源抓取一个更新的 Mac HAL 驱动程序——machardriver . sys，将 Windows 10 引导至安全模式，并用这个新文件覆盖旧文件。你会在`c:\Windows\System32\`中找到旧的 machaldriver.sys，替换它可能需要你将原始文件重命名为类似 machaldriver.bak 的文件，然后你需要重启系统，等待 Windows 10 启动，然后将新文件复制到你的\System32\目录中。

否则，你可以等到 7 月下旬，让微软来解决这个问题，但这并不好玩。替换。SYS 文件应该可以让你顺利使用 Windows 10 版本 1903。