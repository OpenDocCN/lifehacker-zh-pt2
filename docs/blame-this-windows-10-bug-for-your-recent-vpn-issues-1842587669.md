# 将你最近的 VPN 问题归咎于这个 Windows 10 的错误

> 原文：<https://lifehacker.com/blame-this-windows-10-bug-for-your-recent-vpn-issues-1842587669>

如果你的 Windows 台式机或笔记本电脑出现了网络连接问题——你已经排除了用户错误或 [糟糕的无线连接](https://lifehacker.com/why-does-my-work-laptop-have-slower-wifi-than-my-other-1842489912)——微软可能是罪魁祸首的可能性很小。有一个影响用户使用代理或 VPN 连接的错误，它严重到足以保证微软发布一个非计划更新来修补这个问题。



正如微软最初 [描述的](https://docs.microsoft.com/en-us/windows/release-information/status-windows-10-1903#406msgdesc) :

> *使用手动或自动配置代理的设备，尤其是使用虚拟专用网络(VPN)的设备，可能会在通知区域的网络连接状态指示器(NCSI)中显示受限或无互联网连接状态。这可能在连接或断开 VPN 时发生，或者在两者之间改变状态后发生。存在此问题的设备在使用使用 WinHTTP 或 WinInet 的应用程序访问互联网时也可能会出现问题。在这种状态下，设备上可能受到影响的应用程序示例如下，但不限于 Microsoft Teams、Microsoft Office、Office365、Outlook、Internet Explorer 11 和某些版本的 Microsoft Edge。*

不过，这里有个问题:微软让你来决定你是否需要紧急更新。如果您的网络连接问题*听起来*像微软描述的那样，那么您可能需要考虑安装带外更新来修复该问题。以下是所有不同的更新及其适用的各种 Windows 版本:

*   Windows 10，版本 1909 ( [KB4554364](https://support.microsoft.com/help/4554364) )
*   Windows 10，版本 1903 ( [KB4554364](https://support.microsoft.com/help/4554364) )
*   Windows 10，版本 1809 ( [KB4554354](https://support.microsoft.com/help/4554354) )
*   Windows 10，版本 1803 ( [KB4554349](https://support.microsoft.com/help/4554349) )
*   Windows 10，版本 1709 ( [KB4554342](https://support.microsoft.com/help/4554342) )

要安装更新，只需访问 [微软的更新目录](https://www.catalog.update.microsoft.com/) 并寻找适合您的 Windows 版本的正确更新(或者点击其中一个“KB”链接并滚动到底部，以找到该特定更新的更新目录的链接，如果您不想手动搜索)。很有可能你需要 x64 (64 位)或 x86 (32 位)系统的更新，你可以通过点击开始菜单并调出**设置>系统>关于:**来检查你有哪一个

如果你不想手动更新，你最好坚持下去。考虑到这个问题的严重性，我相信微软会很快将这个补丁更新到一个更大的 Windows 更新中。