# 如何快速移除 Windows 10 的新 Cortana 应用

> 原文:[https://life hacker . com/how-to-fast-remove-windows-10s-new-cortana-app-1843906742](https://lifehacker.com/how-to-quickly-remove-windows-10s-new-cortana-app-1843906742)

新的 Windows 10 V 版本 2004 更新正在缓慢地向兼容的设备推出，尽管一些用户将会在 [等待更长的时间](https://lifehacker.com/how-to-install-the-windows-10-may-2020-update-if-its-mi-1843732242) 。此次更新为操作系统带来了几个新功能，包括微软全新版本的数字助理 Cortana，不管你喜欢与否。

Watch

Cortana 现在成为一个独立的应用程序，它不再是语音控制的。它还放弃了许多与其他第三方服务的集成，转而专注于工作流帮助和基于文本的命令。

以这种方式分割 Cortana 是明智的；这并不像任何人真的用它来控制他们的音乐或打开其他应用程序，也许调整后的焦点将帮助微软找到助手的一个好用途。然而，尽管现在是“可选的”，新的 Cortana 应用程序在默认情况下是作为 Windows 10 2004 更新的一部分安装的 ，而就在那里，随时准备在你每次启动电脑时提供帮助。然而，如果你不打算使用助手，有一个简单的方法可以防止这种情况发生。

### 如何关闭或卸载新的 Cortana 应用

要禁用新的 Cortana 应用程序，你需要在打开设备时阻止它自动启动。最简单的方法是通过 Windows 任务管理器:

1.  按 **Ctrl+Shift+Esc** 打开任务管理器。
2.  点击**“启动”**选项卡
3.  滚动列表，直到找到“Cortana”
4.  右键点击**“Cortana”，**然后选择**“禁用”**
5.  关闭任务管理器。

你也可以打开设置应用，点击**应用>启动**来完成同样的事情。

完全卸载 Cortana 有点复杂。您希望以管理员身份启动 PowerShell(在开始菜单中右键单击它并选择该选项)，然后键入以下内容:

`Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage`

一旦你做到了这一点，不要忘记右键单击你的 Windows 任务栏并取消选中“显示 Cortana 按钮”，因为一旦你 [将应用程序发送到幻影 Zo ne](https://www.youtube.com/watch?v=2u3eQc_rx54) 中，单击该按钮将不会做任何事情。