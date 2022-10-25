# 你现在应该在浏览器中启用的五个自定义搜索

> 原文：<https://lifehacker.com/five-custom-searches-you-should-enable-in-your-browser-5971715>

定制搜索引擎是任何现代浏览器中最酷的功能之一。只需敲击几下键盘，你就可以直接从地址栏搜索维基百科，在谷歌上搜索 Lifehacker 的文章，甚至还能找到某个特定地点的行车路线。

Watch

这些自定义搜索非常容易设置。在 **Chrome** 中，只需右击地址栏，选择“编辑搜索引擎”。您可以编辑现有的或添加您自己的，给它们一个名称、URL 和一个您将键入的关键字来启动搜索。

在 **Firefox** 中，你可以通过创建一个 [智能关键词](https://support.mozilla.org/en-US/kb/how-search-from-address-bar) 来完成同样的过程——只需右击网站上的任何搜索框，选择“为此搜索添加关键词”，然后输入你知道你会记住的东西。然后，当你在浏览器的地址栏中输入关键词和搜索词时，你就可以直接在那个网站上搜索了。

你也可以通过扩展 添加搜索工具 [，当你开始在 Firefox 的地址栏中输入内容时，这些工具就会以小图标的形式出现在窗口底部的“这次，搜索”栏中。](https://addons.mozilla.org/en-US/firefox/search/?sort=rating&type=search)

如果你需要一点帮助来思考如何将新的搜索引擎整合到你的浏览器中，我们可以提供帮助。这里有五条，几乎每个人都可以(也应该)用来让自己的生活变得更轻松。

* * *

### **在谷歌上搜索过去一年的网页**

你有没有在谷歌上搜索过，却发现一堆不再相关的旧页面？如果你想将你的搜索限制在一个特定的时间——比如说，过去一年的内容——尝试这个链接(使用“%s”作为你想要查找的任何内容的通配符):

[`https://www.google.com/search?hl=en&tbo=1&tbs=qdr:y&q=%s`](https://www.google.com/search?hl=en&tbo=1&tbs=qdr:y&q=%s)T4】

你可以在任何你想要的时间范围内这样做，比如一个月，两个月，或者两年，就像我们在之前提到的[。](http://lifehacker.com/use-keywords-to-search-specific-time-frames-from-your-a-5858650) 

* * *

### **在维基百科上搜索电视节目或音乐专辑**

用自定义搜索引擎搜索维基百科很容易，但维基百科也内置了很多很酷的东西。例如，维基百科上有几乎所有现存电视节目的剧集列表。因此，您可以创建一个自定义搜索，只搜索电视节目，类似于这样(%s 是您输入的通配符):

[`<small>http://en.wikipedia.org/wiki/Special:Search?search=list+of+%s+episodes</small>`](http://en.wikipedia.org/wiki/Special:Search?search=list+of+%s+episodes)T4】

给这个搜索输入一个关键词，比如“ep”，然后在地址栏输入一个短语，比如`ep The Simpsons`，马上就能得到该剧所有剧集的列表。

如果您使用此 URL 进行自定义搜索，您也可以对音乐专辑进行同样的操作:

[`http://en.wikipedia.org/wiki/Special:Search?search=%s+discography`](http://en.wikipedia.org/wiki/Special:Search?search=%s+discography)T4】

你可以用同样的概念改编维基百科上的任何其他“系列”页面，这可能是各种有用的，取决于你通常在服务上查找什么。

* * *

### **通过谷歌地图获取某个地址的行车路线**

这个很简单。将此 URL 用于您的自定义搜索(使用“%s”作为您的通配符条目):

[`http://maps.google.com/maps?f=q&source=s_q&hl=en&q=from+my+home+address+to+%s`](http://maps.google.com/maps?f=q&source=s_q&hl=en&q=from+my+home+address+to+%s)T4】

用你真实的家庭(或工作，或其他)地址代替`my+home+address`。给搜索一个像`maps home`这样的关键词，然后在地址栏中输入`maps 123 main street`，就可以立即找到从你住的地方到主街 123 号的方向。

实际上，我们之前已经分享过这个，以及其他一些地址栏“技巧”(虽然不完全是搜索，但仍然非常有用)。查看我们的 [指南，用你的地址栏](http://lifehacker.com/how-to-perform-nearly-any-task-from-your-browsers-addre-5731656) 做任何事情，以获得更多乐趣，自定义搜索引擎的类似用法。

* * *

### **搜索您当前正在浏览的任何网站(如 Lifehacker)**

如果您发现了一个博客，并想在它的档案中搜索特定的内容，该怎么办？你可以使用一个定制的搜索引擎，只搜索你当前的域名:

```
javascript:location='[http://www.google.com/search?num=100&q=site:'%20+%20escape(location.hostname)](http://www.google.com/search?num=100&q=site:%27%20+%20escape(location.hostname))%20+%20'%20%S'%20;%20void%200
```

给它一个关键字，比如`cd`，然后像其他搜索一样运行它。去一个网站，然后在地址栏中输入`cd windows 8`，你会从那个网站得到关于 Windows 8 的结果*。这是终极通配符方法。*

* * *

### **搜索你能想到的任何网站(除了那些显而易见的网站)**

以上大多数搜索使用了你自己可能都没有想到的巧妙的 URL 技巧。同样值得一提的是，你仍然可以使用定制搜索引擎来搜索任何你想要的网站:IMDB、YouTube、维基百科、Lifehacker 或任何你能想到的网站。例如:

#### **在字典或词典中查找单词**

Dictionary.com 和 Thesaurus.com 是非常有用的工具(如果你懒得在 Google.com 输入 define:yourword 的话)。要在字典中查找单词，只需使用:

[`http://dictionary.com/browse/%s`](http://dictionary.com/browse/%s)T4】

要在词典中查找，请使用:

[`http://thesaurus.com/browse/%s`](http://thesaurus.com/browse/%s)T4】

#### **在谷歌上翻译单词**

如果你正在学习一门新语言，谷歌翻译是一个很好的工具，你可以设置一个定制的搜索引擎，使搜索变得更容易。使用 URL 创建搜索:

[`http://translate.google.com/#auto|en|%s`](http://translate.google.com/#auto|en|%s)T4】

这可以将另一种语言的单词翻译成英语，不过你可以调整`auto|en`部分来适应你想要的语言。

#### **在谷歌上自动“感到幸运”**

如果你知道你的搜索词会显示某个页面，或者你只是想冒险，谷歌的“我感觉很幸运”作为关键词是有用的。只需使用此 URL:

[`http://www.google.com/search?q=%s&btnI=Im+Feeling+Lucky`](http://www.google.com/search?q=%s&btnI=Im+Feeling+Lucky)T4】

#### **了解一个网站是否已经关闭**

我们最喜欢的网站之一，Down For Everyone Or Just Me，只有一个目的:告诉你一个网站是否已经关闭，或者你的设置是否有问题。为了测试一个特定的网站，尝试这个定制的搜索引擎:

[`http://www.downforeveryoneorjustme.com/%s`](http://www.downforeveryoneorjustme.com/%s)T4】

* * *

### 我们错过了什么吗？

如果你有任何你绝对喜欢的定制搜索引擎，请在评论中告诉我们！我们很乐意在未来的更新中突出您提交的内容。