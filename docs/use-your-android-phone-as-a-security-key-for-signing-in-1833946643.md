# 使用您的 Android 手机作为登录网站的安全密钥

> 原文：<https://lifehacker.com/use-your-android-phone-as-a-security-key-for-signing-in-1833946643>

所有运行 Android 7.0 或更高版本的 Android 智能手机 [现在都可以用作安全密钥](https://cloud.google.com/security-key/) 登录网站——只有谷歌的，目前只能通过 Chrome，但希望更多的网站和浏览器很快会支持该功能。这是一种方便的双因素身份认证方法，因为大多数人即使在桌面上浏览时，也将他们的 Android 手机或平板电脑放在手边，并且它减轻了处理其他硬件令牌或身份认证应用程序的需要。



这项新功能是 Android 最近获得 FIDO2 和 WebAuth 认证的结果。如果你想知道这项技术是如何工作的，我们有 [快速解释器](https://lifehacker.com/update-google-play-services-to-enable-touch-id-sign-ins-1832874607) ，但是电梯推销是你的 Android 手机与 Chrome 通信以验证你的身份和你登录的网站的合法性。这两个设备检查:

*   您与通过蓝牙和位置数据登录的设备位于同一位置
*   您正在登录的网站是安全可信的(而不是试图骗取您密码的虚假登录页面)

### 如何将您的 Android 智能手机用作安全密钥

#### **你需要什么**

*   Android 7.0 或更高版本的 Android 智能手机(支持蓝牙)
*   最新版 [谷歌浏览器](https://www.google.com/chrome/)
*   启用了 [两步验证](https://myaccount.google.com/signinoptions/two-step-verification) 的谷歌账户

要将您的智能手机添加为安全密钥，如果您以前使用过安全密钥，请在两步验证页面的安全密钥部分查找“添加安全密钥”链接；如果您没有使用过，请在页面下方查找“设置备用第二步”部分。系统会提示您选择安全密钥(您的智能手机)，您只需完成一个简短的提示即可为您的帐户启用该功能。

### 使用智能手机登录

现在，您可以使用您的 Android 设备来验证您的 Google 登录。这是如何工作的:

1.  确保在您的 Android 手机上启用了蓝牙和 [位置](https://support.google.com/accounts/answer/3467281?hl=en) 。
2.  当您登录 Gmail、YouTube、Chrome 或 Drive 等谷歌服务时，浏览器会提示您解锁手机，并按照指示确认登录。
3.  轻按手机上的**“Yes”**，然后等待认证过程完成。(如果您使用的是 Pixel 3 或 Pixel 3 XL，您也可以按下调低音量按钮来验证请求。)