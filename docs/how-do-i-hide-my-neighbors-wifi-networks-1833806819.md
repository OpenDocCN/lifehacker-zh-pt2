# 如何隐藏邻居的 Wifi 网络？

> 原文：<https://lifehacker.com/how-do-i-hide-my-neighbors-wifi-networks-1833806819>

我在这个 [**Tech 911**](https://lifehacker.com/c/tech-911) 建议专栏里讲了很多关于无线网络的内容。本周也不例外。就在我认为我们已经涵盖了一切的时候，一个读者问题突然出现了，需要引起注意——部分是因为这是一个古怪的问题，部分是因为我喜欢用一杯新鲜的 wifi 相关建议开始我的周五早晨。

Watch

本周的问题来自 Lifehacker 的读者 Ricky，他写道:

> *“有没有办法不让邻居的网络显示在我的 wifi 列表中？我刚刚读了你的文章* *关于一个人的邻居信号太强以至于屏蔽了他的，我的问题不是这个。实际上，我似乎不得不频繁地更换频道，因为我的邻居总是跟着我的频道，每当我更换频道以获得更清晰的信号时，他们都会换到同一个频道*

隐藏邻居的 wifi 网络，不要和 [屏蔽](https://lifehacker.com/how-do-i-block-my-neighbors-wifi-1833464189) 混为一谈，是完全可能的。不应该是这样。毕竟，如果你保存了凭证，你的设备会自动连接到*你的*无线网络。在 Windows 的“wifi 连接框”中，由于缺乏更好的名称，你的操作系统会自动将它看到的所有 wifi 网络从信号强度最强到最弱进行排序(减去任何隐藏的网络)。除非你的邻居在你的房子里有一个接入点，否则你应该在顶部或附近看到你的 wifi 网络。

诚然，你可能会尝试在 wifi 网络的边缘连接，这意味着它的信号强度会很低，你的设备会在你的网络之前显示所有更强的相邻网络。我知道这有多烦人。不过，如果你像大多数人一样在 Windows 中保存 wifi 网络的密码，不管信号强度如何，这些网络都会出现在连接列表的顶部。

对于你的具体问题，有一种方法可以在 Windows 的潜在连接列表中隐藏各种无线网络。(我还没有找到在 Mac 上做到这一点的好方法，但我会继续探索。)

不过，给你个警告。隐藏 wifi 网络有点麻烦，因为你必须单独隐藏每个无线网络。一旦你做到了，你就万事俱备了(直到你的邻居把他们的 wifi 换成另一个聪明的名字，比如“吴”)

首先用管理员权限打开命令提示符。单击星号按钮，键入“命令提示符”，右键单击应用程序，然后选择“以管理员身份运行”然后，在命令提示符下键入以下内容:

`netsh wlan show networks`

这将为您提供一个列表，列出您的系统检测到的所有 wifi 网络，无论这些网络在哪里，您都应该将其复制并粘贴到一个临时文本文件中。(您将在“SSID #”列表后看到每个名称；您可以忽略其他“网络类型”、“身份验证”和“加密”条目。)

完成后，您可以在命令提示符下键入以下内容:

`netsh wlan add filter permission=block ssid="[[[NAME]]]" networktype=infrastructure`

显然，您会想要将[[[NAME]]]部分替换为您想要隐藏的任何 wifi 网络的名称。保留报价。

如果您想查看您添加到这个黑名单中的无线网络，您可以使用以下命令:

`netsh wlan show filters`

要从过滤器中删除无线网络，您将使用以下命令:

`netsh wlan delete filter permission=block ssid="[[[NAME]]]" networktype=infrastructure`

和以前一样的交易；确保您使用的是您阻止的实际 SSID，而不是[[[NAME]]]，但要保留引号。此外，大小写也很重要 SSID 的名称必须与过滤器上的名称完全匹配。

如果你想变得更疯狂，你还可以使用过滤器来阻止每一个没有被你特别列入白名单的无线网络。只有当你打算永远在同一个地方使用笔记本电脑或台式机时，这才有意义。否则，下次你带着你的笔记本电脑去任何地方并需要连接到一个新的 wifi 网络时，这将是一个彻底的痛苦。

如果您想走这条路，首先使用以下命令将您想要的各种 wifi 网络添加到白名单中:

`netsh wlan add filter permission=allow ssid="[[[NAME]]]" networktype=infrastructure`

然后，使用此命令阻止所有其他内容:

`netsh wlan add filter permission=denyall networktype=infrastructure`

一旦你意识到这是一个多么糟糕的决定，你可以用这个命令来回复你的愚蠢:

`netsh wlan delete filter permission=denyall networktype=infrastructure`

另外，我应该注意到这种过滤是系统范围的。当你点击桌面右下角的普通图标时，你不仅会看到(或看不到)各种 wifi 网络，而且这些网络还会从你可能正在使用的任何 wifi 扫描应用 的 [中出现和消失:](https://lifehacker.com/which-wifi-channels-should-i-use-for-my-wireless-networ-1832788063)

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>

<small></small>