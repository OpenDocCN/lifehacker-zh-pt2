# 今天如何试用 Chrome 86 的大电池节省修复

> 原文：<https://lifehacker.com/how-to-try-out-chrome-86s-big-battery-saving-fix-today-1844283047>

谷歌 Chrome 令人难以置信的拖慢系统的能力可能很快就会成为过去。最新的 Chrome Canary 版本包括 Chrome 处理后台网站的方式的重大变化，这可能会减少 Chrome 对设备电池寿命的压力。这些变化应该有望成为 Windows、Mac、Android、Linux 和 Chrome OS 的 Chrome 86 更新的一部分，成为稳定版本。



一组网络开发人员研究了 Chrome 过多的 [Javascript 定时器唤醒](https://news.thewindowsclub.com/google-chrome-ships-a-new-feature-to-increase-the-battery-life-101417/) ，发现让这些定时器随心所欲地启动并不能让浏览器更好用。虽然这些 Javascript 计时器中有一些会跟踪重要的过程——比如你是否在社交媒体页面上收到了新消息或通知——但还有一些会检查不必要的信息，比如广告互动，或者你是否进一步向下滚动了一页。许多多余的计时器会占用额外的内存，结果会消耗更多的电池寿命。

谷歌正在引入限制，将这些计时器限制为每分钟更新一次，这应该可以在不影响网站性能的情况下缓解一些系统和电池压力 。多少钱？谷歌在测试中将笔记本电脑的电池延长了*两个小时*(36 个随机打开的标签；Javascript 定时器唤醒限于每分钟一次)。

### 如何在 Chrome Canary 中启用 Chrome 的省电设置

像其他测试版和早期软件一样，Chrome Canary 还没有完成，可能不稳定。你总有可能会遇到错误或兼容性错误，但这是尝试 Chrome 潜在节能变化的唯一方法(就目前而言)。如果有任何问题，只要换回普通的旧铬。

此外，启用实验标志的步骤仅适用于 Chrome Canary。一旦 Chrome 86 公开发布，它很可能会成为浏览器新的默认行为。所以您可能不需要启用任何东西。

1.  [下载安装 Chrome 金丝雀](https://www.google.com/chrome/canary/)T3。它作为一个单独的应用程序安装，不会覆盖稳定的 Chrome 应用程序。
2.  在 Chrome Canary 中打开一个标签，进入 **chrome://flags**
3.  搜索**“在后台节流 Javascript 计时器。”**

4.  使用下拉菜单将标志设置为**“隐藏标签时立即启用”**
5.  点击**“重新启动”**关闭并重新加载 Chrome Canary。该设置将在重新启动后应用。