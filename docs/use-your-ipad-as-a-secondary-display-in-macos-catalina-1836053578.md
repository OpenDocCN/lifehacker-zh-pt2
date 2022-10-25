# 在 macOS Catalina 中将您的 iPad 用作辅助显示器

> 原文：<https://lifehacker.com/use-your-ipad-as-a-secondary-display-in-macos-catalina-1836053578>

[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)) : title[![](../Images/80a55aae3a4e6ac59b23fae8fccddf22.png)](https://applemacos.kinja.com)[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)Many people turn to Macs because they're incredibly easy to operate. That's true, but there's still plenty worth knowing before you can truly master your Mac.

你会在 macOS Catalina 中发现一个更简洁的功能——至少肯定引起了我的注意——是苹果新的“Sidecar”模式。就像大型摩托车上的小座椅一样，Sidecar 可以让你将 iPad 连接到 Mac 上，并将其用作辅助显示器。如果你有一支苹果铅笔，你甚至可以和屏幕上的物体互动。



由于这项功能是作为 macOS Catalina 的一部分进行测试的，一旦 OS 的最终版本发布(今年秋天)，它的确切性质可能会发生变化。即使现在，苹果也没有列出哪种设备组合支持 Sidecar，但下面是人们拼凑的作为可能性:

*   2015 年末 27 英寸 iMac 或更高版本
*   2017 款 iMac Pro
*   2016 年年中 MacBook Pro 或更新版本
*   2018 年末 Mac mini 或更高版本
*   2018 年末 MacBook Air 或更新版本
*   2016 年初的 MacBook 或更新版本
*   2019 年 Mac Pro

至于 iPad，任何运行 iPadOS *的设备都应该能够使用 Sidecar，这意味着任何 iPad Pro，第五代和第六代 iPad，iPad Mini(第五代)和 iPad Mini 4，以及 iPad Air(第三代)和 iPad Air 2。*

### 如果您 Mac 不在列表中

如果你的 Mac 太旧，一旦 macOS Catalina 的最终版本发布，你可能就不能运行 Sidecar 了。现在，你可以利用一个小漏洞来尝试这个特性。在 macOS Catalina 中调出终端 [，输入如下:](https://lifehacker.com/the-safest-way-to-install-the-macos-catalina-beta-1835836662) 

`defaults write com.apple.sidecar.display AllowAllDevices -bool true; defaults write com.apple.sidecar.display hasShownPref -bool true; open /System/Library/PreferencePanes/Sidecar.prefPane`

一旦你按下回车键，你的系统首选项应该出现，新的“边车”选项应该可见。你可能不喜欢边斗的质量，但你至少可以看到它的样子(概念上)。正如一位 Redditor [写的](https://www.reddit.com/r/apple/comments/bx3eet/sidecar_support_on_older_macs/) :

“我设法让 Sidecar 与我的 2014 年年中 MacBook Pro work 和 iPad Pro 兼容。它在最小延迟方面很棒，但图像质量很差。我猜限制是关于硬件 HEVC 编码，它需要英特尔酷睿第六代处理器。”

### Sidecar 入门

要开始使用 Sidecar ，打开系统偏好设置并寻找 Sidecar 选项。打开它，你会看到一个漂亮的屏幕，上面有一些基本的选项。您可以选择有线或无线方式连接到您的设备。

在这种情况下，我已经从下拉菜单中选择了我的 iPad，否则它会出现在 iPad 的巨大图像下。这样一来，它会自动将我的 iPad 显示屏转换成我桌面的扩展版:

理论上，左边的左上角图标应该隐藏和显示你的工具栏。(我从来没有得到它做任何事情。)它下面的图标隐藏并显示你的 Dock——把它从 Mac 上拉下来显示在 iPad 上，反之亦然。

其他图标应该是不言自明的。不过，请特别注意 iPad 显示屏底部的虚拟触摸条。即使你的 Mac *没有*Touch Bar，这里也会出现一个供你玩。或许这会鼓励你升级，或者反过来，提醒你 Touch Bars 有点傻。

#### 不要用你的手指

如前所述，你需要一支 Apple Pencil 来与你的显示器交互，我不相信它的压力敏感性适用于这种模式(至少，当我用 Affinity Photo 测试它时，它没有)。你的点击就像是在你的鼠标上左击；没有办法右键单击或弹出上下文菜单，如果你试图调整窗口大小并意外关闭它，这会让事情变得有点危险。

不过，你可以直接在 iPad 上用 Affinity Photo 或 Adobe Photoshop 之类的应用程序画画。虽然这不如简单地在 iPad 上完成整个绘图，然后发送到 Mac 上进行额外编辑那么优雅，但这至少是一种快速润色的好方法。

#### 在设备间切换应用

我还没有找到使用键盘命令在两个桌面之间移动活动窗口的方法，但是单击并拖动窗口是一个简单的选择。您也可以点击窗口，然后选择“移动到...”在 Mac 和 iPad 之间发送应用程序(然后再返回)。

苹果 macOS Catalina 的初始文档列出了一些与 Sidecar 兼容的应用程序:

不要被骗了。大量其他应用程序可以在你的辅助显示器上工作，即使你可能不得不在窗口而不是全屏模式下使用它们。然而，对于游戏来说，情况就不一样了。我可以运行基本的 Steam 游戏——比如 jack box Party Pack——但更复杂的游戏根本无法在我的 Mac 上运行。我在我的 Mac 或连接的 iPad 上玩我从 App Store 下载的游戏都没有问题，但我只真正测试了一款游戏:[《Flappy Golf 2》](https://apps.apple.com/us/app/flappy-golf-2/id1154174205?mt=12)。我很好奇，看看是否有更重的击球手与 Sidecar 配合得很好。我怀疑他们不会，考虑到你的系统有多少是与双显示器设置捆绑在一起的。

#### 混合 Mac 和 iPadOS 应用程序

Sidecar 最有趣的应用之一是，你可以用它在同一个屏幕上与 Mac *和* iPadOS 应用程序进行交互。由于 Sidecar 本身从技术上来说是一个应用程序，你可以通过 Slide Over 将其他应用程序钉在它上面(iPad 显示屏左边的 [或右边的](https://support.apple.com/en-us/HT207582) )。不幸的是，你不能同时拆分 Sidecar 和另一个应用程序，但你至少可以管理 Mac 上任何打开的窗口的大小，这样它们就不会隐藏在你滑过的 iPadOS 应用程序下面。

#### 镜像或扩展您的显示器

我还喜欢在 iPad 上扩展*或*镜像你的桌面显示是多么容易，这个选项可以在你工具栏的传统显示图标中找到。请注意，切换到镜像模式会(暂时)扰乱 Mac 的分辨率，但之后你就可以用 Mac 或 iPad 控制单个屏幕了——如果你不想一直来回切换应用程序，这很有用。

#### 边车很快

Sidecar 最棒的部分之一就是整个交互是多么的无缝。虽然这无疑会受到你的 wifi 连接和/或你的两个设备之间的距离的影响(如果你像我一样使用无线网络)，但我对你在与你的 iPad 互动时能够快速进入边斗模式和 Apple Pencil 的响应速度印象深刻。尽管它有它的怪癖，边车模式使用起来感觉很棒。