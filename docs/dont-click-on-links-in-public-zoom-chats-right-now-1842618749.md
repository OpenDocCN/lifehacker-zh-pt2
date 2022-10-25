# 现在不要点击公开缩放聊天中的链接

> 原文：<https://lifehacker.com/dont-click-on-links-in-public-zoom-chats-right-now-1842618749>

Zoom 将 URL 转换为超链接的方式中恰好存在一个漏洞，黑客可以使用该漏洞来收集您的 Windows 登录凭据，并可能远程访问您的桌面。在 Zoom 解决这个问题之前，忍住点击来自你不信任的人的网址的冲动——也就是你参加的所有公开的 Zoom 会议，以避免冠状病毒引起的无聊。



缩放将 internet URLs 和 UNC(通用命名约定)路径(例如“C:\Users\Public”)转换为通用超链接。点击其中一个，Windows 就会试图打开这些 UNC 超链接来访问远程文件，这使得 PC 的用户名和密码哈希(基本上是包含用户密码的一堆代码)对从另一端观看的任何人都是可见的。该密码散列可以使用容易获得的软件解密，然后用于远程访问您的 PC 和/或网络。

目前还不清楚 Zoom 公司是否正在解决这个问题——我们希望他们正在解决——但是有一个解决方案可以在此期间保护你的安全。公平的警告:这是一个苦差事设置。

更好的方法是关注聊天中的链接。如果看起来像服务器，类似“\ \ uhoh . com . tk \ images \ awesome . jpg”之类的，就不要点开了。对于未受过训练的人来说，这可能看起来像是一个简单的指向另一个网站的超链接，但它反而促使 Windows 试图通过 SMB 连接到那个远程服务器，从而为密码攻击打开了大门。这些相同的链接甚至可以用来在用户的电脑上启动应用程序，尽管至少你会得到一个弹出警告，你必须在应用程序启动前确认。

### 如何防止 UNC 超链接共享您的 Windows 登录信息

此更改不会阻止缩放显示 UNC 链接，也不会阻止 Windows 尝试访问 UNC 路径。但是，它会阻止您的 Windows 登录凭据与远程服务器或 PC 共享。感谢电脑给 [发出哔哔声，原来指出了](https://www.bleepingcomputer.com/news/security/zoom-lets-attackers-steal-windows-credentials-via-unc-links/)的修复。

1.  在 Windows 10 工具栏中搜索**“注册表编辑器”**。
2.  右键**“注册表编辑器”****以管理员身份运行。**如果 Windows 询问您是否要让应用程序对您的电脑进行更改，请单击**“是”**。
3.  在注册表编辑器窗口中，导航到**“Computer \ HKEY _ LOCAL _ MACHINE \ SYSTEM \ current Control set \ Control \ Lsa \ ms v1 _ 0”**
4.  在 MSV1_0 文件夹中，**右击>新建> DWORD (32 bit)**
5.  将新键命名为**RestrictSendingNTLMTraffic**。
6.  创建完成后，右击**RestrictSendingNTLMTraffic**，点击**“修改”**
7.  将**“值”**字段设置为 **2** 。点击**【确定】**关闭，然后关闭注册表编辑器。

如果此更改导致任何问题，只需删除使用注册表编辑器从 MSV1_0 文件夹中创建的 RestrictSendingNTLMTraffic 注册表项即可撤消。