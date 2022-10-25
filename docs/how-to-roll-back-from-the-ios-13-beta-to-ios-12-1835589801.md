# 如何从 iOS 13 测试版回滚到 iOS 12

> 原文：<https://lifehacker.com/how-to-roll-back-from-the-ios-13-beta-to-ios-12-1835589801>

iOS 13 [的第一个测试版是给开发者](https://lifehacker.com/how-to-install-the-latest-apple-betas-if-youre-not-a-de-1835296432) 玩的(还有喜欢生活在边缘的 [craftier 苹果粉丝](https://lifehacker.com/how-to-install-the-latest-apple-betas-if-youre-not-a-de-1835296432) )，但这不全是乐趣和游戏。虽然有一些 [令人敬畏的新功能](https://lifehacker.com/all-the-big-ios-13-changes-apple-announced-at-wwdc-19-1835216984) 测试版测试人员如果现在安装 iOS 13 就可以试用，但该操作系统并不完整，在 iOS 13 准备好公开发布之前，苹果还有几个月的测试时间。

Watch

如果你已经提前升级到了 iOS 13 测试版，并且感觉到了一些升级者的懊悔，不要担心。你可以让 iOS 回到 iOS 12 的舒适和稳定——至少，直到下个月晚些时候公开测试版发布，这应该比第一个开发者测试版更稳定一点。

### 下载必要的系统文件

首先，找到并下载您设备的。从[https://ipsw.me/](https://ipsw.me/)到的 IPSW 文件。您可以使用右侧边栏菜单中的“识别我的 iOS 设备”工具，也可以搜索您的 iPhone 或 iPad 的型号名称(如 iPhone X、iPad Pro、iPhone 8s 等。).保存。iOS 12.3、12.3.1 或 12.3.2 的 IPSW 文件。当它下载时，这是一个好机会，如果你在 Windows PC 上进行回滚，请确保你已经安装了[iTunes](https://www.microsoft.com/en-us/p/itunes/9pb2mz1zmb1s)。

### 配置您的 iOS 设备

在执行降级之前，不要费心备份您的设备。虽然在升级到新版本的 iOS 时这样做通常是个好习惯，但您不能使用 iOS 13 备份在 iOS 12 中执行恢复。(当你想安装测试版时，我们总是建议对你的旧版本 iOS 做一个基于 iTunes 的离线备份。)

你还需要禁用 iOS 13 中的“查找我的 iPhone/iPad”选项。这可能看起来是一个奇怪的步骤，但是您需要关闭它以防止该特性在回滚期间导致错误。

1.  打开 iOS 设备上的设置。
2.  点击设置窗口顶部的您的帐户名称，然后前往**“查找我的”>“查找我的 iPhone/iPad”**，点击**“查找我的 iPhone/iPad”**滑块将其禁用。
3.  键入您的 Apple ID 和密码以应用更改。

### 安装旧版本的 iOS

一旦您禁用了**“查找我的设备”**设置和您的。IPSW 文件已经下载完毕，你可以开始回滚。

1.  将您的 iOS 设备插入 Mac 或 PC。iTunes 应该会自动启动。
2.  在侧边栏中，单击“设备”下的 iPhone 图标，打开“设备摘要”屏幕。
3.  在 Mac 上按住 Option 键，或者在 Windows 上按住 Shift 键，然后点按“恢复 iPhone”
4.  在出现的文件浏览器中，找到并打开您先前下载的 IPSW 文件。
5.  答:会出现一个弹出窗口，让你知道你正在安装新版本的 iOS。点击“恢复”
6.  等待过程突突前进。在安装过程中，可能会要求您输入设备密码。当设备重新启动并出现“欢迎”启动屏幕时，安装完成。
7.  如果您在运行 iOS 12 时备份了手机，并且想要恢复数据，请轻按“从 iCloud 恢复”或“从 iTunes 备份恢复”如果没有，请轻按“设置为新 iPhone”按照屏幕上的说明完成设置和恢复。

随着这些步骤的完成，你的设备现在安全地回到了 iOS 12 充满爱意的稳定怀抱。