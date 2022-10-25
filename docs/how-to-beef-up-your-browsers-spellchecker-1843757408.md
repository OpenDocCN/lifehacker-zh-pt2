# 如何增强浏览器的拼写检查功能

> 原文：<https://lifehacker.com/how-to-beef-up-your-browsers-spellchecker-1843757408>

由于谷歌和微软最近的合作，基于 Chromium 的 Windows 网络浏览器获得了一个全新的拼写检查器。Windows 拼写检查，而不是 [Hunspell](http://hunspell.github.io/) ，现在将帮助你修复你的各种错别字和 [明显的拼写错误](https://www.merriam-webster.com/word-games/spell-it) (特别是 URL 和首字母缩写)，但你可能需要先启用该功能才能利用它。

Watch

正如微软 [写的](https://blogs.windows.com/msedgedev/2020/05/28/improved-spellcheck-microsoft-edge-83/) ，这个新的拼写检查器应该会自动在最新版本的**微软 Edge** 中工作——那将是前几天刚刚放弃的版本 83。如果你不想不断质疑你自己的“我在 e 之前”的规则，请打开 Windows Update 并查看是否有可用的东西，以确保你已经更新了你的浏览器。(是的，和大多数浏览器不同，原来的 Edge 是通过 Windows 本身更新的。)

从那里，输入`edge://settings/languages`到你的地址栏，并确保你已经为你在中写的任何语言启用了拼写检查。就这么简单。

如果你使用的是 [**边缘铬**](https://www.microsoft.com/en-us/edge?form=MA13DE&OCID=MA13DE) 或 [**铬**](https://www.google.com/chrome/) ，你需要启用一个浏览器标志，这样你就可以确定你使用的是新的 Windows 拼写检查。你会在`chrome://flags/#win-use-native-spellchecker`找到它

如果你一直在使用 Chrome 的增强拼写检查功能，该功能会将你的文本发送到谷歌以验证其准确性，设置该标志会将你的浏览器下拉至“基本拼写检查”，如下所示:

我认为这是质量和隐私之间的一个很好的权衡，因为我一直有点儿*嗯*把我输入的所有东西都发送到谷歌——尽管谷歌让这个过程 [听起来相当良性](https://www.google.com/chrome/privacy/whitepaper.html#spelling) 。

不过，这并不是你唯一可以乱动的 Chrome 标志。如果你启用了 Windows 拼写检查器和这个标志——`chrome://flags/#win-use-hybrid-spellchecker`——你可以让 Windows 拼写检查器*和*两者都准备好。Windows 拼写检查器将是你的默认拼写助手，但如果你使用的语言它不支持(你可以通过**设置>时间&语言>语言**在 Windows 中设置)，那么 Hunspell 将接管并尽最大努力识别你的错误。

(使用 **Edge Chromium** 的人可以使用上述标志启用 Windows 拼写检查，但你不能选择使用混合方式。)