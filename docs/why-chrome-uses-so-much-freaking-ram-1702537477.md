# 为什么 Chrome 使用这么多该死的内存

> 原文：<https://lifehacker.com/why-chrome-uses-so-much-freaking-ram-1702537477>

谷歌 Chrome 是围绕 的最受欢迎的 [网络浏览器之一，但它占用了你电脑过多的内存。快速浏览一下你的任务管理器，就会发现数量惊人的占用内存的 Chrome 进程。这就是为什么 Chrome 使用这么多内存的原因——以及你可以采取哪些措施来抑制它的贪吃。](https://www.digitaltrends.com/computing/best-browser-chrome-vs-firefox-vs-safari-vs-edge/)

Watch

### **什么 Chrome 使用所有的内存用于**

想想看:当你使用电脑时，你所做的大多数事情都发生在你的浏览器中，从打开标签页，到观看 YouTube 视频，到使用与你的机器其余部分集成的网络应用程序或扩展。那是一大堆东西。

Chrome 将每个标签和扩展拆分成自己的进程，所以如果一个东西崩溃了，它不会立刻关闭整个网页或所有打开的标签。这对你来说方便多了，但这会导致更高的内存使用，因为 Chrome 不得不 [为每个标签](https://www.howtogeek.com/124218/why-does-chrome-have-so-many-open-processes/) 重复一些任务。

幕后还有其他事情在进行。 [比如 Chrome 的预渲染功能](https://www.chromium.org/developers/design-documents/prerender) 会导致更高的内存使用率，但它会让你的网页加载更快。某些扩展或网站也可能 [泄漏内存](https://developers.google.com/web/tools/chrome-devtools/memory-problems) 并随着时间的推移导致更高的 RAM 使用率。

当然，你安装、打开和运行的标签和扩展越多，Chrome 使用的内存就越多。

所以是的:Chrome 使用了大量的内存，但是它这么做有一个很好的理由:你的方便。我们已经习惯了大量的标签和快速的页面加载，我们付出的代价是以千兆字节的内存来衡量的。

### **高 RAM 使用率(通常)是好的**

你的任务管理器的内存栏中的那个巨大的数字可能令人震惊，但是记住空闲 RAM 是无用的 RAM 也是很重要的。内存的存在是有原因的:如果你的电脑可以在短期记忆中储存大量的东西，那么它可以在以后很快回忆起这些东西。如果你的计算机最终不需要这些资源，它会把它们扔掉，为需要这些资源的其他程序腾出空间。如果 RAM 是空的，那么它就没有被使用，您也不会从中受益。

按照这种逻辑，让你的 RAM *几乎*满可能是一件好事。当你的内存总是满的并且降低你的系统速度时，这就变成了一件坏事。如果您正在做的事情需要比您的电脑所能提供的更多的内存，它会开始将一些短期内存交换到您的电脑硬盘上，这可能会慢得多。

简而言之:不要因为 Chrome 使用了大量内存就抓狂。这意味着它在做它的工作。如果它占用了太多的内存，以至于你试图在电脑上做的其他事情都感觉迟钝，那么你肯定有一个值得解决的问题。

### **如何遏制 Chrome 的饕餮胃口**

所以你知道为什么 Chrome 使用大量内存，你也知道有时候这没什么。但如果它导致速度变慢，你有两个解决方案:降低 Chrome 的内存使用量，或者为你的电脑增加内存。

后者在台式电脑上很容易做到(如果你有钱的话)，但如果你的笔记本电脑 [不能升级](https://www.howtogeek.com/346541/how-to-upgrade-or-replace-your-pcs-ram/) 的话，在你的笔记本电脑上完成可能会更困难。如果这就是你的情况，你将不得不求助于一个不同的计划:为了节省一些内存而牺牲一些便利。

#### **找出占用内存的原因，并关闭它**

首先，打开 Chrome 并按 Shift+Esc(或者，在 Mac 上，进入窗口>任务管理器)。这将打开 Chrome 自带的任务管理器 ，让你更准确地看到每个标签和扩展占用了多少内存。您可以单击“Memory”列的顶部，按 RAM 使用率从高到低进行排序。

一旦你这样做了，你应该知道从哪里开始。也许你需要关闭那些 Gmail 标签页，或者也许这个方便的扩展并不值得你去使用 RAM。如果是这样的话， [从你的工具栏或者通过 Chrome 的扩展页面卸载](https://support.google.com/chrome_webstore/answer/2664769?hl=en) 。

#### **使用内存释放扩展管理您的标签使用**

当然，我们中的一些人无法在少于 24 个标签的情况下生存(我们的支持团体在周二和周四聚会)。如果这听起来像你，有一些扩展可以帮助你。安装更多的扩展来限制内存的使用可能看起来是违反直觉的，但是它实际上可以产生很大的影响。

[伟大的吊杆](https://chrome.google.com/webstore/detail/the-great-suspender/klbibkeccnjlkjkiokjodocebajanakg) 是一个 [非常酷的扩展](http://lifehacker.com/the-great-suspender-suspends-memory-hungry-chrome-tabs-5982490) 在标签处于非活动状态一段时间后挂起标签。它们仍然会在你的标签栏中打开——只是当你点击它们时，加载时间会稍长一些，因为 Chrome 正在从头开始重新加载它们。如果你一直打开标签页，并打算以后再打开它们，这会很有帮助。

有些人还喜欢 [OneTab](https://chrome.google.com/webstore/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall) ，其中 [执行类似的功能](http://lifehacker.com/onetab-unloads-all-your-tabs-into-a-shareable-list-5990088) ，但没有自动化。当您有一组您知道以后不会用到的选项卡时，您可以单击 OneTab 按钮将它们全部关闭，并打开一个带有每个选项卡链接的选项卡。这样，当你以后想回到它们的时候，你可以随意重新打开它们。这也减少了标签混乱，这很好。

[会话伙伴](https://chrome.google.com/webstore/detail/session-buddy/edacconmaakjimmfgnblocblbcdcpbko) 是另一个扩展，允许你分类和保存标签，并在以后重新打开它们。

尝试上述所有解决方案，找出最适合您工作流程的解决方案。要知道，你可能不得不做出一些牺牲——无论这意味着关闭标签页、卸载扩展，还是购买一台内存更大的新笔记本电脑，都取决于你。

本故事最初发表于 2015 年 5 月 21 日，并于 2019 年 10 月 1 日更新，以提供更多最新信息和资源。2012 年 3 月 3 日更新了新的细节。