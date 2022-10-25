# 如何立即在 Android 上手动启用 RCS(更新)

> 原文：<https://lifehacker.com/how-to-manually-enable-rcs-on-android-right-now-update-1839416118>

谷歌宣布计划推动 RCS 的采用已经有一段时间了，这样 Android 用户就可以最终摆脱过时的短信技术，但大多数用户都在等待他们的移动运营商在 2020 年的某个时候打开开关。碰巧有一种手动打开 RCS 的方法，但是正如许多用户——以及我们的许多读者——已经发现的那样，它充其量是不一致的。



如果你不确定 RCS 是什么或者你为什么想要启用它， [我们的 RCS 初级读本有所有的细节](https://lifehacker.com/whats-rcs-messaging-and-why-should-you-care-1832235783) ，但最重要的原因是 RCS 文本消息比 SMS 更好，支持更多的功能。你知道苹果的 iMessage 如何让你看到你的朋友在多台设备上打字或进行对话吗？RCS 让 Android 用户最终可以在他们的核心短信应用程序中完成这两项任务——甚至更多。

谷歌不久前更新了 Android messages 应用程序的 RCS 支持，但这取决于每个移动运营商在其网络上启用它。然而， [Android Police 最近报告了](https://www.androidpolice.com/2019/10/26/screw-your-carrier-heres-how-to-enable-rcs-in-the-messages-app-yourself-right-now/)Reddit 用户在他们的 Android Messages 应用中成功启用了 RCS 功能，无需运营商批准。从那以后， [这一招似乎在一些手机](https://9to5google.com/2019/10/31/enabling-rcs-trick-breaks/) 上不再奏效，大多数情况下是在一加的设备上，尽管据报道在 Pixel 手机和三星 Galaxy 机型上也出现了这种情况。

尽管存在这些问题，这个技巧对许多用户来说仍然是可能的，尽管这个过程可能需要尝试几次才能坚持下来。

### 如何在 Android 上手动启用 RCS 消息传递

1.  在此过程中，您需要关闭设备的 Wi-Fi。在手机屏幕上向下滑动以显示快速设置和通知菜单，然后找到并点击**“Wi-Fi”**快捷方式将其禁用。
2.  接下来，**打开** [**活动启动器 app**](https://play.google.com/store/apps/details?id=de.szalkowski.activitylauncher&hl=en_US) ，从下拉菜单中选择**【所有活动】**。
3.  点击**“信息”**，然后向下滚动并点击**“设置 RCS 标志”**
4.  向下滚动到“ACS Url”，从下拉菜单中选择**“http://RCS-ACS-prod-us . sandbox . Google . com”.**。
5.  强制关闭消息。
6.  如果你还没有安装 [“运营商服务”](https://play.google.com/store/apps/details?id=com.google.android.ims&hl=en_US) 应用程序，那么进入设置，搜索**“所有应用程序”**查找运营商服务，清除其 app 数据。
7.  重新打开邮件并重复步骤 2 和 3。
8.  接下来，在“OTP 模式”下拉菜单中，选择**“您的\ s messenger \ s verification \ scode \ sis \ sG-(\ d { 6 })”**
9.  向下滚动并点击**“应用”**
10.  强制关闭“信息”应用程序，然后重新打开它。如果有一个横幅要求您“立即升级”，这样您就可以看到您的朋友在键入什么，点击**“立即升级”**如果没有，请参考上述步骤，再次确认您没有遗漏任何东西。

升级后，您可以点击**“...>设置>聊天功能**在 Messages 应用中查看哪些 RCS 功能对你可用。如果你在屏幕上方看到一条警告信息，这可能意味着你的电话号码无法被验证，不过不要担心，这是可以解决的。首先，确保你正确地遵循了上述步骤。如果这不能解决任何问题，请执行以下操作:

*   强制关闭信息，然后再次尝试清除运营商服务的应用数据。重启你的手机。
*   手机重启后，再次打开“信息”应用程序，进入**“...>设置>聊天功能>状态:设置**然后点击**“验证”**，输入你的电话号码。

如果你已经完成了所有这些步骤，但似乎仍然无法让 RCS(或“信息”应用程序)工作，或者你的手机直接告诉你你的运营商不支持 RCS，那么你可能就不走运了，只能等待你的运营商将来启用 RCS 支持。在这种情况下，您可以按照上面的步骤回溯整个过程，但是在步骤 4 中删除“ACS Url”字段，在步骤 8 中删除“OTP 模式”。

*更新于 2019 年 11 月 1 日，更新了修订的步骤、故障排除和如何撤销该技巧，以及新的信息和相关链接，因为有报告称变通办法已在一些设备上停用。*