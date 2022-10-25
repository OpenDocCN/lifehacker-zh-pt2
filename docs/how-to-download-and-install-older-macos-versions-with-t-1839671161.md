# 如何使用“终端”下载和安装旧版本的 macOS

> 原文：<https://lifehacker.com/how-to-download-and-install-older-macos-versions-with-t-1839671161>

[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)) : title[![](../Images/80a55aae3a4e6ac59b23fae8fccddf22.png)](https://applemacos.kinja.com)[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)Many people turn to Macs because they're incredibly easy to operate. That's true, but there's still plenty worth knowing before you can truly master your Mac.

当需要安装新版 macOS 或下载新的更新时，几乎每个人都会去 Mac App Store 开始这个过程。虽然 App Store 使操作系统的安装变得简单且相对容易，但它并不总是有效的——也许是时候转向终端(和一点创造力)了。

Watch

如果您正尝试安装旧版本的 macOS 或 OS X,“终端”尤其有用，从技术上讲，许多旧版本都可以从 Mac App Store 获得，但当您尝试下载时会被列为“不可用”。您可能无法通过这种方式获取它们，但是“终端”可以为您做些跑腿的工作。

### 如何使用终端下载 macOS 更新和安装文件

我们将在本指南中重点介绍两个特定的命令:一个下载最新的 macOS 更新，另一个让你下载旧的 macOS 或 OS X 版本，详见 GitHub 上的 [512 像素](https://512pixels.net/2019/10/download-macos-installers-with-terminal/) 和 [JAMF 开源社区](https://github.com/jamf) 。这样做比简单地点击应用商店需要更多的工作，但是不要担心——如果你是新手，终端命令可能看起来令人生畏，但是我们将要使用的命令执行起来很简单。方法如下:

1.  进入**查找器>应用>实用程序>终端**，开始打开 macOS Catalina 的终端。
2.  在终端中键入以下命令之一:
3.  **要下载最新的 macOS 更新**，请键入:`softwareupdate —fetch-full-installer`
4.  **要下载旧版本的 macOS** ，请键入:`softwareupdate —fetch-full-installer [build number]`(例如:“软件更新-获取-完整-安装程序 10.14.5”)
5.  按下**回车键/回车**键执行该命令。
6.  安装文件将下载到 Mac 的“应用程序”文件夹中。打开文件开始安装，然后按照屏幕上的说明完成更新(或回滚)。

请记住，并非所有版本的 macOS 或 OS X 都可以通过这种方式下载，有些版本只与某些 Mac 硬件兼容。不过，这应该可以很好地抓取最新的 macOS 更新，你应该可以下载几个旧的 macOS 和 OS X 版本(可能早在 OS X Yosemite)。

对于高级用户来说，值得一提的是，这些并不是你可以用来更改或更新 Mac 操作系统的唯一终端命令，你可以在 JAMF 社区 Github 页面 的 [找到更多命令。](https://github.com/jamf/erase-install-webinar/wiki)