# 如何阻止微软在你的电脑上安装 Edge (Chromium)

> 原文:[https://life hacker . com/how-to-keep-Microsoft-from-installing-edge-chromium-o-1840481536](https://lifehacker.com/how-to-keep-microsoft-from-installing-edge-chromium-o-1840481536)

微软计划在 1 月 15 日通过 Windows 更新推出 Edge。自从浏览器的 Chromium 版本在 4 月份首次亮相以来，我们已经玩得很开心了，在下个月正式发布之前，我们可能会有更多的话要说。但我也不希望你的台式机或笔记本电脑上有另一个浏览器——不幸的是，在这个问题上你没有太多的选择。

Watch

我们认为，由您来决定将什么推送到您的系统中是非常重要的。更新是一回事；在你的系统上安装一个额外的浏览器是另一个问题。谁知道 Edge 一旦进入你的系统会有多强呢？您是否必须返回并将您最喜欢的浏览器设置为默认浏览器？你会不会收到恼人的提醒，说 *Edge 提供了更好的体验*和*你真的应该切换到它*和*请尝试一下也许？*

如果您知道在 Microsoft 将 Edge 自动安装到您的系统上时您根本不会使用它，您可以阻止 Windows Update 这样做。很简单。访问 [这个微软网站](https://docs.microsoft.com/en-au/deployedge/microsoft-edge-blocker-toolkit) ，下载拦截器工具包。运行可执行文件，它会将一个. CMD 文件(和另外两个文件)解压缩到您想要的任何位置。然后，打开一个管理命令提示符(当您通过开始菜单搜索它时，右键单击并选择“以管理员身份运行”)，并导航到该文件所在的文件夹。CMD 文件存在。

在那里，通过在命令提示符中输入**" edge chromium _ blocker . cmd "**来运行它。然后，您将看到可以使用哪些标志来阻止和取消阻止自动安装。如果你想直接跳到那一步，那么输入**" Edge chromium _ blocker . cmd/b "**来阻止 Windows Update 在你的系统上安装 Edge，如果你想反向操作，使用 **"/u"** 标志。

需要注意的是，如果你想试用微软 Edge，这并不妨碍你安装它。这只会阻止 Microsoft 通过 Windows Update 为您安装它。你仍然可以正常运行 Windows Update 来获得所有最新的系统修复和驱动程序更新，如果你设置了阻止安装的标志，你就不会在 1 月份获得 Edge。

如果你已经是一个大的 Edge 用户——普通浏览器，而不是基于 Chromium 的新版本——有必要知道当这个新的更新在 1 月份取代你当前的浏览器时会发生什么。根据 [到微软](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-sysupdate-windows-updates) ，下面是它的意思:

> *   *All start menu pins, tiles and shortcuts of the current version of Microsoft Edge will be migrated to the next version of Microsoft Edge.*
> *   *All taskbar pins and shortcuts of the current version of Microsoft Edge will be migrated to the next version of Microsoft Edge.*
> *   *The next version of Microsoft Edge will be nailed to the taskbar. If the current version of Microsoft Edge has been fixed, it will be replaced.*
> *   *The next version of Microsoft Edge will add a shortcut to the desktop. If the current version of Microsoft Edge already has a shortcut, it will be replaced.*
> *   *Most of the protocols handled by Microsoft Edge by default will be migrated to the next version of Microsoft Edge.*
> *   *At present, Microsoft Edge will hide all UX interfaces in the operating system, including settings, all applications and any file or protocol support dialog boxes.*
> *   *All attempts to start the current version of Microsoft Edge will be redirected to the next version of Microsoft Edge.*

如果你真的真的想继续使用微软 Edge 的旧版本*和新版本*，你也可以这样做，用 [稍微提前规划一下](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-sysupdate-access-old-edge) 。除非这是关键任务，否则我建议冒险一试。让 Chromium Edge 成为你的新优势。不要退缩。