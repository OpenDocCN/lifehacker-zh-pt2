# 防止您的 Mac 制作加密电子邮件的纯文本副本

> 原文：<https://lifehacker.com/prevent-your-mac-from-making-plain-text-copies-of-your-1839779443>

IT 大师 Bob Gendler 上周在媒体上分享了一个关于苹果邮件的惊人发现。如果你将应用程序配置为发送和接收加密的电子邮件——没有正确的解密密钥，任何人都无法读取这些信息——苹果的数字助理会将你的电子邮件*以纯文本*的形式存储在你的 Mac 硬盘上。



更令人沮丧的是，你可以在 Mac 上完全禁用 Siri，而你的消息仍会出现在名为 *snippets.db 的 Mac 数据库中。一个名为【T2 建议】的*进程仍会梳理你的电子邮件，并将它们转储到这个明文数据库中。根据 Gendler 的说法，这个问题出现在 macOS 的多个迭代中，包括最近的 Catalina 和 Mojave 版本。

正如詹德勒 [写的](https://medium.com/@boberito/apple-mail-stores-encrypted-emails-in-plain-text-database-fix-included-3c2369ce26d4) :

> “我在 7 月 25 日发现了这个数据库及其存储内容，并开始在多台安装了苹果邮件的电脑上进行广泛测试，并在 7 月 29 日完全确认了这一点。那周晚些时候，我确认了这个数据库存在于 10.12 到 10.15 版本的机器上，并且以相同的方式运行，存储未加密的加密消息。如果你启用了 iCloud 和 Siri，我知道会有一些数据发送给苹果，以帮助改进 Siri，但我不知道这是否包括来自这个数据库的信息。”

### 考虑把 Siri 从你的电子邮件中删除

虽然苹果目前正在努力解决 Gendler 提出的问题，但有两种简单的方法可以确保你的加密电子邮件不会以不加密的形式存储在 Mac 上。首先，您可以在“系统偏好设置”的“Siri”部分中停用邮件的 Siri 建议。

其次，您可以启动终端并输入以下命令:

`defaults write com.apple.suggestions SiriCanLearnFromAppBlacklist -array com.apple.mail`

还有第三种方法可以使用——安装一个 [系统级配置文件](https://github.com/boberito/ConfigurationProfiles/blob/master/suggestd.mobileconfig)——Gendler 在他的帖子中详细介绍了这种方法。

无论你选择哪一个选项，你都会想要删除 *snippets.db* 文件，因为禁用 Siri 的收集功能不会自动删除已经被*收集的内容(显然)。你可以通过打开苹果电脑的驱动器( **Go > Computer** )快速搜索“snippets . db”
来找到它*

苹果还告诉 [The Verge](https://www.theverge.com/2019/11/8/20954130/apple-mail-encrypted-unencrypted-email-macos-siri-text) 你还可以限制哪些应用程序被允许在你的 Mac 上拥有完整的磁盘访问权限——通过**系统偏好设置>安全&隐私>隐私选项卡**——以确保它们不能访问你的 snippets.db 文件。您还可以打开 FileVault，这将防止您的电子邮件在 snippets.db 中显示为明文。