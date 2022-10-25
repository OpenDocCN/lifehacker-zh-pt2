# 如何修复谷歌丑陋、充满标识的搜索结果

> 原文：<https://lifehacker.com/how-to-fix-googles-ugly-logo-filled-search-results-1841062453>

前几天当我在谷歌上搜索的时候，我感觉有些不对劲。事实证明，谷歌对其搜索结果页面进行了一点重新设计，增加了 favicons，这是一个用于赞助结果的大“广告”图标，并调整了网站 URL 的位置。



冒着听起来像坏脾气的提线木偶霍道夫和斯塔特勒的风险，我不喜欢它。如果你和我一样对这些杂乱的结果感到不快，那就有可能消除谷歌所做的一些改变，让你的搜索恢复平静和秩序。

首先，您需要在浏览器中安装广告拦截器，以阻止网站中的内容。这个我用的是威武的 [UBlock 原点](https://github.com/gorhill/uBlock) ，不过 [AdBlock 加](https://adblockplus.org/) 也可以。导航到你的扩展设置——无论在哪里，你都可以放入定制的过滤器——并输入 [这些过滤器](https://support.google.com/websearch/thread/16131099?hl=en&msgid=25784939) 来清理谷歌搜索结果页面的各个部分:

*   **移除 favicon:**Google . com # # . xa 33 GC
*   **删除网址:**Google . com # # . iuh 30 . BC . rpchfe
*   **去掉网址旁边的箭头:** google.com###am-b0 *和*Google . com # # . GHD vef . ab _ button
*   **删除一切:** google.com##。TbwUpd *和* google.com###am-b0 *和*Google . com # # . GHD vef . ab _ button

这是后两个更容易粘贴的版本。

#### **删除 URL 旁边的箭头:**

*Google . com # # # am-B0*
T3】Google . com # # . ghdvef . ab _ button

#### **清除一切**

*google.com##。TbwUpd*
*Google . com # # # am-B0*
*Google . com # # . GHD vef . ab _ button*

有了这些小小的过滤器，我就可以改变我的搜索结果页面了:

来个更赏心悦目的:

而且因为我很野，让我们也把那些烦人的视频去掉吧。在你的广告拦截器中输入这个过滤器来处理这些:
*Google . com # # g-section-with-header:has-text(/Videos/)*

当你这样做的时候，你的页面会变成这样:

我非常高兴。现在，这是一个看起来更优雅的搜索结果页面。