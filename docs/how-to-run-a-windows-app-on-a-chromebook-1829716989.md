# 如何在 Chromebook 上运行 Windows 应用程序

> 原文：<https://lifehacker.com/how-to-run-a-windows-app-on-a-chromebook-1829716989>

谷歌基于云的 Chrome OS 已经演变成一个令人印象深刻的计算平台，现在它兼容 Android 应用程序，最近又兼容 Linux 应用程序。

Watch

但是你可能会想，Windows 应用程序呢？所有关于 Windows 兼容性的传言都到哪里去了？它们仍在浮动，但你不必等待它们变成现实，就可以在 Chromebook 上运行 Windows 应用程序。你所需要的是交叉应用程序和一点实验时间。

Crossover 是一个免费的应用程序(目前)，可以在虚拟机中运行 Windows 程序。它很容易使用，虽然 Linux 已经有了一个完全成熟的版本，也与 Chrome OS 兼容，但 Android 版本的 Crossover 更加用户友好。如果你对在 Chromebook 上运行 Windows 应用程序的新奇感感到好奇，或者也许你非常想运行一个经常使用的最喜欢的应用程序，请继续阅读。

### 什么是跨界？

Crossover 是一个在中可用的免费虚拟机。它还在测试阶段，尽管在应用的主页上有一个巨大的“试用期”横幅。([)code weavers](https://www.codeweavers.com/products)称你“很快”就能支付完整的安卓版本这款应用的 Android/Chrome OS 版本仍处于试验阶段，但它采用了与 macOS 和 Linux 版本相同的底层技术。

由于 Crossover 已经在其他平台上酝酿了一段时间，其 Android 版本相当强劲。如果需要，每个通过 Crossover 启动的 Windows 应用程序都可以在不同版本的 Windows 上运行，你甚至可以添加基本组件，如字体库。

需要记住的一个主要警告是，由于 Chrome OS 的 Android 环境的限制，Crossover 只能运行 32 位应用程序。(Crossover 在 macOS 和 Linux 上运行 64 位应用程序。)

### 如何安装分频器

在你可以从 [【谷歌 Play 商店】](https://play.google.com/store/apps/details?id=com.codeweavers.cxoffice) 安装 Crossover 之前，你需要确保你的 Chromebook 能够处理安卓应用*和*足够快来运行虚拟机。Codeweavers 建议在基于英特尔的 Chromebook 上使用该应用程序。

为了确保你的设备可以运行从 Play Store 下载的 Android 应用程序，请进入 Chromebook 的设置菜单。如果一切正常，你会看到一个 Google Play 选项，带有一个指向 Chrome OS 's Android 设置的外部链接。如果你使用的是旧版本的 Chrome 操作系统，你可能需要启用开发者模式来访问 Android 应用。

### 如何使用交叉安装 Windows 应用程序

使用 Crossover 安装 Windows 应用程序有两种方式。第一种是通过 Crossover 的已知应用程序数据库安装一个可执行文件。您可以使用应用程序主页上的搜索栏来访问它。键入你希望安装的程序的名称，Crossover 会在屏幕上显示匹配的结果。你可以寻找的一些应用程序包括微软 Office 2006 和 2010，旧版本的 Adobe Photoshop，FileZilla 和 7-Zip。(您可能需要购买密钥才能使用其中的一些应用。

如果您找不到想要的内容，请尝试使用“安装未列出的应用程序”选项来安装 Windows 应用程序，该选项允许您直接指向安装程序文件。在搜索栏中输入应用名称后，点击右下角的选项。在下一个窗口中，选择“搜索安装程序”导航到安装文件。按照出现的安装提示进行操作。

一旦你使用任何一种方法安装了 Windows 程序，你就可以从 Chromebook 的应用程序抽屉或 Crossover 的主登录页面启动该应用程序。

运行 Windows 应用程序还有第三种方法，但只有在前两种方法都不成功的情况下才应该尝试。它包括创建各种各样的“shell 桌面”,以便您可以手动运行安装程序文件。像以前一样，输入程序名后点击“安装未列出的应用程序”，然后选择“创建一个空环境”选项这将安装运行 Windows 应用程序所需的组件。

一旦虚拟环境准备就绪，就会弹出一个对话窗口。点击下拉菜单中的“启动文件资源管理器”选项，然后导航您设备的文件系统以选择。exe 文件来启动。

如果您需要在不同版本的 Windows 上运行应用程序，也可以使用这种方法。要访问此设置，请从主交叉页面点击应用程序，然后从下拉菜单中选择“葡萄酒配置”。将出现一个应用程序选项卡，底部有一个选项，用于更改该应用程序的 Windows 版本。你可以选择早至 Windows 3.0 的版本，也可以选择 Windows 10 加入我们这个时代。默认情况下，Crossover 将根据数据库中的信息为每个应用程序设置兼容性。

### 如何在 Chrome 操作系统上使用 Windows 应用

如上所述，你可以从 Chromebook 的应用程序抽屉或 Crossover 的主登录页面启动应用程序。如果一个应用程序崩溃(这种情况经常发生)，Crossover 会弹出一个通知，并提供一个强制关闭的选项，这有助于缓解你设备的内存缓存。

通过 Crossover 使用 Windows 应用相对简单，但不要把期望值设得太高。并非所有的 Windows 应用程序都支持这个版本的 Crossover。我试过安装 Windows 版的 Spotify 和 Adobe Creative Cloud，都没有成功。然后我安装了 Steam，让我可以用它的聊天应用给我的朋友发信息，尽管它经常因为无法加载一些促销弹出窗口而崩溃。

一些应用程序甚至不允许你安装软件，因为它是一个虚拟机，虽然 Codeweavers 提供了对微软 Office 2010 等传统程序的直接访问，但你仍然需要一个有效的密钥来解锁体验。即使你设法让这样的应用程序运行起来，你也可能不得不通过在互联网上到处搜索来弥补任何缺失的组件。

我确实在谷歌的 Pixelbook 上成功运行了 Windows 应用程序。 [7-Zip](https://www.7-zip.org/) 完美无缺地将 Zip 文件解压到下载文件夹，我从运行一个老经典、 [滑雪免费](https://ski.ihoc.net/) 中得到了乐趣。 [FileZilla](https://filezilla-project.org/) 允许我访问我的 FTP 服务器，而 [Gimp](https://www.gimp.org/) 与 Pixelbook 的触摸屏一起使用很有趣。我还设法运行了一些不太知名的应用程序，比如 [批量重命名实用程序](https://www.bulkrenameutility.co.uk/Main_Intro.php) ，它的界面非常过时，但在批量重命名数百个文件时却很有效。

这些例子解释了为什么你会不厌其烦地在 Chromebook 上运行 Windows 应用程序:以帮助提高你在 Chrome OS 上的工作效率。毕竟，并不总是有一个 Android 应用或 Chrome 扩展可以完成这项工作。虽然 Crossover 并不完全等同于在 Chrome OS 上运行成熟的 Windows 应用程序，但至少在谷歌继续建立其基于云的操作系统时，它有助于弥合一些差距。