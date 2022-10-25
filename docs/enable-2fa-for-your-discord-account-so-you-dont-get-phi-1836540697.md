# 如何在你的不和谐账户上启用双因素认证

> 原文：<https://lifehacker.com/enable-2fa-for-your-discord-account-so-you-dont-get-phi-1836540697>

好消息是什么？最近的一次网络钓鱼尝试击中了 Discord，并且只困住了一小批用户——总共大约 2500 人。坏消息呢？没有简单的工具来判断你是否在那个名单上，所以你最好现在就花点时间在服务上重置你的密码。更重要的是，是时候停止懒惰，启用双因素身份认证，这可以帮助保护您免受未来的网络钓鱼企图。



正如今天 [Vice](https://www.vice.com/en_us/article/evye3a/hackers-publish-list-of-discord-email-addresses-passwords-login-credentials?utm_source=mbtwitter) 报道的那样，受骗用户的名单很小，甚至充满了意识到自己被钓鱼的聪明的不和谐用户:

> “一些无效的登录信息显然是伪造的，比如‘fucking @ phish . io’和‘fucku’这样的电子邮件，很可能来自那些试图向黑客提供垃圾数据的人。”

不幸的是，名单上也有合法账户。即使你的安全没有受到影响，也很有可能是安全的，特别是如果你最近没有向任何网站或服务提供不和谐的登录和密码，像这样的时刻是考虑你的安全实践的绝佳机会:

*   你使用的 [是不是一个很容易猜到的密码](https://lifehacker.com/instead-of-changing-your-passwords-upgrade-them-1836182279) ？
*   您在 Discord 上使用的密码是否与您在其他服务上使用的密码相同？
*   你是否正在使用 [一个密码管理器](https://lifehacker.com/the-five-best-password-managers-5529133) 来存储你应该为每个服务使用的 [唯一密码](https://lifehacker.com/how-to-create-secure-passwords-that-arent-impossible-to-1825048324) ？
*   您是否启用了 [双因素认证](https://lifehacker.com/two-factor-authentication-isnt-enough-to-keep-your-acco-1827867557) ？

### 在不和谐时更改您的密码

要更改您的不和谐密码，请调出 [网站](https://discordapp.com/activity) 或桌面应用程序，并点击屏幕左下角您姓名右侧的齿轮图标。然后，点击“我的帐户”部分的编辑按钮:

从那里，寻找“更改密码？”链接。单击它，键入您的当前密码和新密码，然后单击保存以确认您的更改。

### 向您的 Discord 帐户添加双因素身份验证

是的，只要 Discord 检测到来自新 IP 地址的登录尝试，它就会向您发送电子邮件。启用双因素身份验证仍然是一个更好的做法，因为任何有权访问您的电子邮件的人(尤其是如果您已经为多个服务使用了同一个密码)都可以批准该请求。

使用 2FA，攻击者需要能够实际访问您的设备和验证器应用程序，才能以您的身份登录。虽然 [攻击者仍然有可能说服你](https://www.allthingsauth.com/2018/04/05/totp-way-more-secure-than-sms-but-more-annoying-than-push/#vulnerabletophishingandmitmattacks) 在一个实际上没有冲突的网站或应用程序中键入你的 2FA 安全码，但 2FA 至少会帮助你保持一点安全——除此之外，你有责任确保你在正确的网站上输入你的凭据。

要开始使用 Discord 上的 2FA，请在服务的“我的帐户”屏幕中寻找双因素认证部分。单击“启用双因素身份验证”按钮。

点击它，你会看到标准的二维码提示，你应该习惯看到你是否为你的其他帐户启用了双因素身份验证(你应该这样做！).用你最喜欢的认证器 app 扫描它——我们喜欢 [Authy](https://authy.com/) ，但是还有 [大量的替代品](https://lifehacker.com/two-factor-authentication-isnt-enough-to-keep-your-acco-1827867557)——输入它给你的代码，确认它能工作。

然后会提示你注册短信认证作为备份方法，这比 2FA 应用程序更不安全。你还会被要求下载你的备份代码，这是你绝对应该做的，以防你失去对 authenticator 应用程序的访问权，无法再登录 Discord。