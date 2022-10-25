# 如何找回你丢失的火狐密码

> 原文：<https://lifehacker.com/how-to-recover-your-missing-firefox-passwords-1835616191>

火狐用户最近打开浏览器，发现他们所有保存的密码都不见了。如果这发生在你身上，不要担心:你的密码没有去任何地方，尽管看起来是这样。

Watch

据 [Mozilla](https://bugzilla.mozilla.org/show_bug.cgi?id=1558765) 报道，该问题涉及 AVG 反病毒应用程序的一个功能( [密码保护](https://support.avg.com/SupportArticleView?l=en&urlName=Activate-AVG-Password-Protection) )与浏览器 67.0.2 版本(一周前发布)中推出的新 Firefox 证书之间的不兼容。正如 Mozilla 所写的:

> “AVG 团队已经能够在 AVG 的一个功能(密码保护)中找到问题的根源。该产品保护用户免受存储在 Firefox 和其他浏览器中的密码被盗的风险。对于 Firefox，它只允许由 Firefox 证书签名的进程访问存储。
> 
> 我们已经能够识别将证书信任传播到我们所有系统的问题。FF 67.0.2 由 2019 年 5 月 31 日起生效的新颁发证书签署，问题很可能是由此引起的。我们已经手动修复了后端的内部证书标志，并更新了未来证书更新的流程(预计不迟于 2020 年 6 月 4 日)"

要解决这个问题，你应该采取两个步骤。首先，你必须 [更新 AVG](https://support.avg.com/SupportArticleView?l=en&urlName=Update-AVG-Antivirus&supportType=home) 到最新的病毒定义——版本至少是 19061402。在此过程中，您可能需要重新启动电脑，因此请确保您已经保存了正在进行的任何操作。

接下来，你需要 [安装这个火狐插件](https://addons.mozilla.org/en-US/firefox/addon/restore-logins/) 来恢复你保存的密码。如果这对你不起作用，或者你更喜欢用手动方式做事，这里有 [步骤](https://support.mozilla.org/en-US/kb/passwords-disappearing-avg-security-software?redirectlocale=en-US&redirectslug=passwords-disappearing-avg-security) 附加复制:

1.  单击菜单按钮，单击帮助，然后选择故障排除信息。

2.  在“应用程序基础”下，单击“配置文件文件夹”旁边的“打开文件夹”按钮。
3.  关闭 Firefox
4.  检查您是否在个人资料文件夹中看到名为 *logins.json* 的文件。如果是这样，将其重命名为 *logins.json.old* 。
5.  检查您是否在个人资料文件夹中看到一个名为 *logins.json.corrupt* 的文件，日期为 2019 年 6 月。如果这样做了，右键单击该文件，复制它，然后将其重命名为 *logins.json* 。
6.  启动火狐。