# 安装 macOS Catalina 测试版的最安全方式

> 原文：<https://lifehacker.com/the-safest-way-to-install-the-macos-catalina-beta-1835836662>

苹果所有最新操作系统版本 [的公开测试版终于发布了](https://twitter.com/marcoarment/status/1143227695838502913)(watch OS 除外)。我们总是警告人们在他们的主要设备上安装这些，因为你不希望你工作和社交所依赖的 iPhone 开始因为一个错误版本的 iOS 而冻结。

Watch

如果你是 Mac 用户，你很容易做到。而不是更换你的操作系统——糟糕！—您可以在您的驱动器上创建一个全新的卷，并在那里安装 macOS Catalina。然后你就可以随时选择是启动你信任的旧 macOS 还是全新的测试版，当你玩完之后，你可以很容易地从你的系统中删除 Catalina 测试版。除非您的系统空间紧张，否则没有理由不选择 Catalina beta 版。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1143227695838502913&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1143227695838502913&autosize=1) 

苹果公司有 [一个伟大的纲要](https://support.apple.com/en-us/HT208891) 你需要做的一切来实现这一点。以下是关键点:

*   在你做任何事情之前备份你的系统(以防万一)
*   打开“磁盘工具”，在最左侧的边栏中选择您当前的宗卷，然后点按工具栏上“宗卷”下的+图标以添加新的 APFS 宗卷。
*   确保你注册了 [苹果测试软件项目](http://beta.apple.com/) 。当您下载 macOS Catalina 并准备安装它时，选择新的宗卷，而不是现有的宗卷作为目标。
*   安装 macOS Catalina 后，通过使用“系统偏好设置”中的“启动磁盘”或在 Mac 启动时按住 Option 键，在操作系统之间切换。

要删除 macOS Catalina，您只需删除安装它的 APFS 宗卷。打开“磁盘工具”,突出显示该卷，然后单击“卷”下面的-图标来删除它——就这么简单。