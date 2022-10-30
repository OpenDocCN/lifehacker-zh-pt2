# 立即从您的 Mac 上移除缩放

> 原文：<https://lifehacker.com/remove-zoom-from-your-mac-right-now-1836209383>

对于 Mac 用户来说，Zoom 视频会议应用程序包含两大安全问题。首先，以常规方式卸载应用程序实际上不会将其从系统中移除；相反，通过安装 Zoom，你实际上已经在你的系统上安装了一个持久的 web 服务器，可以用来在未经你允许的情况下*重新安装*应用程序。



为什么这是个问题？因为攻击者可以向你发送一个会议邀请链接——嵌入在网站中，或者 [甚至电子邮件](https://vimeo.com/347012057)——这将启动 Zoom(即使你“删除”了它)。这会将你加入到一个电话会议中，默认情况下，，你的网络摄像头在上*，这可能会根据你在做什么而造成一些尴尬的时刻。*

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1148466535104692224&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1148466535104692224&autosize=1) 

这个问题有两个主要的修复方法，安全研究员 Jonathan Leitschuh 在他最近关于 Zoom 漏洞的公开披露中概述了这两个方法。至少，你需要进入 Zoom 的视频设置并启用这个设置:“加入会议时关闭我的视频。”

如果你想变得有趣，你也可以通过 Mac 终端来启用这个设置。运行两个命令之一:

#### 仅为您的本地帐户默认关闭您的网络摄像头

`defaults write ~/Library/Preferences/us.zoom.config.plist ZDisableVideo 1`

#### **默认情况下，为 Mac 上的**所有用户关闭网络摄像头

`sudo defaults write /Library/Preferences/us.zoom.config.plist ZDisableVideo 1`

如果你问我，更大的解决方案是完全卸载 Zoom 这意味着移除它在你的系统上丢弃的持久网络服务器。为此，您需要打开 Mac 终端并运行两个命令:

首先，运行这个来获取 web 服务器的进程 ID，或者 PID: `lsof -i :19421`

接下来，运行这个命令并输入 PID，括号中的文本是:`kill -9 [process number]`

然后你会想在你的 Mac 上找到`~/.zoomus`目录 [并将其完全删除。](https://support.zoom.us/hc/en-us/articles/201362983-How-to-uninstall-Zoom-on-a-Mac-)

最后，为了确保该服务器不会因为任何原因被重新安装到您的系统上，请在终端中运行以下两个命令:

`rm -rf ~/.zoomus`

`touch ~/.zoomus`

当然，删除 Zoom 应用程序就像删除任何你想卸载的应用程序一样。

### 未来:将基于浏览器的应用用于网络会议

大多数主要的网络会议服务——Zoom、Lifesize、WebEx 等等——都允许你通过浏览器参加会议。虽然欢迎你在你的电脑上安装应用程序，但没有理由忽视更干净的基于浏览器的方法。你不会在你的系统上安装一个你可能不需要的应用程序(或者，在 Zoom 的情况下，一个带有一堆安全问题的应用程序。)在 [大多数情况下](https://twitter.com/BradRubenstein/status/1148474691851444226) ，你仍然可以在会议中做任何你原本可以做的事情

 [https://lifehacker.com/embed/inset/iframe?id=twitter-1148470839186247686&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-1148470839186247686&autosize=1) 

如果你绝对*必须*拥有非基于浏览器的体验，考虑在你的 iPhone 或 Android 设备上安装 web meeting service 的应用。虽然这意味着当你拨号上网时，你必须找到一个地方来支撑你的手机或平板电脑，但至少你不会在你的主要电脑上安装一些有问题的软件。

***更新 2019 年 7 月 9 日下午 2:30 PT:**Zoom is*[*今天晚些时候发布更新*](https://blog.zoom.us/wordpress/2019/07/08/response-to-video-on-concern/) *该更新从其软件的 Mac 版本中删除了烦人的 web 服务器。如果你想在你的系统上保持缩放，请确保你更新到应用程序的最新版本。这很容易做到，因为你会得到一个提示缩放本身下一次你加载它。正如 Zoom 所描述的:*

> *" 7 月 9 日补丁:计划在今晚(7 月 9 日)太平洋时间上午 12:00 或之前发布的补丁将执行以下操作:1 .更新 Zoom 客户端后，完全移除本地 web 服务器–我们将停止在 Mac 设备上使用本地 web 服务器。一旦补丁被部署，Mac 用户将在缩放用户界面(UI)中被提示更新他们的客户端。更新完成后，该设备上的本地 web 服务器将被完全删除。2.允许用户手动卸载 Zoom–我们在 Zoom 菜单栏中添加了一个新选项，允许用户手动完全卸载 Zoom 客户端，包括本地 web 服务器。一旦补丁部署完毕，一个新的菜单选项将会出现，上面写着“卸载 Zoom。单击该按钮，缩放功能将与用户保存的设置一起从用户设备中完全删除*