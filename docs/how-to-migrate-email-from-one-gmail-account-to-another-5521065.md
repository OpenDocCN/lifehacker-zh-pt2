# 如何将邮件从一个 Gmail 帐户迁移到另一个帐户

> 原文:[https://life hacker . com/how-to-migrate-email-from-one-Gmail-account-to-another-5521065](https://lifehacker.com/how-to-migrate-email-from-one-gmail-account-to-another-5521065)

无论你是将 [从工作邮箱迁移到私人邮箱](https://lifehacker.com/how-can-i-save-all-my-emails-for-a-personal-backup-5990556) ，还是只是不喜欢你选择的用户名，想换一个听起来更专业的用户名，你并不是唯一一个在寻找将所有 Gmail 数据从一个地方转移到另一个地方的人。

Watch

我们已经在 [上讲解了如何为你的工作电子邮件创建个人备份](https://lifehacker.com/how-can-i-save-all-my-emails-for-a-personal-backup-5990556) 和 [如何使用谷歌外卖](https://lifehacker.com/how-to-back-up-your-gmail-and-view-mbox-files-1827660389) 下载 Gmail 邮件，然后将其恢复到新帐户中。但如果你只是想让旧 Gmail 帐户的邮件出现在新 Gmail 帐户的收件箱中，最简单的选择是设置 POP(也就是邮局协议)访问。

以下是方法。

### **在旧的 Gmail 设置中配置 POP 访问权限**

从原始 Gmail 帐户(您要转发的帐户)的收件箱开始。点按邮件窗口右上角的齿轮图标，然后选择“设置”>“转发和 POP/IMAP”。

*   切换**启用所有邮件的 POP**。
*   在#2 下的下拉列表中选择如何处理原始邮件。您可以保留、存档或删除该收件箱的 Gmail 副本，或者将邮件标记为已读。
*   点击窗口底部的**保存更改**按钮。

### **将邮件导入您的新 Gmail 帐户**

登录您的新 Gmail 帐户，打开设置>帐户并导入。

*   在检查来自其他帐户的邮件下，选择**添加邮件帐户**。
*   输入您要导入的 Gmail 地址。单击下一步。
*   选择**从我的其他帐户(POP3)导入电子邮件**。

*   输入您的帐户密码，并确定“取回邮件时总是使用安全连接(SSL)”已选定。所有其他切换选项取决于您管理和组织邮件的个人偏好。
*   点击**添加账号**。
*   在下一个屏幕上，选择是否希望该选项使用旧别名发送消息，然后单击下一步>下一步。

注意:如果你对 Gmail 使用双因素认证(而你 [绝对应该对 Gmail 使用双因素认证](https://lifehacker.com/no-one-knows-about-two-factor-authentication-and-privat-1838913065) ！)，你的常规密码在这里就不管用了。你需要进入你的 [谷歌账户](https://myaccount.google.com/) >安全>登录谷歌>应用密码。登录您的帐户，选择需要密码的应用程序和设备，然后选择生成。

### **确认您的账户之间的关联**

一旦您选择使用备用地址发送邮件，您将需要通过几个额外的步骤来验证您的两个帐户是否属于您。Gmail 将向您的旧地址发送一封确认电子邮件，其中包含确认码和验证链接。

如果您在单击“后续步骤”后仍未关闭上一步骤中的弹出窗口，则可以在那里输入确认码。如果您关闭了它，您可以点击验证电子邮件中的链接，或者转到“设置”>“帐户”,导入您的新帐户，点击您要导入的电子邮件地址旁边的“验证”,然后按照提示输入您收到的确认码。(后一种做法可以防止混淆你登录的是哪个帐户。)

### **其他邮件客户端的替代选择**

如果你使用 Outlook、Thunderbird 或 Apple Mail 之类的邮件客户端在账户之间拖放邮件，还有另一种(更笨拙的)方法。你必须设置你选择的桌面客户端来通过 IMAP 访问你的两个 Gmail 账户。谷歌在这里 详细介绍了流程 [，我们就不一一赘述了。还要注意，为了达到最佳效果，你需要在 Gmail 的设置>](http://mail.google.com/support/bin/answer.py?answer=75726) [标签](https://mail.google.com/mail/#settings/labels) 中为你的所有标签(包括已发邮件和所有邮件)启用“在 IMAP 中显示”。

这篇文章最初发表于 2010 年 4 月，并于 2022 年 3 月 3 日更新了最新信息。