# 使用此 Windows 10 PowerToy 一次重命名多个文件

> 原文:[https://life hacker . com/rename-multiple-files-at-once-with-this-windows-10-power-1839454901](https://lifehacker.com/rename-multiple-files-at-once-with-this-windows-10-powe-1839454901)

微软掉了一个全新的开源 Windows 10 PowerToy，它和另外两个 一样好玩有用。这个新增的“PowerRename”为您提供了一个在文件资源管理器中批量重命名文件的简单方法。它免费、简单，值得花 10 秒钟安装到您的系统上。

Watch

首先，点击微软 PowerToys 的 [GitHub](https://github.com/microsoft/PowerToys) ，下载最新发布的。一旦你安装了它，所有三个 PowerToys——fancy zones、PowerRename 和快捷键指南——都应该默认启用，但你可以通过右键单击任务栏中的小图标并选择“设置”来检查这一点

假设 PowerRename 正在运行，你所要做的就是打开文件资源管理器，选择几个你想要重命名的文件，点击右键，从上下文菜单中选择“PowerRename”。

由此，PowerRename 很容易理解。在顶部字段(*“搜索”*)中键入您想要将*更改为*的任何文本，并将您想要将*更改为*的任何文本放在底部字段(*“替换为”*)——就像您刚刚在上面的动画中看到的那样。

我喜欢 PowerRename 的一点是，你可以在(适当命名的)预览窗口中实时预览你的更改，这样你就可以确保你正在尝试做的事情——无论你选择什么选项，如果你使用这些选项的话——都能完美地完成。

说到这个，如果你好奇这些选项是做什么的，这里有微软的 [快速描述](https://github.com/microsoft/PowerToys/tree/master/src/modules/powerrename) :

> *   ***Use regular expression:** If selected, the search field will be interpreted as a regular expression. If unchecked, the search field will be used as the text in the replacement field.*
> *   ***Case sensitive:** If selected, the text specified in the search field will only match the same uppercase and lowercase text in the entry. By default, our matching is case-insensitive.*
> *   ***Match all matches:** If selected, all the matches of the text in the search field will be replaced with the replacement text. Otherwise, only the first instance (from left to right) of the search text in the project will be replaced.*
> *   ***Excluded files:** files will not be included in the operation.*
> *   ***Excluded folder:** folder will not be included in the operation.*
> *   ***Exclude items in subfolders: items in** folders will not be included in the operation. By default, all subfolder items are included.*
> *   ***Enumeration items:** A numeric suffix is appended to the file name modified in the operation. Example: foo.jpg- 【T4] Spitfire ①. jpg*
> *   ***Only project name:** Operation only modifies the file name (not the file extension). ex:txt . txt- > newname . txt*
> *   ***Only project extension:** The operation only modifies the file extension (not the file name). Ex: txt.txt - > txt。 new extension* T54

不过，老实说，这一切让 PowerRename 听起来比实际复杂得多。你可能会对基本的搜索/替换功能感到满意，而预览呢？它让我像厨师一样亲吻我的手指。多么伟大的小工具。