# 如何在 Mac 上重建 iOS 13 的动态壁纸

> 原文:[https://life hacker . com/how-to-recreate-IOs-13s-dynamic-wallpaper-on-your-MAC-1835654716](https://lifehacker.com/how-to-recreate-ios-13s-dynamic-wallpaper-on-your-mac-1835654716)

[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)) : title[![](../Images/80a55aae3a4e6ac59b23fae8fccddf22.png)](https://applemacos.kinja.com)[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)Many people turn to Macs because they're incredibly easy to operate. That's true, but there's still plenty worth knowing before you can truly master your Mac.

iOS 13 测试版为我们提供了一个新的动态背景预览，当 iOS 13 在今年秋天向公众推出时，iPhone 用户将会看到这些背景。iOS 13 上的新背景会根据你使用的是亮还是暗主题来变换颜色。静态图像本身不会这样做，但自从 macOS 在 Mojave 中开始支持动态桌面背景后，只需最少的努力和几个额外的文件，就可以在 Mac 上重新创建 iOS 13 的壁纸效果。

Watch

为此，我们将使用 [开源 macOS 程序 wallpaper](https://github.com/mczachurski/wallpapper)，它允许你从图像文件夹中创建动态壁纸。从头开始创建一个动态壁纸文件需要一点编码，但是多亏了 [Github 开发者 alicerunsonfedora](https://github.com/alicerunsonfedora/ZephyrMac) ，壁纸图像已经被编译成我们可以在 wallpaper 中使用的目录。

下面是整个过程，一步一步来:

*   首先，确保你的 Mac 上安装了 [Xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12) 和 [Swift 5](https://www.apple.com/swift/) 。
*   打开终端，安装神奇的 [家酿](https://brew.sh/) 软件包管理器(如果你还没有的话)
*   使用以下命令使用家酿安装壁纸:`brew tap mczachurski/wallpapper`和`brew install wallpapper`
*   接下来，在终端中运行`wallpapper -h`来验证你是否成功安装了 Wallpapper。如果是这样，您应该会看到这样开始的响应:

```
wallpapper: [command_option] -i inputFile
```

*   接下来从 Github 下载 alicerunsonfedora 的 [ZephyrMac](https://github.com/alicerunsonfedora/ZephyrMac) 目录 [。这包含了为每种泽法背景色正确组织和编译的图像目录:黑色、红色、绿色和蓝色。](https://github.com/alicerunsonfedora/ZephyrMac/archive/master.zip)
*   在“终端”中，使用“cd”命令导航到解压 ZephyrMac 主文件的位置。对于大多数人来说，这将涉及两个命令:`cd downloads`和`cd zephyrmac-master`
*   之后，输入`cd <color>`，将<颜色>替换为任何代表你想要的壁纸的文件夹名称。之后，输入以下命令:`wallpapper -i wallpapper.json -o wallpapper.heic`
*   这将创建一个名为 wallpaper.heic 的新文件，我们现在可以通过进入**苹果>系统偏好设置>桌面&屏幕保护程序**将其应用为桌面背景。在“桌面”选项卡下，找到并选择 wallpapper.heic 文件以应用背景。