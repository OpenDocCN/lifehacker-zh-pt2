# 如何为 Windows 10 中的所有应用打开 HTTPS DNS

> 原文:[https://life hacker . com/how-to-turn-on-DNS-over-https-for-all-apps-in-windows-1-1843544589](https://lifehacker.com/how-to-turn-on-dns-over-https-for-all-apps-in-windows-1-1843544589)

使用 HTTPS DNS(DoH)可以隐藏您的电脑正在访问的网站，从而使您的 web 浏览更加安全。我们已经介绍过 [在浏览器](https://lifehacker.com/how-to-enable-dns-over-https-in-your-web-browser-1841909057) 中开启 DoH，但是最新的 Windows Insider 更新为 Windows 10 增加了系统级 DoH 设置。它非常方便。

Watch

打开 Windows 10 的系统级 DoH 将为安装在支持它的 PC 上的所有浏览器启用 HTTPS DNS，以及现在或将来可以使用它的任何其他基于互联网的程序。Brave、Chrome、Edge Chromium、Firefox 和 Opera 目前都支持 DoH，但迄今为止，你必须单独配置每个浏览器的 DoH 设置——如果你使用多个浏览器，这是一个繁琐的过程。使用 Windows 10 DoH 会应用您电脑的互联网适配器，以便访问它的每个浏览器或应用程序都将使用相同的 DNS 设置。

虽然 [Windows 10 的 DoH 功能](https://techcommunity.microsoft.com/t5/networking-blog/windows-insiders-can-now-test-dns-over-https/ba-p/1381282) 目前只对 Windows 内部人士开放，但它在最新更新中的出现意味着公开发布可能很快就会发生。但是，如果您想尽早访问微软的系统级 DoH，我们将向您展示如何获得它。

### 如何为 Windows 内部人员打开 Windows 10 的 HTTPS DNS

为了试用 Windows 10 系统级 DoH 的早期版本，你需要成为 Windows Insider——基本上是 Windows 10 beta 测试者——因为 Windows 10 DoH 在最近的 Insider 系统更新中可用。要注册，只需打开 Windows Update，然后单击左侧边栏上的 Windows Insider 计划部分。我们推荐内部版本的慢环；您可以通过坚持发布预览版来降低风险(以牺牲特性为代价)，或者通过追求快速环来降低风险(以牺牲系统稳定性为代价)。

一旦你是一个内部人员，并且你有了最新的 Windows 更新，以下是如何检查你正在使用的版本:

1.  按开始键打开 Windows 开始菜单。
2.  搜索`winver`并运行应用程序。
3.  将弹出一个窗口。查找版本号旁边的**“OS Build”**号。您需要运行 OS Build 19628 或更高版本才能打开 DoH。
4.  点击**【确定】**关闭窗口。

如果你的操作系统版本不匹配，确保你已经安装了 [最新的 Windows beta 更新](https://lifehacker.com/get-the-newest-version-of-windows-forever-with-windows-1775733312) ，然后再次检查。

一旦你确认你正在运行正确的内部版本，你现在可以打开 DoH 了。这比你的普通功能需要更多的文件操作，但微软表示这一过程只适用于 Windows Insider 版本。一旦公开推出系统级 DoH，设置将更加简单。

要开始使用:

1.  首先，打开 Windows 开始菜单，搜索并以管理员身份打开注册表编辑器。
2.  在注册表编辑器窗口中打开:**HKEY _ LOCAL _ MACHINE \ SYSTEM \ current control set \ Services \ DNS cache \ Parameters**
3.  在 **"Parameters"** 文件夹中点击右键，创建一个新的 Dword (32 位)值。将这个新文件命名为“EnableAutoDOH”，并将其值设置为“2”
4.  关闭注册表编辑器，并重新启动您的电脑。
5.  重新启动后，再次打开开始菜单并打开设置。
6.  前往**网络&互联网>更改适配器选项**
7.  右键单击您的电脑使用的互联网适配器，然后选择**“属性”**
8.  向下滚动并双击**互联网协议版本 4** 或**互联网协议版本 6** (如果适配器两者都有，您需要重复接下来的步骤)。
9.  选择**“使用以下 DNS 服务器地址”**，然后键入以下 DNS 服务之一的地址:

**Cloudflare**

*   1.1.1.1(IP v4)
*   1.0.0.1(IP v4)
*   2606:4700:4700::1111 (IPv6)
*   2606:4700:4700::1001 (IPv6)

谷歌

*   8.8.8.8(IP v4)
*   8.8.4.4(IP v4)
*   2001:4860:4860::8888 (IPv6)
*   2001:4860:4860::8844 (IPv6)

**Quad9**

*   9.9.9.9(IP v4)
*   149.112.112.112(IP v4)
*   2620:fe::fe (IPv6)
*   2620:fe::fe:9 (IPv6)

添加地址，然后点击**【确定】**关闭窗口并保存设置。

你现在可以通过访问 [Cloudflare 的帮助页面](https://1.1.1.1/help) 来测试你的 DoH 连接，它会告诉你你的浏览器是否在使用 DoH。如果一切看起来都很好，那么您的设置是可靠的，您现在可以使用几乎无处不在的 DoH 设置进行浏览。

如果你看到任何错误或者它说你*没有*通过 HTTPS 的 DNS，回到上面的步骤，并三次检查所有的名字都是正确的，所有的地址都是正确的。

要关闭 Windows 10 的 auto-DoH 设置，请删除您之前创建的注册表项。您也可以将 DNS 设置从手动切换到自动，但您将失去第三方 DNS 服务的优势(可能速度更快)，至少与您的 ISP 相比是这样。