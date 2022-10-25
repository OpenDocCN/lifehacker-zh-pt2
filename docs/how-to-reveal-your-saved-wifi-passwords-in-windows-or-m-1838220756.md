# 如何在 Windows 或 macOS 中显示您保存的 Wifi 密码

> 原文:[https://life hacker . com/how-to-reveal-your-saved-wifi-passwords-in-windows-or-m-1838220756](https://lifehacker.com/how-to-reveal-your-saved-wifi-passwords-in-windows-or-m-1838220756)

给我出个谜语:你在某个地方，你需要用一个新设备连接到 wifi 网络。您意识到您的笔记本电脑上保存了 wifi 密码，但您想要连接的任何设备上都没有。而你要么是懒得再问密码，要么是以你现在的条件根本没办法获取。

Watch

你是做什么的？简单。拿出你的笔记本电脑，查找一下。方法如下:

### Windows 操作系统

要查找保存的 wifi 密码，您有几个选项。**首先**，你可以弹出一个命令提示符，输入这个有点复杂的字符串:

`netsh wlan show profile [NAME OF YOUR WIFI NETWORK] key=clear`

你会想把[你的 WIFI 网络名称]部分替换成你所连接的任何 SSID 的名称。当你按下回车键时，你会在安全设置栏的“关键内容”列表中看到上述 wifi 网络的密码——这应该很明显。

如果你想尝试另一种方式，你可以通过 Windows 10 设置应用程序调出你的密码。启动它，点击**网络&互联网**，向下滚动一点并点击**网络和共享中心**，点击“连接:”字段旁边的蓝色“Wi-Fi”链接，点击“无线属性”，点击“安全”选项卡，并选择“显示角色”

还有其他实用程序，您可以尝试以更简单的方式获得您的密码，但我应该注意，Windows Defender 可能不太喜欢它们。至少，当我试图下载 Nirsoft 的 [WirelessKeyView](http://www.nirsoft.net/utils/wireless_key.html) 时是这样的——这肯定是一个无害的程序，但一旦它完成向你的系统的传输，就会让 Windows Defender 抓狂。

### 苹果个人计算机

在 macOS 上，显示保存的 wifi 密码很简单。**首先**，你可以拉起终端，输入以下内容:

`security find-generic-password -wa [NAME OF YOUR WIFI NETWORK]`

和以前一样:将[您的 WIFI 网络名称]完全替换为它所显示的内容。接下来你必须以管理员的身份认证进入你的系统，但是一旦你这样做了，你输入的任何 wifi 网络的密码都应该出现在终端中。

您也可以浏览“钥匙串”,特别是“钥匙串访问”应用程序，找出存储的密码。启动应用程序，点击左上角的系统钥匙串。找到要查找的 wifi 网络，双击即可。

当您这样做时，您将看到一个如下所示的框。点击“显示密码”就可以了——当然是在你验证了自己的身份之后。