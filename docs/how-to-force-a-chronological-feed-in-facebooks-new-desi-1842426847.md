# 如何在脸书的新设计中“强制”一个按时间顺序排列的提要

> 原文:[https://life hacker . com/how-to-force-a-chronological-feed-in-face books-new-desi-1842426847](https://lifehacker.com/how-to-force-a-chronological-feed-in-facebooks-new-desi-1842426847)

新脸书在这里，但一个新的按时间顺序排列的新闻源却没有——除非有一个聪明的小技巧。

Watch

如果你打开桌面浏览器，点击界面右上角的下拉箭头，选择“切换到新脸书”，你现在就可以测试脸书的重新设计，就像这样:

它的外观和感觉变成了这样——如果你选择黑暗模式，那就是:

在你最左边的工具条上，你可以点击你的新闻提要旁边的点，在脸书的精选提要和严格的、纯粹的按时间顺序的帖子提要之间切换。我绝对喜欢后者，并希望脸书能让我默认它——唉——该公司现在已经在新设计中埋葬了这一选项。

如果你点击左边的“查看更多”链接，向下滚动感觉像是永远，你会在最底部看到一个“最近”选项。(或者，至少，前几天我的就在那里；此后，这种选择有所上升。)

如前所述，脸书不允许你默认一个“最近”的订阅源，所以我们要想办法解决这个问题。最简单的方法是在你的浏览器中——最好是在工具栏中——创建一个脸书的书签，并确保它使用这个链接:`https://www.facebook.com/?sk=h_chr`

当你这样做的时候，点击你的书签总是会在“最近”模式下调出脸书。简单。但是如果你不想做书签，因为你更习惯在浏览器的地址栏中输入“facebook.com ”,我们也可以做到这一点。

如果你在 [**Chrome**](https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd?hl=en) 或[**Firefox**](https://addons.mozilla.org/en-US/firefox/addon/redirector/)上，只需抓取并安装重定向器扩展(从这些链接中的任何一个)。一旦你设置好了，点击它的图标并选择“编辑重定向”出现的屏幕如下所示:

您需要点击**“创建新的重定向”**下一个屏幕可能看起来有点混乱，但是很简单。我来分解一下:

*   **描述:**您可以随意命名您的重定向。
*   **例子网址:**只需输入好的 ol’`facebook.com/`。除此之外没什么可做的了。
*   **Include pattern:** 为了确保你所要做的就是在你浏览器的地址栏中输入 facebook.com，你需要在你的示例 URL—`facebook.com/`—前面加上一个通配符。如果你想变得疯狂，你可以把示例 URL 改为“fb”，不加引号，并使用*fb*模式，这意味着你只需在浏览器的地址栏中输入这两个字母，然后按回车键就可以访问脸书。你的选择！而且，是的,“包含模式”中的正斜杠对这个过程是至关重要的；我花了很长时间才意识到这一点，所以别忘了。
*   **重定向至:**输入你想让 facebook.com 去的网址。在这种情况下，那就是`https://www.facebook.com/?sk=h_chr`
*   **图案描述:**随便输入！

就是这样！您可能想知道为什么我不直接使用整个包含模式，或`*facebook.com*`。嗯，这样做意味着你在浏览器中输入的任何其他脸书网址——比如复制并粘贴到一个群组的链接——都会立即重定向到前面提到的“最近”新闻源网址。这很烦人。在这种情况下，我们对规则进行了限制，只有在浏览器中输入 facebook.com 的*才会将你发送到你想要的新网址；你仍然可以输入其他 facebook.com/whatever 网址没有问题。*

整个过程的一个警告是，这是一次性交易。在脸书的网站上导航*，点击左上角的大图标重新访问你的新闻订阅，会给你一个蹩脚的非时间顺序的订阅。不幸的是，这个扩展只能捕获你输入地址栏的内容，而不能捕获那些经常存在的内容。如果我为*那*找到更好的解决方案，我会让你知道。*