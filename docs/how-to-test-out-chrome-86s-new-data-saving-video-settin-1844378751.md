# 如何测试 Chrome 86 新的数据保存视频设置

> 原文：<https://lifehacker.com/how-to-test-out-chrome-86s-new-data-saving-video-settin-1844378751>

如果即将到来的 Chrome 86 更新有一个主题，那似乎就是“效率”。我们已经看到了 [节省内存的变化，这应该使 Chrome 不那么耗电](https://lifehacker.com/preview/switch-to-chrome-canary-for-now-to-get-chrome-86s-batte-1844283047?rev=1594064460353) ，但用户也有一个新的节省数据的“LiteVideo”模式值得期待。

Watch

LiteVideo 模式通过“假装”设备的网络连接很慢来强制视频以标清(SD)播放，因此网站将切换到标清播放分辨率，而不是高清。这减少了流传输时使用的数据量，应该有助于视频加载更快，在连接不良的情况下播放更流畅。

与 Chrome 86 即将推出的许多功能一样，LiteVideo 模式目前处于测试阶段；你可以通过下载 Chrome Canary 并打开控制设置的两个实验标志来尝试一下。它可以在 Android、Windows、Mac 和 Chrome OS 版本的 Chrome 上使用。 [Chrome 金丝雀](https://www.google.com/chrome/canary/) 与普通的 Chrome app 是分离的，因此可以在不覆盖 Chrome 稳定版本的情况下安装使用。如果你在 Canary 上遇到错误或稳定性问题，你可以很容易地切换回 Chrome(或其他浏览器)。

### 如何提早试用 Chrome 的 LiteVideo 模式

1.  [在你的设备上下载、安装并启动 Chrome Canary。](https://www.google.com/chrome/canary/)T3】
2.  打开一个新标签，进入 **chrome://flags**
3.  使用搜索框找到**“Enable lite videos”**使用下拉框将标志设置为**“Enabled”**
4.  接下来，搜索**“强制 LiteVideos 决策”**，并将其设置为**“启用”**。
5.  重新启动 Chrome Canary 以使更改生效。

只有在测试功能时，才需要启用标志。很难说用户会如何打开最终形式的 LiteVideo，它可能会比现在容易得多——假设它会在 9 月或 10 月的某个时候发布公共 Chrome 86。实验特征经常被推后或完全删除。不过现在，在 Chrome Canary 中使用 LiteVideo 可以节省一些数据，减少视频加载时间。