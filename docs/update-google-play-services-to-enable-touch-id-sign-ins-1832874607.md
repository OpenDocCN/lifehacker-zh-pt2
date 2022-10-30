# 更新 Google Play 服务，为网站启用 Touch-ID 登录

> 原文：<https://lifehacker.com/update-google-play-services-to-enable-touch-id-sign-ins-1832874607>

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-5ZIQabDrnT0&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-5ZIQabDrnT0&start=0) 

今天， [FIDO 联盟和环球网财团(WC3)](https://fidoalliance.org/android-now-fido2-certified-accelerating-global-migration-beyond-passwords/)
[宣布](https://fidoalliance.org/android-now-fido2-certified-accelerating-global-migration-beyond-passwords/)Android OS 已经获得 [FIDO2 认证](https://fidoalliance.org/fido2/) 。这将使 Android 用户能够使用他们的指纹——而不是密码— 登录网站和其他服务,开发人员现在可以在他们的 web 应用程序和登录页面中添加无密码认证,以及在 Google Play 服务自动更新后添加他们的原生 Android 应用程序。



虽然许多 Android 设备和应用程序之前都包含了基于指纹的登录，但 FIDO2 的实现是不同的，它在 Android 上的采用意味着我们可能正在慢慢接近密码过时的未来。

### **如何在 Android 上设置无密码网络登录**

一旦 FIDO2 支持扩展到您的设备，您将只能使用指纹 ID 登录允许它的网站——尽管更多人可能会开始实现指纹登录，因为大约 10 亿台新设备将很快支持该功能。要在这些网站上使用无密码登录，您需要:

1.  至少运行 Android 7.0 或更高版本的设备。
2.  最新的 Google Play 服务更新。这些更新通常会自动完成，但你可以通过在你的设备上打开该应用程序的 Google Play 商店页面 来仔细检查是否有新版本。
3.  接下来，如果你还没有在你的安卓设备 上设置你的指纹档案，你需要 [。](https://lifehacker.com/whats-the-best-way-to-unlock-your-android-phone-1828856042)
4.  一旦你存储了你的指纹 ID，你现在就可以在浏览 Chrome、Firefox 和 Microsoft Edge 时使用你的 Android 设备的指纹传感器登录网站和基于网络的应用程序(前提是网站首先支持无密码认证)。

### 安全吗？

像任何安全措施一样，指纹识别也有风险，所以用另一种方法——密码、pin 码、人脸识别或猜谜语桥牌——是最佳实践。然而，FIDO2 协议非常安全，通过防止用户在不安全的 web 域和带有可疑(或网络钓鱼)URL 的网站上使用基于指纹的 web 登录，增加了一层额外的保护。FIDO2 还可以在出现安全漏洞时保护您的安全。与要求用户和应用/服务都知道密码的密码系统不同，FIDO2 只要求用户输入正确的认证信息。

本质上，使用你的 Android 设备的指纹传感器的工作方式与解锁你的锁屏或登录某些应用程序的工作方式大致相同:y 我们的个人信息和指纹档案数据存储在本地设备上，永远不会与你登录的应用程序或网站共享。相反，你的设备会检查指纹是否与它存储的打印 ID 或登录密钥匹配，然后通过应用程序或网站确认一切正常，并让你登录(或者在信息不匹配的情况下，将你锁定)。

万一你需要更多的保证指纹认证是安全的，我们有一些让你的指纹数据尽可能安全的。