# 这里有一种方法可以检查你的 Chrome 扩展是否安全

> 原文：<https://lifehacker.com/heres-one-way-to-check-that-your-chrome-extensions-are-1836630986>

鉴于最近的 DataSpii 浏览器扩展泄漏，数百万用户的数据被跟踪，并通过看似良性的浏览器扩展出售给 ，值得检查一下你可能已经安装或正在考虑安装的其他 Chrome 插件，以 [嗅出任何不良行为者](https://www.ghacks.net/2019/07/22/how-to-search-all-chrome-extensions-for-the-dangerous-unsafe-eval/) 。

Watch

为此，我们将使用一款名为[Chrome Extension Source Viewer](https://chrome.google.com/webstore/detail/chrome-extension-source-v/jifpbeccnghkjeaalbbjmodiffmgedin?hl=en)的轻量级软件，该软件可以发现潜在的可疑行为，如执行远程代码的能力。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1139306139072507906&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1139306139072507906&autosize=1) 

在我们开始这些步骤之前，我们应该指出，这个工具可能无法捕获每一个危险的浏览器扩展。DataSpii 插件通过欺骗谷歌并隐藏其恶意活动，逃脱了广泛的数据跟踪，其他人也可能这样做。此外，该工具可能会识别出完全正常的扩展。这只是您的安全工具包中的一个项目；仍然需要一些尽职调查来区分好的扩展和坏的扩展，但至少您会对要查找的内容有一个更好的想法。

### Chrome 扩展源代码查看器入门

1.  安装 [Chrome 扩展源码查看器](https://chrome.google.com/webstore/detail/chrome-extension-source-v/jifpbeccnghkjeaalbbjmodiffmgedin?hl=en) 插件
2.  打开 Chrome 网络商店页面，查看您想要查看的每个扩展。
3.  在 Chrome Web Store 页面上寻找扩展时，点击地址栏旁边的 Chrome 扩展源代码查看器“CRX”图标。
4.  点击“查看源代码”。
5.  等待新页面完全加载，然后找到并打开“manifest.json”文件。
6.  按 F3 或“CTRL+F”打开页面搜索，查找“unsafe-eval”

这是什么意思？“unsafe-eval”内容安全策略表示特定的扩展可以执行远程代码。这可能是一个安全风险，取决于扩展实际上在做什么——注意，这是一个足够大的风险，Mozilla [不允许 Firefox 扩展](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/content_security_policy#exampleNote_1) 在其目录中这样设置:

> *...由于重大安全问题，在 addons.mozilla.org 上列出的扩展不允许在其 CSP 中包含“unsafe-eval”、“unsafe-inline”、远程脚本、blob 或远程源的扩展*

同样，“unsafe-eval”并不一定意味着扩展是恶意操作的。但是，这确实表明您可能希望对该扩展进行更多的审查。搜索网页，看看是否有任何关于它的有问题的报告。如果你想减少你使用的浏览器扩展的数量——这是一个很好的安全措施——这可能有助于你识别出那些你并不经常使用并且可以安全删除的潜在扩展。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1151979025423904770&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1151979025423904770&autosize=1)