# 如何在你的 Android 上防止基于波束的攻击

> 原文：<https://lifehacker.com/how-to-prevent-beam-based-hacks-on-your-android-1839608741>

今天在“更新你的设备总是一个好主意”中，最近发现了 Android 基于 NFC 的文件共享功能的一个漏洞， [Android Beam](https://developer.android.com/training/beam-files) ，使得有人可以在你的设备上安装应用程序。谷歌在上个月发布的 Android 更新中已经发现并修复了这个漏洞，所以勤奋的更新者已经被覆盖了。如果你还没有，现在是时候这么做了。

Watch

[ZDNet](https://www.zdnet.com/article/android-bug-lets-hackers-plant-malware-via-nfc-beaming/) 报道的 bug，确实是对 Beam 的安全权限的错误分类。对于大多数基于 NFC 的交易，用户应该会收到一个提示，警告他们信息正在被传输。特别是应用程序，Android 应该会阻止安装来自 Google Play 商店之外的“未知来源”的应用程序，除非你确认你想要它们。

在 Android 8.0 及更高版本中，Android 将 Google Beam 列入白名单，使其与 Play Store 一样值得信赖。因此，如果有人通过 Beam 发送应用程序，一旦你确认了该应用程序，它就会自动安装，而不会发出任何安全警告。作为一个总是半读通知的人，我可以证明这样一个事实，即使是最有安全意识的人也会不小心安装恶意软件。

Google 在[2019 年 10 月安卓更新](https://source.android.com/security/bulletin/2019-10-01#2019-10-01-details) 中更新了 Beam 的权限。如果您的手机保持最新，问题就已经解决了。(如果你上周没有更新，我建议你检查一下，以防万一。)

如果你不使用 NFC 文件共享，你也可以完全禁用它，方法是进入设置应用程序，点击“连接”，然后点击“NFC 和支付”，然后关闭 Google Beam。关闭 Beam 将阻止所有通过 NFC 进行的文件共享，而不会禁用其他基于 NFC 的应用，如 Google Pay。