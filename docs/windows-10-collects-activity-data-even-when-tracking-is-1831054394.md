# Windows 10 即使在禁用跟踪的情况下也会收集活动数据，但您可以阻止它[更新]

> 原文:[https://life hacker . com/windows-10-collects-activity-data-even-when-tracking-is-1831054394](https://lifehacker.com/windows-10-collects-activity-data-even-when-tracking-is-1831054394)

又是一天，另一家科技公司对其隐私做法不诚实。这一次是微软，在它发现 [Windows 10 继续跟踪用户的活动](https://www.ghacks.net/2018/12/12/windows-10-activity-may-be-recorded-even-if-you-disable-it/) 后，即使他们在 Windows 10 设置中禁用了活动跟踪选项。

Watch

你可以自己试试。调出 Windows 10 的设置，进入隐私部分，禁用你活动历史中的所有内容。给它几天。访问[Windows Privacy Dashboard online](https://account.microsoft.com/privacy/)，你会发现一些应用、媒体，甚至浏览历史仍然会显示出来。

当然，这些数据可以被手动删除，但它被跟踪的事实对微软来说不是一个好兆头，自从这个疏忽被发现以来，许多用户都在网上表达了他们的沮丧。幸运的是，Reddit 用户 [a_potato_is_missing 找到了一个阻止 Windows 和 Windows Store 跟踪你的 PC 活动的变通办法](https://www.reddit.com/r/Windows10/comments/a4lpg0/windows_10_still_collecting_activity_history/) ，它来自 Tenforums 用户 Shawn Brink 最初发布的一个 [教程。](https://www.reddit.com/r/Windows10/comments/a4lpg0/windows_10_still_collecting_activity_history/)

我们尝试了 Brink 的策略，发现这是一个有效的解决方案，值得那些想要永久限制微软活动跟踪的人分享。这是一个简单的过程，只需要你下载并打开一些文件，但我们会指导你完成这些步骤，因为有一些你想知道的注意事项。

### 如何在 Windows 10 中禁用活动跟踪器

Brink 的方法通过编辑窗口注册表中的值来阻止活动跟踪器(通过. REG 文件)。为了透明起见，下面是文件所做的更改:

*HKEY _ LOCAL _ MACHINE \ SOFTWARE \ Policies \ Microsoft \ Windows \ System*

*publisheuseraventions DWORD*

*0 =禁用*
*1 =启用*

这些变化只适用于活动跟踪，不应该以任何其他方式影响你的操作系统。但是，如果确实出错了，您可以逆转这个过程，这将在步骤 7 中解释。要开始布林克的改造:

1.  将 [布林克教程](https://www.tenforums.com/tutorials/100341-enable-disable-collect-activity-history-windows-10-a.html#option2s2) 中的“**Disable _ Activity _ history . reg**”文件下载到任意文件夹。
2.  双击。REG 文件打开它，然后单击**“运行”**开始将更改应用到您的注册表。
3.  您将得到通常的窗口 UAC 通知，允许文件对您的计算机进行更改。点击**“是”**
4.  将弹出一个警告框，提醒您对注册表进行更改可能会导致应用程序和功能无法工作，或者导致系统错误-所有这些都是真的，但我们在应用此修复程序时没有遇到任何问题。如果你同意，点击**“是”**应用更改。这个过程应该立即发生，之后您将得到最后一个对话框，通知您添加到注册表中的信息。点击**【确定】**关闭文件，结束注册表变更。

5.  注册表编辑完成后，你需要退出 Windows(按下 **Windows 键+X** 然后**关机或退出>退出**)，然后重新登录以应用注册表更改。
6.  当您重新登录时，Windows 将不再跟踪您的活动，甚至是之前漏掉的内容。
7.  要撤销注册表更改并重新启用活动跟踪器，请下载“**Enable _ Activity _ history . reg**”文件，该文件也可以在 [Tenforums 教程](https://www.tenforums.com/tutorials/100341-enable-disable-collect-activity-history-windows-10-a.html#option2s2) 中找到，然后按照上面相同的步骤操作。

**更新 2018 年 12 月 13 日中午 12:30 PT:**微软已经向 [Neowin](https://www.neowin.net/news/microsoft-says-windows-10-is-not-sending-your-data-to-the-cloud-when-you-tell-it-not-to) 发布了关于前述“活动历史”的声明以下是 Windows &设备集团隐私官玛丽莎·罗杰斯的声明:

*“微软致力于保护客户隐私，我们为了您的利益而收集和使用的数据是透明的，我们给予您管理数据的控制权。在这种情况下，Windows 10 和 Microsoft Privacy Dashboard 使用了相同的术语“活动历史”。Windows 10 活动历史数据只是 Microsoft Privacy Dashboard 中显示的数据的子集。我们正在努力在未来的更新中解决这个命名问题。”*

正如 Neowin 指出的，微软表示，如果你想阻止你的电脑上传你的活动数据，你应该考虑两个设置:

“一种是转到“设置”->“隐私”->“活动历史记录”，并确保“让 Windows 将我的活动从这台电脑同步到云”处于未选中状态。此外，你可以进入“设置”->“隐私”->“诊断与反馈”，并确保它设置为“基本”