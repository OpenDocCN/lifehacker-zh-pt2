# 不要安装微软 Surface 8 月份的固件更新

> 原文:[https://life hacker . com/do-not-install-your-Microsoft-surfaces-August-updates-1837281948](https://lifehacker.com/do-not-install-your-microsoft-surfaces-august-updates-1837281948)

如果你有一台微软最新的 Surface 设备 Surface Book 2 或 Surface Pro 6——你会想暂停一会儿 Windows 更新，因为微软的最新固件绝对会让你的系统性能大打折扣。然而，如果你的笔记本电脑已经被冲洗过了，我们有一些如何修理它的方法。

Watch

你如何知道你有一个迫在眉睫的固件更新？请检查 Windows Update。你不能错过它，尽管也欢迎你将你的待定更新列表与微软为你的 Surface 设备提供的 2019 年 8 月固件更新列表进行交叉引用。

当你从微软八月份的列表中看到任何固件更新时，你会想要确保你不会意外地安装它们。如果你从 4 月份就开始更新 Windows 10 Home，你会在 Windows Update 的下载按钮下方看到一个“暂停更新 7 天”选项。按一次，然后按任意多次，以防止更新在 35 天内自动安装到您的系统上。

这应该会给微软足够的时间来解决困扰一些 Surface Book 2 和 Surface Pro 6 用户的问题，包括 [将你的 CPU 频率](https://www.reddit.com/r/Surface/comments/cqr3rh/microsoft_surface_pro_6_and_surface_book_2/) 锁定在仅仅 400 MHz——非常慢。

此外，其他用户报告说，8 月份的更新使连接到 5GHz wifi 网络变得困难，这是另一个大问题，因为这是你能够在无线交流路由器上从笔记本电脑中获得 [最佳 wifi 性能](https://lifehacker.com/which-wifi-band-should-i-use-for-my-devices-1832635625) 的唯一方法。

### 如果我已经安装了更新，该怎么办？

如果您因为安装了 8 月份的固件更新而看到令人难以置信的性能下降或遇到 wifi 问题，您有几个可能的解决方案。公平的警告:第一个不漂亮。

#### 修复你超慢的 CPU

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-jcAtuUjthcI&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-jcAtuUjthcI&start=0) 

那些因为笔记本电脑的 CPU 突然运行在 400Mhz(任务管理器中的 0.4GHz)而不是 1.6-4.2 GHz(取决于您的系统规格)而经历痛苦减速的人应该尝试等待微软发布更新来修复这一混乱。我还没有看到具体的时间表，但微软表示，它正在迅速解决这个问题。

如果你陷入困境，需要马上使用你的笔记本电脑，一些受影响的用户建议你可以硬重置系统来解决这个问题。按住电源按钮大约 20 秒钟，然后重新开机。(如果这实际上修复了操作系统中可能的节流问题，我会感到惊讶，但这位 Reddit 用户 声称它可以工作，所以值得一试。不过，节流问题可能会在某个时候*卷土重来。)*

你也可以尝试使用 [ThrottleStop](https://www.techpowerup.com/download/techpowerup-throttlestop/) 应用程序来禁用 BD PROCHOT，它会告诉你的系统在检测到你的处理器过热时限制你的 CPU。这可能会解决你的问题，因为 [之前也有类似的问题](https://www.reddit.com/r/Surface/comments/8fvsji/surface_book_2_locks_to_400mhz/) ，但不清楚 [是否会直接解决](https://www.reddit.com/r/Surface/comments/95b7wi/sb2_15_bd_prochot_disabled_and_still_04_ghz/) 从 2019 年 8 月更新开始导致 CPU 节流的任何问题。尽管如此， [我还是要试一试](https://www.reddit.com/r/Surface/comments/cn9i4z/feel_like_this_cpu_throttling_issue_should_be/ew89osr/) ，如果或者当微软发布其修复程序时，不要忘记重新启用 BD PROCHOT。

否则，你也可以采取 [重置你的系统](https://www.reddit.com/r/Surface/comments/95b7wi/sb2_15_bd_prochot_disabled_and_still_04_ghz/e3tgljm/) 的艰苦过程——格式化你的驱动器并重新安装 Windows 10，然后不安装 8 月更新(如前所述)。你必须重新设置你的系统，重新安装你所有的应用程序，并且，很明显，从你之前应该做的备份中恢复你的文件。除非你别无选择，否则我不会走这条路，但这不是最糟糕的主意，因为运行在 0.4GHz 的系统基本上是不可用的。不幸的是，这对你来说可能太慢了，以至于*无法让*成为你文件的有效备份，所以这个选项可能不是最好的。

#### 来修理你的破无线网络

这个修复要容易得多。如果您在安装任何 2019 年 8 月更新后无法连接到 5GHz wifi 网络，请通过“开始”菜单调出“设备管理器”，单击“网络适配器”，选择您的无线交流网络控制器(可能是 Marvell)，右键单击，选择“属性”，单击“驱动程序”选项卡，然后选择“回滚驱动程序”选项。

您可能还需要为您的 Marvell 蓝牙驱动程序重复相同的过程，以防这也导致您的整体连接问题(如一些报告所述)。