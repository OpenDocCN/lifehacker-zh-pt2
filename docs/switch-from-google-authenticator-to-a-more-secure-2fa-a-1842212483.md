# 从 Google Authenticator 切换到更安全的 2FA 应用

> 原文：<https://lifehacker.com/switch-from-google-authenticator-to-a-more-secure-2fa-a-1842212483>

根据最近来自 [Nightwatch 网络安全](https://wwws.nightwatchcybersecurity.com/2020/03/03/google-authenticator-for-android-allows-screen-capture/) 的一份报告，谷歌的 Android 认证应用程序存在一个未解决的问题，如果你的设备上安装了任何恶意软件或其他不可靠的应用程序，可能会造成一场巨大的安全噩梦。(安卓系统的 [**微软认证器**](https://play.google.com/store/apps/details?id=com.azure.authenticator&hl=en_US) 应用也存在同样的问题，所以暂时也不要切换到*那个*应用。)

Watch

这两个应用，截至我们写这篇文章时，都没有使用 Android 的 FLAG_SECURE 设置，该设置禁止其他应用(和你)截图。不相信我？在 Android 上拉起 Google Authenticator，按住电源键+底部音量键截图。*轰。*截图。在像 [**Authy**](https://play.google.com/store/apps/details?id=com.authy.authy&hl=en_US) 这样的应用上试试，你可以想按住按钮多久就按住多久——什么都不用做。

虽然谷歌肯定会在*某个时候*修复这个问题，但无论如何，Authy 是一个管理你的 2FA 代码的更好的应用。你不仅可以通过额外的验证步骤来保护应用程序，这样没有你的输入，有人就无法访问你解锁的设备的代码，而且在多个设备上部署应用程序也很容易。一旦您在新设备上安装了应用程序并验证了您就是您，您在主设备上同步的所有 2FA 代码将自动出现在您的新设备上。现在，当你登录网站和服务时，你有两个可以使用的设备，你花在设置上的时间和一开始下载 Authy 的时间差不多。

如果你因为什么原因不想用 Authy，那么至少要测试一下看看你的 authenticator app 是否允许你截图。如果是，考虑别的；如果没有，使用它可能是安全的。