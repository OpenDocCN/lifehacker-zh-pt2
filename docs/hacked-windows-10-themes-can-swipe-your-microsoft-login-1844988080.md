# 被黑的 Windows 10 主题可以刷你的微软登录

> 原文：<https://lifehacker.com/hacked-windows-10-themes-can-swipe-your-microsoft-login-1844988080>

Windows 10 用户可以用独特的主题定制他们的桌面，并且能够创建和与他人分享这些主题。黑客也可以用它们来窃取你的凭证。



Windows 10 的主题创建功能中存在一个缺陷，黑客可以修改自定义主题，一旦安装，就会通过假冒的登录页面欺骗用户传递他们的 Microsoft 帐户名和密码数据。这种技术对普通人来说不一定会引起任何危险，因为一些合法的 Windows 10 主题会让你在安装后登录。

这种“ [传递哈希](https://www.beyondtrust.com/resources/glossary/pass-the-hash-pth-attack) ”攻击不会一字不差地窃取你的密码，而是窃取密码哈希——你的密码数据的混乱版本。公司对存储在远程服务器上的密码数据进行哈希处理，以使其更加安全，但黑客可以用现成的软件破解密码。在某些情况下，密码可以在几秒钟内被破解。

这个漏洞是由网络安全研究人员吉米·拜恩(Jimmy Bayne)发现的，他在 Twitter 帖子中公开了这一发现。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1302264069311926274&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1302264069311926274&autosize=1) 

Bayne 提醒微软注意安全风险，但该公司表示，它没有计划改变主题功能，因为凭证传递是一个预期的功能；黑客只是找到了恶意使用它的方法。

由于没有采取官方行动，因此用户必须保证自己的安全，远离 Windows 10 的不良主题。

[bleeding computer](https://www.bleepingcomputer.com/news/microsoft/windows-10-themes-can-be-abused-to-steal-windows-passwords)和 [Bayne](https://twitter.com/bohops/status/1302264072218566662) 为 Windows 10 的企业版勾勒出选项，但这些对一般用户不起作用。最明智的做法是完全避免自定义主题，但如果你继续使用它们，请确保你只从安全的来源下载官方主题，如 Windows 商店。

无论你是否继续使用自定义主题，你也应该用 [唯一密码](https://lifehacker.com/how-to-create-secure-passwords-that-arent-impossible-to-1825048324) 更新你的账户，开启 [双因素认证](https://lifehacker.com/no-one-knows-about-two-factor-authentication-and-privat-1838913065) ，使用 [加密密码管理器](https://lifehacker.com/the-five-best-password-managers-5529133) 。我还建议取消第三方帐户与您的 Microsoft 帐户的链接，并使用本地用户帐户登录您的电脑，而不是您的 Microsoft 帐户。像这样的保护措施使得外人更难窃取你的数据，即使他们碰巧得到了密码。