# 如何让 uBlock Origin 在火狐的广告拦截上更胜一筹

> 原文：<https://lifehacker.com/how-to-make-ublock-origin-even-better-at-ad-blocking-in-1839964889>

Firefox 是阻止广告和垃圾网页跟踪器的最佳浏览器之一，你可以使用“nuke-'em-all”浏览器扩展，如 [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) ，让它变得更好。现在， [Ghacks](https://www.ghacks.net/2019/11/20/ublock-origin-for-firefox-addresses-new-first-party-tracking-method/) 和 GitHub 的用户指出，uBlock Origins 甚至能够阻止新型广告、追踪器和网站内容，这是 Chrome 等浏览器无法(或不愿)阻止的，即使安装了插件。

Watch

这种特殊内容使用规范名称(CNAME)记录，通过告诉浏览器正在显示的内容是需要在网站上显示的重要第一方内容来通过内容阻止程序。如果你在 Firefox 上使用 uBlock Origin，情况就不一样了，Firefox 也在测试一种阻止这种令人讨厌的变通方法的方法——在浏览器对其竞争对手 的青睐中又增加了 [。](https://lifehacker.com/why-you-should-switch-from-google-chrome-to-firefox-1821879163)

uBlock Origin 为 Firefox 扩展的 CNAME 阻止功能目前正在测试中，但一旦该插件的版本 1.24.1 下降，很快就会在 Firefox 中提供。无论你现在获得测试版还是等待下一个稳定的更新，用户都必须授予 uBlock Origin 一个新的权限来“访问 IP 地址和主机名信息”之后，您需要调整一些附加组件的设置来启用高级广告拦截:

1.  在 Firefox 地址栏中输入**“about:addons”**并按回车键打开扩展设置
2.  点击**“…”uBlock Origins 旁边的**图标，然后点击**“选项”**
3.  勾选**“我是高级用户”**框，然后点击旁边出现的**齿轮状图标**
4.  在下一个窗口中，从列表中找到 **"cnameAliasList"** ，并将设置值更改为" * "
5.  点击**“应用更改”，**然后关闭选项。你可能需要重启 Firefox

在这些设置被更改后，uBlock Origins 将能够使用 CNAME 记录过滤掉那些讨厌的广告和跟踪器。