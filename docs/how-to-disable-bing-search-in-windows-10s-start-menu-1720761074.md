# 如何在 Windows 10 的开始菜单中禁用必应搜索

> 原文：<https://lifehacker.com/how-to-disable-bing-search-in-windows-10s-start-menu-1720761074>

我之前使用了一个聪明的黑客技术来阻止 Bing 出现在 Windows 10 的内置搜索结果中，但重新安装该操作系统并用 2020 年 5 月的更新打补丁让 Bing 回来了。我不反对任何人*希望*将这种体验融入他们的操作系统，但对于那些不想这样做的人，你必须尝试一些新的技巧来永远抛弃 Bing。

Watch

如果你运行的是**Windows 10 Home**(2020 年 5 月更新) [，一个简单的注册表调整](https://superuser.com/posts/1531112/revisions) 应该足以将必应从你操作系统的搜索结果中移除。打开开始菜单，键入“regedit”，并启动 Windows 注册表编辑器。然后，导航到该键:

`HKEY_CURRENT_USER\SOFTWARE\Policies\Microsoft\Windows\Explorer`

如果它不存在，而你被困在“Windows”文件夹中，只需右键单击右边栏并创建一个新的密钥。将其命名为“探索者”，不带引号。单击左侧边栏中新键，然后再次右键单击右侧边栏并创建一个新的 DWORD (32 位值)。将其命名为“DisableSearchBoxSuggestions”，不带引号或逗号。然后，双击它，并将其值设置为 1。最后，重启你的电脑。

这是 Windows 10 的搜索框在这次小攻击之前的样子:

这是之后的样子:

幸福的寂静。我非常高兴。

如果您没有最新版本的 Windows，那么您需要导航到不同的注册表项来禁用 Bing: `HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Search`

您需要创建或编辑以下 DWORD (32 位)值，并在注册表编辑器中将它们设置为“0”:

*   `BingSearchEnabled`
*   `CortanaConsent`

### **在 Windows 10 Pro 上禁用 Bing**

如果你更喜欢运行 Windows 10 Pro 而不是 Home，你*应该能够使用组策略设置而不是注册表调整来达到同样的效果。打开你的组策略编辑器(通过开始菜单的“编辑组策略”链接)，在左侧边栏打开以下内容:**用户配置>管理模板> Windows 组件>文件浏览器**。*

从那里，在右边栏寻找“关闭文件浏览器搜索框中最近搜索条目的显示”。双击它并将其设置为“启用”，然后单击确定，退出其他所有操作，并重新启动 Windows 10。这应该具有相同的效果，如下所示:

*本文最初由 Eric Ravenscraft 于 2015 年发表。大卫·墨菲(David Murphy)在 2020 年 6 月重写了它，以纳入最新版本 Windows 10 的新信息。*