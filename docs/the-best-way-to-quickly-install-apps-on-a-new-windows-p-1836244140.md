# 在新的 Windows 电脑上快速安装应用程序的最佳方式

> 原文：<https://lifehacker.com/the-best-way-to-quickly-install-apps-on-a-new-windows-p-1836244140>

当我面对一个全新的操作系统时，我做的第一件事就是启动它的默认浏览器——即 *meh* Edge 或 Safari——然后直奔到 [Ninite](https://ninite.com/) (Windows)或[Mac apps . link](https://macapps.link/en/)(Mac)。这两个网站都允许你挑选你想安装在新系统上的应用。一旦你最终确定了你的列表，你就可以得到一个定制的安装程序(Ninite)或者一个终端命令(macapps.link ),你可以运行它来快速地把一堆应用程序转储到你的新系统上。



这个过程比手动操作要快得多——访问每个应用程序的网站，下载并运行它的安装程序，然后坐在那里等它慢慢运行——但是现在我们可以做得更好。这一切都要归功于一个易于使用的软件包管理器，它支持的软件甚至比 Ninite 或 macapps 还要多。

我们之前已经讨论过 Chocolatey 主要是这个应用的 [GUI 版本](https://lifehacker.com/install-and-update-all-your-windows-apps-at-once-with-t-1827588626) ，它基本上是在你的桌面上重建一个小版本的 Ninite。今天，我们将忽略所有漂亮的东西，直接进入命令行，因为这是在全新的 Windows PC 上安装必备应用程序的最快、最简单的方法。

### 第一步:安装巧克力

要让这个免费的软件包管理器在你的新系统上运行，你需要安装它。这再容易不过了。通过在 Windows 开始菜单中搜索“命令”，右键单击“命令提示符”列表，并选择“以管理员身份运行”，弹出一个管理命令提示符

为了节省更多宝贵的时间，你也可以右击开始菜单图标，选择“命令提示符(管理)”，如果它出现的话。如果你得到了 PowerShell 的列表，转而打开命令提示符——它会在 [之后为你节省一步](https://chocolatey.org/install) 。

一旦命令提示符弹出，在 中键入 [this，然后回车。(它应该在命令提示符下显示为一行巨大的文本。)](https://chocolatey.org/install)

`@”%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe” -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command “iex ((New-Object System.Net.WebClient).DownloadString(‘` [`https://chocolatey.org/install.ps1'))`](https://chocolatey.org/install.ps1'))) `“ && SET “PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin”`

当安装过程开始时，你会看到一串文本。如果成功，最后几行应该是这样的:

你猜怎么着？你已经完成一半了。

### 第二步:用 Chocolatey 安装一堆应用程序

接下来，您需要在桌面上打开一个文本文档。(你可以在任何地方打开，真的；没关系。)您将使用它来存储您想要安装在新系统上的所有不同应用程序的列表——从技术上讲，是通过 Chocolatey 安装它们的命令。

你还会想打开你的网络浏览器，导航到 Chocolatey 的 [丰富的应用程序目录](https://chocolatey.org/packages) 。

坏消息呢？我们现在处于最困难的阶段，但是你只需要做一次。你需要浏览 Chocolatey 的应用目录，寻找你喜欢在电脑上使用的所有不同的应用。你可能已经知道它们是什么了；如果没有，在你要处理的旧电脑上查找它们并不难(如果适用的话)，或者通过浏览 Chocolatey 的应用程序列表(按名称或受欢迎程度排序)也不难。我们有 [我们自己的选择](https://lifehacker.com/lifehacker-pack-for-windows-our-list-of-the-essential-1828117805) ，如果这能帮到你的话。

一旦你找到一个你想安装在你的新系统上的应用程序，你会想把它输入到你的文本文件中，就像这样:

`choco install [name of package] -fy`

[包的名称]应该是 Chocolatey 的应用程序目录中列出的任何内容。所以，如果你安装的是谷歌浏览器，看起来会是这样的:`choco install googlechrome -fy`

小小的“-fy”标志是一个简单的标志，它告诉 Chocolatey 在安装过程中出现任何提示时选择“yes”。换句话说，我们希望尽可能地自动化这一过程，因为我们的目标是让你不必点击或做任何事情，而所有你喜欢的应用程序都神奇地出现在你的系统上。

你要安装的每个应用程序都需要单独的一行，每一行看起来都应该一样。所以，当你完成时，你的文本文件应该看起来像这样(无论你选择什么应用程序):

你*可以通过一行代码*安装所有这些应用，如下所示:`choco install googlechrome 7zip.install notepadplusplus.install vlc -fy`

我更喜欢多行方法，因为随着需求的变化，它可以非常容易地添加和删除应用程序。

一旦你完成了要安装的应用程序列表，保存文本文件并关闭它。然后重命名它，将它的扩展名改为。击球，然后按回车键。(如果您没有看到您的文件扩展名为。txt，您首先需要在文件资源管理器中启用文件扩展名。)

之后，右键单击您的新。bat 文件并选择“以管理员身份运行”，这将触发所有应用程序的 Chocolatey 安装过程。就这么简单。

一旦你完成了，我建议保存这个。bat 文件到云端——你的 [Dropbox，Google Drive，或者其他什么](https://lifehacker.com/google-one-is-now-open-for-everyone-but-is-it-a-good-d-1826049257)——这样你就可以在设置新系统的时候随时访问它(包括 [你正在尝试的任何虚拟桌面](https://lifehacker.com/how-to-set-up-a-virtual-machine-for-free-1828969527) )。

### 额外步骤:如何用一个文件安装所有的东西

如果您已经做到了这一步，您可能想知道是否可以同时完成本文中的所有工作。换句话说，通过同样简单的方式安装 Chocolatey *和*你最喜欢的应用程序。bat 档。

你可以！

打开。bat 文件，并将 Chocolatey 安装命令文本附加到顶部。当你完成时，它应该看起来有点像这样。(我已经打开了自动换行以便于阅读，但是安装文本应该占据一行。)

保存该文件，然后你就可以运行它(以管理员权限)让一台全新的 Windows 电脑立即启动并运行你最喜欢的 Chocolatey *和*应用程序。看到了吗？这甚至比尼尼特还要快。