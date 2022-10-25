# 使用此 PowerShell 脚本快速免费将 Windows 7 升级到 Windows 10

> 原文：<https://lifehacker.com/quickly-upgrade-windows-7-to-windows-10-for-free-with-t-1840843214>

如果你正在读这篇文章，你可能知道如何将一个版本的 Windows 升级到另一个版本。即使这是一个简单的过程，观看 Windows 下载和安装仍然是乏味和无聊的，然后你必须花更多的时间在屏幕上移动和调整设置。*咩。*

Watch

如果你或你认识的人一直坚持 Windows 7 直到痛苦的尽头，你应该知道你的操作系统在 1 月 15 日之后不会再收到任何安全更新。现在是最终将你的系统升级到 Windows 10 的最佳时机，尤其是因为 [可能是免费的](https://lifehacker.com/the-best-ways-to-get-windows-10-for-free-1837174464)——还因为我发现了一个超级简单的 PowerShell 脚本，它可以轻松地执行无人值守的升级。

换句话说，你开始升级过程，在开始时点击一两个对话框，然后你可以起身去做其他事情，而 Windows 10 会自动下载和安装。你的系统会在需要的时候重启，下一次你需要点击鼠标的时候，你就离你全新的操作系统一分钟之遥了。升级没有比这更容易的了。

### Windows 7 SP1 版 PowerShell 入门

因为我们需要 PowerShell 来做这个快速的小升级，并且 PowerShell [被嵌入到自 Windows 7 SP1 以来的](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-windows-powershell?view=powershell-6) 任何版本的 Windows 中，所以请确保您已经在*至少*到 升级了操作系统。换句话说，只要运行 Windows Update，安装它想让你安装的任何东西(如果有的话)。

一旦你准备好开始，点击开始按钮，输入 Powershell，右键点击“Windows Powershell”，选择“以管理员身份运行”

作为一项安全措施，PowerShell 被设置为默认情况下不运行脚本，直到您更改某个注册表项。为此，请在 Powershell 中键入以下内容，并在完成后按 Enter 键:

`Set-ExecutionPolicy Unrestricted`

您现在可以关闭 PowerShell 了。是的，没错。

### 键入您的安装脚本

将 [这个. PS1 文件](http://s000.tinyupload.com/index.php?file_id=51589467397114778925) 下载到你的电脑上。如果它不存在，或者您想手动创建它，打开一个新的文本文件，复制并粘贴以下内容(感谢非常有用的 [/r/PowerShell](https://www.reddit.com/r/PowerShell/comments/e6lndb/script_to_upgrade_windows_7_to_windows_10_like/) 子编辑):

> *$dir =* " *c:\temp*
> 
> *mkdir $dir*
> 
> *$webClient =新建-对象系统。网络客户端*
> 
> *$ URL =*"【https://go.microsoft.com/fwlink/?LinkID=799445】T2
> 
> *$ file =*"*$($ dir)\ win 10 upgrade . exe*"
> 
> *$webClient.DownloadFile($url,$file)*
> 
> *Start-Process-file path $ file-argument list*"*/quiet install/skipeula/auto upgrade/copy logs $ dir*"-动词 runas

删除行与行之间多余的空格，你可能还需要用直引号来替换这些引号，因为 Kinja 在默认情况下会将它们改为左引号和右引号。一旦你这样做了，关闭记事本，用你想要的名字保存你的文件，但是把它的扩展名改成. PS1(从。TXT)。

### 开始无人值守升级

右键单击新的. PS1 文件并选择“用 PowerShell 运行”你可能需要确认至少一个提示，允许“微软视窗”对你的电脑进行修改，但仅此而已。PowerShell 窗口会短暂出现和消失，然后在一段时间内您将看不到任何其他内容。

如果你像我一样多疑，你可以通过打开任务管理器并确保“Windows10UpgraderApp.exe”应用程序正在运行来检查安装是否正在运行。(您应该在流程的早期就能看到。)不然就去做别的吧。您的系统将在需要时自动重启，Windows 10 安装将在无需您任何额外输入的情况下启动。

当你的电脑让你做某件事的时候，你就知道已经完成了*，应该是这样的:*

您基本上只需要一两个屏幕就可以完成，这将花费您 15 秒的时间来完成检查。一旦你进入 Windows 10，你可能会注意到两件事:第一，你所有的数据和应用都应该在原来的地方(因为我们从 Windows 7 升级，而不是执行全新安装)。不能保证所有的东西都在那里——某些程序可能不兼容，不能随身携带——但这是我将在以后的文章中讨论的问题。

不过，升级方面很关键，因为假设你来自激活版本的 Windows 7，你也应该有一个完全激活版本的 Windows 10。如果没有，输入您的 Windows 7 密钥应该是激活 Windows 10 所需要的，使用您的 Microsoft 帐户登录应该会使激活过程对于任何后续安装都更加容易。

### 不要忘记重置 PowerShell 的执行策略

还记得我们解放 PowerShell 并允许它运行任何它想要的脚本吗？为了安全起见，现在是扭转这一局面的好时机。使用管理权限打开 PowerShell(与之前相同)，并输入以下内容:

`Set-ExecutionPolicy Restricted`

一旦你这样做了，你可以关闭 PowerShell 和 [开始骗出你喜欢的 Windows 10](https://lifehacker.com/how-to-set-up-your-windows-laptop-from-scratch-1826146907) 。不过，你可能不需要马上运行 Windows Update，因为你应该已经安装了微软最新版本的操作系统。