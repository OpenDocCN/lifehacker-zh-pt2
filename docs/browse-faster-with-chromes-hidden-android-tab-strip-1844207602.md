# 使用 Chrome 隐藏的 Android 标签条更快地浏览

> 原文：<https://lifehacker.com/browse-faster-with-chromes-hidden-android-tab-strip-1844207602>

我是一个标签迷，但让我的 Android 版 Chrome 保持整洁的是，在我打开的不同网站之间切换是一件令人讨厌的事情。你必须点击 上的，而不是一个看起来很可爱的标签，这是一个丑陋的盒子，然后像纸牌游戏中一叠交错的卡片一样转储出你所有打开的页面。



假设你不只是在地址栏上左右滑动来切换标签，有可能会有一个更好的用户界面来整理你打开的网站。在最新的 Android 版 Chrome 测试版中，谷歌正在测试一项新功能，让你可以通过应用程序用户界面的底部使用图标导航许多打开的网站。这是一个更好看的实现，你可以在 Chrome 测试版和 Chrome 稳定版中得到。(Chrome Stable 需要一点额外的解决方法，我们将在本文末尾讨论。)

要开始使用更简单的方法，请下载[**Chrome Beta**](https://play.google.com/store/apps/details?id=com.chrome.beta&hl=en_US)并通过地址栏导航到此 URL:`chrome://flags/#enable-conditional-tabstrip`

启用那个标志，重新启动 Chrome，你*应该*看到浏览器底部的新标签条。如果没有——我没有——继续像平常一样使用浏览器。 [Android Police](https://www.androidpolice.com/2020/06/29/google-is-working-on-a-bottom-tab-switcher-strip-for-chrome-on-android/) 报告称，如果确实弹出了，可能需要一段时间。

如果没有，您还可以使用稍微复杂一点的方法强制解决这个问题。返回到您的 Chrome 标志，搜索/启用以下内容:

*   **标签组**
*   **选项卡组 UI 改进**
*   **条件标签条**

打开一个新标签，然后打开第二个标签，点击浏览器右上角的“2”框。将一个选项卡拖到另一个选项卡的顶部，使其合并成一个选项卡组(而不是替换选项卡的顺序)，如下所示:

现在，当你在这个标签组中打开和关闭网站时，你会在浏览器底部看到前面提到的新导航。这暂时是一个粗糙的解决方法，但是它很有效！这是*也是*在 **Chrome 的稳定频道**上启用标签条的变通方法——你在 ndroid 上使用的常规应用，不需要测试版。确保打开**选项卡组**、**选项卡组 UI 改进**和**选项卡网格布局**标志，否则无法工作。