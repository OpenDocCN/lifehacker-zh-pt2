# 如何修复 Windows 10 最新的“无法连接互联网”错误

> 原文：<https://lifehacker.com/how-to-fix-windows-10s-latest-no-internet-connection-bu-1844458254>

Windows 10 更新往往会打破东西，最近的 Window 10 版本 2004 更新也不例外。根据许多论坛帖子，最新的恼人错误阻止了 Windows 10 应用程序访问互联网，即使当 PC 成功连接并且您的网络浏览器工作正常时。

Watch

令人恼火的是，这个 bug 似乎没有任何警告或理由就出现了。如果你在 Windows 10 系统托盘中看到一个黄色的“无法上网”错误三角形，并且无法在 Steam、Spotify 或*堡垒之夜*等应用程序中连接互联网，但*可以像平常一样浏览网页，那么你就遇到了问题。*

微软在支持论坛帖子 中承认了这个错误 [，并表示它源于 Windows 10 的网络连接状态指示器的问题。该公司正在调查，并将在解决方案设计出来后修补问题，但一些用户已经找到了一个可靠的解决方法，应该在此期间恢复你的应用程序的网络连接。](https://social.technet.microsoft.com/Forums/en-US/4c8654be-d3da-4611-a649-110ca5a7c70a/ncsi-taskbar-icon-may-report-quotno-internetquot-on-windows-10-2004-devices-that-do-have?forum=win10itpronetworking)

### 如何修复 Windows 10 版网络连接缺陷

1.  使用 Windows 任务栏中的搜索栏搜索“注册表编辑器”
2.  从搜索结果中打开注册表编辑器，当提示让应用程序进行更改时，单击**“是”**。
3.  在注册表编辑器应用程序中，转到`HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\NlaSvc\Parameters\Internet`
4.  右键单击**“EnableActiveProbing”**，选择**修改。**
5.  将**“数值数据”**从 0 更改为 1。
6.  点击**“确定”**关闭窗口并保存编辑内容。
7.  关闭注册表编辑器。
8.  重新启动计算机以使更改生效。

幸运的话，重启电脑后，你的应用程序将可以再次连接到互联网。如果没有，请仔细检查您输入的注册表修复是否正确。如果你仍然运气不好，你可能不得不寻找一个不同的解决方案或者等待微软的补丁。如果你碰巧遇到了另一个补丁或者发现了你自己的，请在评论中告诉我们。

[ [Windows 最新](https://www.windowslatest.com/2020/07/18/windows-10-no-internet-connection-problem/)