# 如何修复 Chrome OS 72 的错误任务管理器

> 原文：<https://lifehacker.com/how-to-fix-chrome-os-72s-buggy-task-manager-1832727274>

如果你有一台 Chrome OS 笔记本电脑或平板电脑，你可能想推迟安装最新的 Chrome OS 更新。虽然此次更新为少数 Chrome OS 设备 带来了 Android 馅饼，但一些安装了该更新(Chrome OS 版本 72)的用户报告了 [性能问题](https://chromeunboxed.com/android-9-brings-crippling-bug-to-chrome-os-72-what-you-need-to-know/) 。到目前为止，谷歌的 Pixelbook 和 Pixel Slate，三星的 Chromebook Plus V2，以及惠普的 Chromebook X2 都受到了影响，但完整的设备列表可能会更长。



谷歌表示已经意识到这个问题 ，并且正在努力解决，但是还没有消息表明何时会推出针对这个问题的补丁。幸运的是，在你等待的时候，有几个步骤可以让你的设备再次提速。

### 不可靠的记忆

这些减速报告背后的罪魁祸首似乎是 Chrome OS 任务管理器。Chrome OS 72 更新中添加的新 Android Pie 功能包括 Chrome OS 任务管理器中的一个新工具，该工具可以报告应用程序或后台进程占用了多少 RAM。具有讽刺意味的是，正是这个特性导致系统由于异常高的 CPU 使用率而停滞不前——根据错误报告，从 50%到 100%不等。

这里最简单的解决办法是不安装 Chrome OS 72 更新，坚持使用版本 71。也就是说，许多用户已经安装了 Chrome OS 版本 72，无论是他们自己启动更新还是他们的设备自动更新。如果是你，就根本不用任务管理器，应该没问题。

正如 9to5Google 所指出的，一些在其 Pixelbook 或 Chromebook 上运行 Android Pie 的用户可能希望(或需要)使用任务管理器。在这种情况下，你需要禁用任务管理器中的内存使用报告功能: 

1.  按**“搜索+ESC”**打开 Chrome OS 任务管理器
2.  右键单击“任务”列标题，然后取消选中“内存占用”选项。这将删除内存占用列并禁用该功能。

当谷歌最终发布官方修复程序时，你应该有希望能够重新启用这个功能。

### 如果这不能解决问题，该怎么办

由于谷歌仍在调查这个 bug，我们介绍的解决方案可能无法完全解决这个问题。如果你已经尝试了这些修复，但在 Chrome OS 72 更新后仍然遇到系统变慢或其他错误，请确保向谷歌发送错误报告。

要在你的 Chrome OS 设备上这样做，按**“Alt+Shift+I”**调出 bug 报告表单。提供尽可能多的信息——比如你的设备型号、操作系统版本，以及你可能有的任何截图或系统日志——包括 [对这个错误报告](https://bugs.chromium.org/p/chromium/issues/detail?id=929359) 的引用。有了足够的信息，谷歌的开发团队应该有望很快解决这个问题。