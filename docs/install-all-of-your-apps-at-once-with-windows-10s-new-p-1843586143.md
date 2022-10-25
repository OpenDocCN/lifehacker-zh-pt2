# 使用 Windows 10 的新软件包管理器一次性安装所有应用

> 原文:[https://life hacker . com/install-all-of-your-apps-once-with-windows-10s-new-p-1843586143](https://lifehacker.com/install-all-of-your-apps-at-once-with-windows-10s-new-p-1843586143)

没有什么比*更性感的了，我使用包管理器来安装应用程序，而不是双击无聊的可执行文件*。它只是脱口而出。但是*使用命令行工具——技术上来说是 PowerShell——安装和更新你的应用程序是一件有趣的事情。一旦你掌握了它的窍门，这种体验甚至比使用普通的 Windows 应用商店更好(我听说是)。*

Watch

好消息:Windows 10 有一个全新的包管理器——或者至少，它将会有。微软现在正在测试 Windows 包管理器，你已经可以用它来安装相当多的应用程序了。然而，要访问包管理器，您需要经历一些困难。

### 如何注册测试 Windows 软件包管理器

正如微软 [对](https://devblogs.microsoft.com/commandline/windows-package-manager-preview/) 的描述，你有几个测试 Windows 包管理器的选项。如果您注册了 Windows Insider 计划(因为您喜欢生活在边缘),您就已经可以访问了。否则，你可以注册特定的 Windows Package Manager Insider 程序，或者自己从 GitHub 安装——尽管如果你选择后者，你不会获得自动更新。

我选择了第二个选项，在申请后，我几乎立即收到了一封电子邮件，通知我接受了预览计划:

无论你选择哪种方式，你都需要打开 Windows 商店并下载应用安装程序。微软在其博客中有一个链接，但对我不起作用。幸运的是，你还可以使用第二个技巧:Mash **Windows Key + R** 并复制粘贴到:

`ms-windows-store://pdp/?productid=9nblggh4nns1`

这让应用程序安装程序为我加载，我立即重新安装它(以防万一):

此时，我试图打开命令提示符并执行“winget”命令来测试包管理器，但是奇怪的事情发生了。

嗯。我不是唯一一个有这个问题的，因为它似乎在安装过程中出现了一些问题。GitHub 线程中建议的任何修复都无法让 winget 为我工作，我最终只能安装软件包管理器的 [GitHub 版本](https://github.com/microsoft/winget-cli/releases) ，这样我至少可以使用它。当我这样做的时候，效果非常好:

### 我已经安装了 Windows 软件包管理器。现在怎么办？

让我们找点乐子。首先，你可能想知道所有可以通过 Windows 包管理器安装的东西。那很简单。只需在命令提示符下键入`wget search`就可以了。以下是您将看到的一小部分示例:

要安装应用程序，只需输入`winget install [app name]`。如果你想了解更多关于这款应用的信息，请先输入`winget show [app name]`,然后再做其他事情。您还可以创建一个简单的脚本来一次安装多个应用程序，例如:

`@echo off Echo Install a bunch of appswinget install winrarif %ERRORLEVEL% EQU 0 Echo WinRAR installed successfully. winget install thunderbirdif %ERRORLEVEL% EQU 0 Echo Thunderbird installed successfully.pause`

将其复制并粘贴到一个文本文件中，添加尽可能多的其他应用程序(通过复制并粘贴第 3 行和第 4 行，然后更改应用程序名称)，并将其保存为. BAT 文件。每当您需要在电脑上重新安装喜爱的应用程序时，请运行。BAT——就像你使用 [Ninite 或其他应用](https://lifehacker.com/the-best-way-to-quickly-install-apps-on-a-new-windows-p-1836244140) 来管理批量安装一样。

### 我的应用程序安装不正确怎么办？我如何更新应用程序？

因为这是 Windows 包管理器的预览版，所以肯定会有一些奇怪的地方。例如，当我试图安装 Gimp 时，它一直提示我从两个版本中选择一个。显然，我会想要最新的，但这是我在构建脚本时不得不担心的又一个变量——只有当你试图安装一个应用程序但它并不完美时，你才会注意到这一点。

说起来，我显然安装了 WhatsApp，但它似乎并不在我的电脑上。我不知道它去了哪里，或者它是否安装了，但你去那里。

由于这是一个预览版，包管理器缺少了一些关键的特性，而这些特性可能是你希望从一个更健壮的程序中得到的。这包括卸载应用程序的能力(现在你必须通过 Windows 控制面板来完成)，以及更新你已经安装的应用程序的更重要的能力。不要担心，这种功能即将到来，只是现在还没有。如果这让你不满意，那么，总有 [勺](https://scoop.sh/) 。