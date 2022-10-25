# 如何设置最好的假电话号码

> 原文:[https://life hacker . com/how-to-set-a-fake-phone-number-1829907777](https://lifehacker.com/how-to-set-up-a-fake-phone-number-1829907777)

当你需要摆脱某人的时候，虚假的电话号码是一件美好的事情。无论你是当场编造号码，还是把号码给像拒绝热线 这样的服务机构 [，给一个假号码可以缩短尴尬的社交接触。不过，最棒的是你自己制作的，就像我给汽车经销商的那种，伪造完整的语音邮件。](https://lifehacker.com/give-out-these-fake-prank-numbers-to-creeps-1826672360)

Watch

当我在市场上购买一辆新车时，我在 [上阅读了](https://jalopnik.com/how-to-shop-for-a-car-without-dealers-stalking-you-fore-1796753270) [这部 Jalopnik 作品](https://jalopnik.com/how-to-shop-for-a-car-without-dealers-stalking-you-fore-1796753270) ，躲避饥渴的经销商 的电话。它建议，申请一个谷歌语音号码。嗯，我已经把谷歌语音用在其他用途上了，而且这项服务并没有给你无限的号码。 [燃烧器应用](https://lifehacker.com/burner-generates-disposable-phone-numbers-for-perfectly-5933208) 是另一种选择，但在这一点上，你不妨从 [Twilio](https://www.twilio.com/) 中抓取一个数字，并从中获得一些乐趣。

我主要用我的号码访问 TrueCar 价格报告。这项服务需要一个电话号码和电子邮件，然后只要你要求一个价格，该地区的每一个汽车经销商都会从暗处爬出来与你联系。我不想不停地屏蔽来电，也不想把它们发送到一个友敌的号码。我只想让它们的叫声消失在空气中，永远也不会传到我的耳朵里，永远也不会反弹回来，而是像扔进雾中的石头一样消失。幸运的是，有一种方法。

### **如何设置您的假号码**

首先注册一个 [Twilio](http://twilio.com/) 账号，是免费的。你也可以免费保留你的第一个电话号码，尽管任何人打电话或发短信都会听到消息说这是一个 [免费试用的 Twilio 账户](https://support.twilio.com/hc/en-us/articles/223136107-How-does-Twilio-s-Free-Trial-work-) 。如果你想的话，你可以停在那里。假号码成功了。

但有趣的部分来了。当你在 Twilio 仪表板上点击你的电话号码设置时，你可以告诉服务当有人打电话或发短信给你的号码时它应该做什么。默认情况下，它会读一点信息(说你还没有设置号码，或者别的什么)。所以我复制了那条信息，并修改了它，让它听起来像一个完整的语音信箱。这是我的剧本:

`<Response><Say voice="alice">You have reached. 5 5 5\. 5 5 5\. 1 2 1 2\. Please leave a message after the tone.</Say><Pause length="1"/><Say voice="alice"> This mailbox is full. </Say></Response>`

免费试用的消息骗不了任何人，所以我为这个号码每月支付 1 美元，外加每分钟 0.0015 美元。我的假号码总共接了 38 个电话，这意味着我躲过了那么多汽车销售人员，总共赚了不到两美元。

### **玩得更开心**

当然，你可以写一个脚本，说任何你想说的话。你可以设立自己的拒绝热线，或者让它朗读一首欢快的诗歌。如果你想的话，你可以让他们*实际上*留言。你甚至可以 [写一个脚本](https://www.twilio.com/docs/voice/twiml) 让漂亮的机器人女士和你的来电者对话。

这也适用于文本。你可以用聊天机器人联系那些给你发 Twilio 号码短信的人，也许是用简单易用的 Dexter 平台 编写的聊天机器人。你可以用你的新假号码享受各种乐趣，从异想天开到邪恶。明智地选择。

*这个故事最初发表于 2018 年，并于 2020 年 2 月 24 日更新了新信息。*