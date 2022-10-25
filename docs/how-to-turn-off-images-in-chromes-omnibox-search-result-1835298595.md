# 如何关闭 Chrome 地址栏搜索结果中的图片

> 原文:[https://life hacker . com/how-to-off-images-in-chromes-omni box-search-result-1835298595](https://lifehacker.com/how-to-turn-off-images-in-chromes-omnibox-search-result-1835298595)

最新最棒的谷歌 Chrome 版本对 [做出了大多数人不会注意到的](https://developers.google.com/web/updates/2019/06/nic75) 改变，比如对浏览器加载页面和图像的方式进行了调整。然而，大多数人*会*注意到的一个特点是，当你在 Chrome 的地址栏或“Omnibox”中搜索时，会弹出一些图像

Watch

这些新图像可以成为搜索的视觉辅助工具，尽管它们只出现在某些类型的搜索中，如名人姓名，并且受到某些版权和隐私限制。但是如果你觉得这些新图片与其说有用，不如说烦人，有几种方法可以在 Chrome 的桌面版中关闭它们。

最简单的方法是将 [换成一个完全不同的搜索引擎](https://gizmodo.com/5-reasons-not-to-use-google-for-search-1785396969) ，因为 Omnibox 中只有谷歌结果显示图片。您可以在浏览器设置中实现这一点:

1.  点击三个堆叠的点图标，然后点击“设置”
2.  在设置页面，向下滚动到“搜索引擎”，然后点击下拉框，选择不是谷歌的东西。
3.  如果您没有看到列出的您想要使用的搜索引擎，“管理搜索引擎”选项允许您添加或删除搜索引擎— [，如 DuckDuckGo](https://lifehacker.com/how-to-maximize-your-browsing-privacy-using-duckduckgo-1830659232) 。

然而，如果你想让谷歌成为你的默认搜索引擎，你需要调整一个 Chrome 标志来去掉这些图片。

在这种情况下，我们要寻找“Omnibox 富实体建议”标志(向 Ghacks 喊出 [，最初指出](https://www.ghacks.net/2019/06/05/google-releases-chrome-75-stable-for-desktop-and-mobile/) )。到达那里:

1.  将**chrome://flags/# omni box-rich-entity-suggestions**复制并粘贴到 Chrome 的地址栏中，然后点击回车。这将把你直接带到 Chrome 的 flags 页面，高亮显示“Omnibox 富实体建议”。
2.  点击标志旁边的下拉框，将其设置为**“禁用”**
3.  关闭并重启 Chrome 以使更改生效。

谷歌经常从 Chrome 中添加和删除功能和标志，所以 Omnibox 图像可能会像谷歌 尝试的许多其他想法一样来来去去。也有可能谷歌会移除前面提到的标志，这将迫使每个人都看到这些 Omnibox 搜索图像。(换句话说，如果这招不管用了，就怪谷歌吧。)