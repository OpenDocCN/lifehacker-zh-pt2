# 如何在桌面上创建一个浮动的网飞播放器

> 原文:[https://life hacker . com/how-to-create-a-floating-a-网飞-player-on-your-desktop-1835784655](https://lifehacker.com/how-to-create-a-floating-netflix-player-on-your-desktop-1835784655)

据多份报道称，网飞正在测试一款新的弹出式播放器，供那些使用网飞网站来播放他们最喜欢的节目的人使用。虽然我倾向于只使用网飞的应用程序，但这种新方法有一些优雅之处——如果你可以使用该功能，点击网飞播放器上的一个小按钮，就会在一个独立的浮动窗口中启动它。这个窗口位于你正在电脑上做的任何事情之上，这意味着当你在工作中有八个小时快乐的电子表格等着你时，这是分散你注意力的最佳方式。

Watch

问题？这是网飞发给 [Engadget](https://www.engadget.com/2019/06/21/netflix-testing-pop-out-player/) 网站询问时的特写:

你不需要等待网飞让你尝试这个功能——如果它曾经尝试过的话。通过一两个小小的调整，你可以创建一个你自己的网飞弹出播放器。

### 铬

要将任何 HTML5 视频播放器变成弹出式播放器，只需创建一个 bookmarklet。为任何站点创建一个书签，然后 r 右键单击它并编辑书签的地址，用下面的代码替换它(一行代码):

`javascript:document.getElementsByTagName(‘video’)[0].requestPictureInPicture();`

然后，无论何时你在 YouTube 或网飞这样的网站上，你都可以点击那个书签，将视频弹出到它自己的播放器中。与网飞的实现类似，画中画视频将位于您正在处理的任何内容之上。你必须让 Chrome 保持打开，但你不必在 Chrome 窗口中才能看到画中画播放器。

如果你不能正常工作，确保你已经将 Chrome 浏览器的 [更新到最新版本的](https://support.google.com/chrome/answer/95414?co=GENIE.Platform%3DDesktop&hl=en) 。

### 火狐浏览器

火狐 68(7 月 9 日发布)应该会提供画中画功能。在那之前，你必须使用一个扩展来复制这种画中画功能。安装 [**浮动播放器**](https://addons.mozilla.org/en-US/firefox/addon/floating-player/?src=search) ，然后在观看网飞视频时点击浏览器工具栏中的图标。浮动标签打开后，您必须关闭原始标签中的视频，但是...一些事情。

您还会注意到，这个弹出式播放器不会位于其他窗口的顶部。要解决这个问题，请使用 Windows 的 [**桌面锁定**](https://efotinis.neocities.org/deskpins/) 应用程序，它允许你将任何你想要的窗口锁定在其他窗口之上。([**Pennywise**](https://lifehacker.com/pin-videos-on-your-screen-while-you-work-with-this-app-1830262895)**或 [**氦**](http://heliumfloats.com/) 也行，如果你不喜欢大惊小怪一个扩展+实用程序的组合。)**