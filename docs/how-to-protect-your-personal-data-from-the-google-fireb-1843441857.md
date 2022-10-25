# 如何保护你的个人数据免受谷歌 Firebase 泄露的影响

> 原文：<https://lifehacker.com/how-to-protect-your-personal-data-from-the-google-fireb-1843441857>

Google Play 商店中近 24，000 个应用程序可能出现了数据泄露。与我们经常报道的主动窃取或分发用户信息的 Play Store 恶意软件和骗局不同，这些应用程序是由于使用最广泛的 Android 应用程序开发平台之一 Google Firebase 的配置不佳而意外泄露数据的。



近三分之一的 Play Store 应用程序使用 Firebase 根据 Comparitech 的 [研究，大约 4.8%的应用程序——大约 24000 个——将你的数据存储在安全措施不当的数据库中。这些不安全的数据库包括大量的个人信息，如您的电子邮件地址、用户名、密码、全名、电话号码、聊天信息副本、街道地址、IP 地址、GPS 数据、信用卡数据等，只需快速的网络搜索即可访问这些数据库。谷歌从其搜索结果中删除了 Firebase 数据库，但它们可以在其他搜索引擎中找到，如 Bing。](https://www.comparitech.com/blog/information-security/firebase-misconfiguration-report/#What_data_is_exposed)

虽然 24，000 个应用程序似乎只是 Play Store 庞大库中的一小部分，但 Comparitech 的团队发现，许多泄漏的应用程序非常受欢迎，在他们测试的应用程序中，共有 42.2 亿次集体下载——最受欢迎的是游戏和教育应用程序。在如此高的数据量下，很有可能你用过的应用程序将你的一些数据存储在了一个易于搜索的数据库中。

### 如何防止你的数据通过 Google Firebase 泄露

不幸的是，完全防止数据泄露的唯一方法是每个应用程序的开发人员更新他们的 Firebase 存储配置；除了不使用这些应用程序(Comparitech 或其他地方没有明确列出)，你没有什么可以阻止这一点。

也就是说，你应该采取同样的预防措施，就像你担心恶意软件 Android 应用程序一样——[，你也应该如此](https://lifehacker.com/how-to-get-rid-of-androids-most-annoying-malware-xhelp-1841699275) :

*   [为你所有的账户创建独一无二的密码](https://lifehacker.com/how-to-create-secure-passwords-that-arent-impossible-to-1825048324) ，并使用加密的 [密码管理器来保证它们的安全](https://lifehacker.com/the-five-best-password-managers-5529133) (并减轻记住它们或以不安全的方式存储它们的压力)。
*   将共享数据和个人身份信息保持在最低限度。这包括联系信息，如您的姓名、地址和个人电子邮件/电话号码；任何财务或支付信息；以及其他用户数据，如 GPS 和网络浏览器历史记录。
*   如果没有必要，不要将你的应用和帐户链接在一起。虽然很方便，但将所有东西都连接起来会让一个人更容易进入多个账户。
*   审查你下载的应用程序。Comparitech 建议只从用户评级高、下载量大的可信发行商那里下载应用程序，但要记住，这些应用程序也可能具有误导性。花额外的时间通读评论， [检查一个应用程序要求什么权限](https://lifehacker.com/use-permissions-to-keep-scammy-apps-off-your-android-1843026818) ，在你安装任何东西之前，在你最喜欢的搜索引擎或网络社区上搜索更多信息。
*   使用 [值得信赖的反恶意软件和反病毒应用](https://lifehacker.com/use-these-antivirus-and-anti-malware-apps-instead-of-av-1841264690) 。虽然这些不一定能防止你的数据被谷歌 Firebase 漏洞暴露，但一个好的防病毒/反恶意软件应用程序将减少将恶意文件和软件下载到你的设备上的机会。

[ [分享](https://www.comparitech.com/blog/information-security/firebase-misconfiguration-report/)