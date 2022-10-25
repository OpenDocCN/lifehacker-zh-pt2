# 如何使用指纹登录网站？

> 原文：<https://lifehacker.com/how-can-i-use-a-fingerprint-to-log-into-websites-1832025199>

当我们在 Lifehacker 结束唤醒周的时候，我希望你和我一样，期待着慷慨的 [**Tech 911**](https://lifehacker.com/c/tech-911) 本周每周五上午，我们将讨论一个我已经好奇了一段时间的问题——并不是说我对你的问题不好奇，但这个话题在我的脑海中萦绕了一会儿，因为我很懒，我



Lifehacker 读者**凯南**写道:

> *“首先，感谢大家对 lifehacker 有帮助的文章。继续努力吧！我有一个问题，到目前为止我还没有找到任何解决方案。*
> 
> 我买了一个内置指纹按钮的微软键盘 *，是给我的 windows 电脑用的。如果我能用这个按钮登录谷歌浏览器的网站，这将是一个非常酷的功能。但我在 Chrome 网上商店找不到任何东西。我现在只是用它来登录我的电脑。如果谷歌 chrome 中有一个插件或软件可以做到这一点，那就太好了。”*

第一，即使我在摇一个我喜欢的发光机械键盘，我还是很羡慕你键盘的指纹键。我只是在我的 MacBook 上玩了玩生物认证，与输入账户名称和密码(或其他任何东西)相比，轻触你的手指来批准或认证网站或应用程序非常方便，即使这是大多数智能手机用户自 2013 年以来就知道的“时尚”。

理论上，你对这个过程的看法是完全正确的。你应该能够使用键盘的内置指纹扫描仪登录网站和窗口。去年早些时候，Mozilla 开始在 Firefox 60 中推出这种支持，随后不久又推出了 [微软](https://blogs.windows.com/msedgedev/2018/07/30/introducing-web-authentication-microsoft-edge/) 和 [谷歌](https://blog.chromium.org/2018/09/chrome-70-beta-shape-detection-web.html) 。

这个无密码梦想的问题是，网站首先必须支持[fido 2 协议](https://medium.com/@herrjemand/introduction-to-webauthn-api-5fd1fb46c285) 才能进行指纹认证。即便如此，我也想不出有多少主要网站会让你只使用指纹通过浏览器进行身份验证。(诚然，*网站*不会验证你的指纹；该设备是，然后发送消息说 [你就是你所说的](https://www.maketecheasier.com/what-is-webauthn/) 。)

我的观点是，为了使用无密码认证，你必须首先在一个网站或服务上注册你的设备，我可以想到许多支持指纹识别器(或 Windows Hello)的网站。你可以使用(通过 Edge)进入你的微软账户，但我没有看到谷歌账户有类似的选项。 [一把安全钥匙](https://lifehacker.com/secure-your-accounts-and-passwords-with-a-hardware-toke-1830063430) ，确定，但不是指纹识别器。这只是一个例子，但同样的事情也可以发生在推特、脸书、我的网上银行、我的信用卡公司等等。

我没有列出支持或不支持指纹认证的网站和服务，而是提出了一个替代方案。如果你还没有使用密码管理器，可以考虑使用类似于 [1Password](https://support.1password.com/windows-hello/) 或 [LastPass](https://support.logmeininc.com/lastpass/help/fingerprint-authentication-lp030021) 的密码管理器。您可以将这两种服务都设置为使用指纹认证，这样可以更快地将您的登录凭据粘贴到站点中。

但是，不要去更改密码管理器的原始密码，因为您仍然需要不时地使用它来登录您的帐户(例如，在重新启动您的 PC 后)。一旦你做到了这一点，当你需要在网络表单中输入密码时，你就可以使用你的指纹来重新认证。

虽然这不是你可能想到的*真正的*“仅使用我的指纹登录”类型的设置，但在我们等待每个人永远取消密码时，这是一个很好的替代选择——或者，至少，提供生物识别登录的补充选项。

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>

<small></small>