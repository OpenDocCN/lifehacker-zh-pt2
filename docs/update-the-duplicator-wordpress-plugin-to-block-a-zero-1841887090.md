# 更新“复制器”插件来阻止零日攻击

> 原文：<https://lifehacker.com/update-the-duplicator-wordpress-plugin-to-block-a-zero-1841887090>

WordPress 插件它也有一个明显的漏洞，你会想要马上修补。否则，一个精明的攻击者可以使用这个插件从 WordPress 网站下载关键文件，比如你非常重要的 wp-config.php 文件。

Watch

一旦他们掌握了这一点，你的博客、电子商务网站或投资组合就会变得非常有趣。正如 [成立](https://www.tenable.com/blog/duplicator-wordpress-plugin-vulnerability-exploited-in-the-wild) 所描述的:

> *“未经验证的远程攻击者可以通过使用 Duplicator 插件的易受攻击版本向 WordPress 站点发送特制的请求来利用此漏洞。这将允许他们下载目标目录之外的文件。攻击者需要了解目标文件的结构，或者试图下载众所周知的文件。*
> 
> 这些文件可能包括 wp-config.php 文件，在 WordPress 安装中被称为“最重要的文件之一”。这是因为配置文件包含数据库凭证、认证密钥和 salts。攻击者可以利用这些信息在易受攻击的站点上创建自己的管理员帐户，或者“注入内容或获取数据”。”‘

根据 [Wordfence](https://www.wordfence.com/blog/2020/02/active-attack-on-recently-patched-duplicator-plugin-vulnerability-affects-over-1-million-sites/) ，复制器漏洞影响 1.3.26(含)之前的任何版本扩展，以及 3.8.7(含)之前的任何版本复制器 Pro 扩展。Duplicator 开发商 Snap Creek 已经发布了该问题的修复程序，所以你应该尽快将你的插件更新到版本 1.3.28(或者 3.8.7.1，用于 Duplicator Pro)。

为此，只需登录你的 WordPress 管理页面，点击插件。你可以查看任何有更新的插件，下载和安装新版本就像点击一个链接一样简单。

作为 [在](https://lifehacker.com/update-this-wordpress-plugin-to-prevent-a-site-hijackin-1841763512) 之前，我认为花几分钟时间安装一个插件来为你处理这个更新过程也是值得的，这可以确保你总是在插件启动时使用最新版本。

安装一个类似 [【伴侣自动更新】](https://wordpress.org/plugins/companion-auto-update/) 的 WordPress 插件，你就再也不用担心更新其他插件了。没错，如果某个更新打破了某个关键特性，这个 T4 就可能毁掉你的网站，但我认为对于大多数拥有 WordPress 博客或简单投资组合的人来说，使用自动更新程序是个好主意。