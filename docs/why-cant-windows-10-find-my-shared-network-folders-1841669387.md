# 为什么 Windows 10 找不到我的共享网络文件夹？

> 原文:[https://life hacker . com/why-cant-windows-10-find-my-shared-network-folders-1841669387](https://lifehacker.com/why-cant-windows-10-find-my-shared-network-folders-1841669387)

在网络上的两台计算机之间共享文件夹总是让人觉得麻烦而不值得。至少，不能保证这个过程会顺利进行，而且当你解决了正在发生的任何问题，建立了你的共享，并传输了文件，那么，你还不如把它们复制到一个外部硬盘驱动器(或闪存驱动器)上。

Watch

如果您要传输的内容太大，闪存驱动器无法容纳，并且您没有外置硬盘，那么是时候咬紧牙关处理网络共享了。准时来了，生活黑客读者**罗杰**带着本周的 [**Tech 911**](https://lifehacker.com/c/tech-911) 问题:

> *MS 放弃了对“家庭组”的支持。我放弃了以太网的支持。两台机器；Win64 & Win32。使用热点的无线 ISP。两台机器都被 hotspot 识别。Win64 看不到 Win32 上的共享。Win32 看到 Win64 上的所有共享。两台机器都使用 USB 无线网络适配器*
> 
> 为了让 Win64 能够看到 Win32，我需要做些什么？？？"

我承认，我从来没有在家里使用过 wifi 热点，所以我的第一反应是检查一下它的设置，确保没有任何东西会干扰你的系统互相查看的能力。但是，如果一个(x86)可以看到另一个(x64)的所有共享，那么这听起来更像是 Windows 配置问题，而不是网络问题。

你没有提到你用的是什么版本的 Windows，所以我假设是 Windows 10。(毕竟 Windows 10 没有 Homegroups，所以感觉这是一个合理的猜测。)

要开始进行故障诊断，我会首先探索您在 32 位 Windows 系统(x86)上的共享设置。拉起**控制面板**，将视图从“类别”改为大图标或小图标，点击“网络和共享中心”然后，点击左侧边栏上的“更改高级共享设置”。

在此屏幕中，确定您已经打开了网络发现(和联网设备的自动设置)，以及文件和打印机共享。

点击“所有网络”菜单，考虑启用公共文件夹——顾名思义，网络上的任何人都可以看到它们。如果您让其他人进入您的网络，这是一个安全问题，因为他们也能够查看这些文件夹中的任何内容，但是如果只有您一个人(或者如果您只是在系统之间设置一个临时文件传输)，这应该不是一个问题。

请注意“密码保护共享”选项。我假设当您试图从 64 位系统访问它时，您是用 32 位系统的用户帐户和密码登录的。如果您尝试以单独的特定用户身份登录，您需要首先禁用此选项。

保存您所做的任何更改，返回到您的控制面板，并调出您的系统属性。两台电脑应该使用同一个工作组，可能称为“工作组”如果没有，请单击“高级系统设置”，然后单击“计算机名”选项卡，并修复它。

接下来，在 x86 系统上打开文件资源管理器。导航到要共享的文件夹，右键单击它，然后选择属性。从那里，点击共享标签。

接下来，单击“共享”按钮。在出现的屏幕中，您将看到允许访问共享的人员(用户)列表。一个应该是您登录的当前用户，另一个应该是“系统”

同样，当出现提示时，您需要以 x86 系统上的用户身份登录，否则您将无法实际访问任何共享文件夹。

如果你愿意稍微开放一下你的共享，可以考虑点击下拉菜单选择“所有人”，点击“添加”，然后授予“所有人”对该文件夹的读/写权限。我发现这通常可以解决我在 Windows 中共享文件夹时遇到的大多数问题，尽管这意味着网络上的任何人都可以访问该文件夹，而无需以任何人的身份登录。

单击“共享”按钮完成操作，然后确保复制并粘贴您看到的网络地址:

现在，启动 64 位 PC 并启动文件资源管理器。点击底部的网络，看看是否有任何东西出现。如果没有，你可能只需要在地址栏中手动输入以前的地址，这应该(希望)会弹出你的网络共享。

如果你仍然看不到任何的东西，并且你厌倦了 [故障排除](https://www.youtube.com/watch?v=uNeo7O6ImAo) ，你还有其他一些选择。你可以使用类似于 [Sharedrop.io](https://www.sharedrop.io/) 的服务从一个系统或另一个系统传输你的文件。或者，就此而言，你可以安装一个类似 [Dropbox](https://lifehacker.com/google-one-is-now-open-for-everyone-but-is-it-a-good-d-1826049257) 的云同步服务，然后从两台电脑登录。(确保您在 Dropbox 的设置中启用了局域网同步，以加快传输速度。)OneDrive 也是一个选项，它直接内置在 Windows 10 中。

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>*</small> 

<small></small>