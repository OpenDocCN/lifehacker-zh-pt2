# 如何通过禁用密码恢复问题来保护 Windows 10

> 原文：<https://lifehacker.com/how-to-secure-windows-10-by-disabling-its-password-reco-1831001538>

密码恢复问题已经成为 Windows 10 的一部分一年多了，但如果你使用微软账户登录你的操作系统，你永远不会知道它们的存在。但是，当您首次安装 Windows 时，请使用本地帐户，系统会提示您创建三个安全问题，如果您忘记了凭据，您可以使用这些问题来重置密码并登录您的帐户。



听起来很方便，对吧？不幸的是，安全问题对于账户安全来说并不是很重要， [就像我们之前讨论过的](https://lifehacker.com/use-your-password-manager-for-security-answers-too-1829498257) 。并不是说黑客很可能猜到你的高中名字，或者你的狗的中间名。因为默认情况下没有办法关闭*这些问题，所以攻击者只需成功闯入一次，就能为你制造一个新的安全问题——并永久入侵你的系统。*

这正是一组安全研究人员在最近的黑帽欧洲安全会议上描述的场景，正如 [Ars Technica](https://arstechnica.com/information-technology/2018/12/what-was-the-name-of-your-first-exploit-win-10-security-questions-open-backdoor/) 写道:

> 研究人员说，问题在于，在由成百上千台电脑组成的网络中，密码重置问题太容易设置，也太难监控。一个拥有管理员证书的人可以在任何 Windows 10 机器上远程打开或更改它们，并且没有简单的方法来监控或更改这些更改。因此，恶意用户——比如一名流氓员工或一名短暂获得未经授权的管理控制权的黑客——可以利用安全问题作为后门，秘密地允许他们在失去控制权时重新获得控制权。”

令人欣慰的是，研究人员(Magal Baz 和 Tom Sela，来自[illusion Networks](http://Illusive Networks))想出了一个快速 Powershell 脚本，可以用来永久禁用 Windows 的内置 Q & A。只需从 [这里](https://github.com/IllusiveNetworks-Labs/Update-AllUsersQA) 下载. ps1 文件，在 Windows 10 操作系统中打开 PowerShell，导航到包含. ps1 文件的文件夹，并输入以下内容来禁用恢复问题:

`Update-AllUsersQA`

当你试图在 Windows 10 登录屏幕上选择“重置密码”选项时，使用该命令会弹出一条错误消息。

如果你仍然想拥有*某种*类型的恢复选项，但是你想隐瞒该功能有效的事实，那么试试这个(用你*知道的*你会记得的恢复答案代替“SecretAnswer”):

`Update-AllUsersQA -answer SecretAnswer`

当你恢复密码时，你会看到一个小小的警告“此功能已被禁用”，但你可以安全地忽略它。如此隐秘；如此安全。