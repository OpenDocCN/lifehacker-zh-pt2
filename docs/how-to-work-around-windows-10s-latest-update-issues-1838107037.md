# 如何解决 Windows 10 的最新更新问题

> 原文:[https://life hacker . com/how-to-work-around-windows-10s-latest-update-issues-1838107037](https://lifehacker.com/how-to-work-around-windows-10s-latest-update-issues-1838107037)

又来了。时间线有点乱，所以这次尽量和我们在一起。微软上周发布了一个 Windows 更新，修复了之前补丁中的一个错误，该错误导致了意外的 CPU 峰值，降低了用户台式机和笔记本电脑的性能。这个补丁自带了一些烦人的 bug，微软(和其他用户)正在努力解决。

Watch

第一次安全更新， [KB4515384](https://support.microsoft.com/en-gb/help/4515384) ，修复了 CPU 尖峰问题，但它也增加了一些额外的问题。这些问题包括破坏开始菜单搜索功能——当你搜索项目时，给你一个没有答案的大屏幕——以及在各种游戏中导致一些意想不到的音频问题。

微软已经将导致游戏玩家声音神秘消失、音量大幅降低或失去低音(仅举几个例子)的变化*回滚*。它还发布了一个更新，为游戏玩家解决他们遇到的任何问题提供了一些建议:

> *"要缓解此问题，请打开受影响游戏中的设置并禁用多声道音频(如果此选项可用)。您还可以在 Windows 控制面板中搜索第三方音频设备控制面板，并禁用多声道音频或虚拟环绕声(如果这些选项可用)。我们正在制定解决方案，估计 9 月下旬会有解决方案。”*

那些受影响的人发现的其他潜在修复方法包括 [降低你的采样率](https://old.reddit.com/r/Windows10/comments/d2unnp/kb4515384_september_10_caused_significant/ezxjth9/) (在你的扬声器或耳机属性窗口的高级选项卡上)，完全卸载 KB4515384(通过 Windows Update >查看更新历史)，甚至是 [禁用你的扬声器或耳机属性的“增强”选项卡下的所有音效](https://old.reddit.com/r/Windows10/comments/d32vfg/volume_decreases_a_lot_close_to_no_sound_after/ezyodnj/) 。

至于窗口搜索问题——另一个大问题——Reddit 用户 [**CptBrian**](https://www.reddit.com/r/Windows10/comments/d2apfk/cumulative_updates_september_10th_2019/ezwjono/) 发布了一个潜在的解决方法，也许可以让你重新开始运行:

> “我在安装 1903 后出现了空白搜索的问题，但我通过简单的注册表编辑解决了这个问题。
> 
> *注册表编辑:*
> 
> `[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Search]“CortanaConsent”=dword:00000001`
> 
> *基本上就是把 CortanaConsent 的值从 0 改成 1。这可能需要重新启动或注销。"*

你也可以试着浏览一下微软关于修复 [Windows Search](https://support.microsoft.com/en-us/help/4520146/fix-problems-in-windows-search) 问题的一般性建议，但是我敢打赌，这些更简单的故障诊断技巧可能对你没什么好处。如果你没有发现任何成功，你总是可以卸载更新(如前所述)，并确保你 [暂停自动安装未来的更新](https://lifehacker.com/how-to-undo-and-prevent-windows-updates-1836420965) 一段合理的时间。(我自己会给它 14 天左右，只是为了彻底，但你选择的时间取决于你。)