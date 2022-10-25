# Windows 10 不让怎么卸载 Edge Chromium

> 原文：<https://lifehacker.com/how-to-uninstall-edge-chromium-when-windows-10-wont-let-1844297854>

[Edge Chromium 是一款像样的网页浏览器](https://lifehacker.com/how-to-try-out-edge-chromiums-latest-features-months-be-1842562597) 。鉴于谷歌 Chrome 在内存使用方面的改进，我甚至可以说它值得从谷歌 Chrome 换过来。然而，微软一直对 [向每个人灌输 Edge Chromium](https://www.express.co.uk/life-style/science-technology/1292563/Google-Chrome-Microsoft-Edge-best-browser-adverts-Windows-10-gmail) 非常恼火，最近的一次 Windows 更新甚至将这款浏览器锁定在你的操作系统中。



当然，你可以将 Firefox 或 Opera 等其他应用程序设置为默认网络浏览器，并忽略 Edge 的存在(以及 Windows 10 不断发出的“尝试新 Edge”的通知)，但如果你从未打算使用 Edge Chromium，最好将其完全移除。

问题是，如果你试图从系统设置中的应用和功能菜单卸载浏览器，Edge 旁边的**“卸载”**按钮现在是灰色的。如果你和我一样，你可能会跳到控制面板，通过“程序和功能”标签卸载它...除此之外，更新还从已安装程序列表中删除了 Edge，因此它也不能以这种方式卸载。

这是有原因的:一些微软应用程序需要 Edge 才能正常运行，所以 [微软加大了卸载 Edge](https://wccftech.com/microsoft-says-you-cant-uninstall-microsoft-edge-browser/) 的难度，以避免因其不存在而导致的不必要的问题(它只是真的希望你使用 Edge)。

这并不意味着 Edge Chromium 必须永久驻留在你的电脑上——你只需要更有创造性地删除它。不，你不会通过卸载 Edge 来破坏 Windows，尽管如果你只是想禁用它并设置一个不同的浏览器作为你的默认应用，我们也会告诉你如何做。

### **如何禁用 Edge 并设置不同的默认浏览器**

鉴于 Windows 10 漏洞百出的历史以及该操作系统对 Edge 的依赖，切换到新的浏览器可能比完全卸载它更安全。

1.  打开开始菜单
2.  点击**设置**，进入**应用>默认应用。**
3.  向下滚动并点击**“网络浏览器”**
4.  选择您想要使用的浏览器，显然您需要先安装该浏览器才能进行切换。如果您需要推荐，请查看我们的列表，获得最佳广告拦截浏览器和最佳隐私浏览器。
5.  您也可以通过右键单击任务栏图标并选择**“从任务栏取消固定”来取消固定 Edge**

这将在大部分时间隐藏 Edge，但 Windows 仍会偶尔建议使用浏览器，一些应用程序甚至会在更改默认程序后打开 Edge 中的链接——但如果这些行为让你感到困扰，你可以从你的 PC 中删除它。

### **如何卸载边缘铬**

尽管微软努力阻止用户删除 Edge，但你可以通过一些简单的 PowerShell 魔法从 Windows 10 中卸载它。我们将介绍两种可能的选择，以防其中一种不适合您。

### **方法一:**

1.  打开 Windows 文件浏览器
2.  在地址栏中输入**“C:\ Program Files(x86)\ Microsoft \ Edge \ Application”**，点击**进入**。这将打开 Edge 安装文件夹，如果没有，请尝试手动导航到该文件夹，或者在文件资源管理器中搜索“Edge”。
3.  应该有一个用数字命名的文件夹。该名称与您电脑上安装的 Edge 的当前版本相同。比如我写的时候，我机器上的文件夹是**“83 . 0 . 478 . 58。”**打开文件夹。
4.  找到并打开**“安装程序”**文件夹。
5.  在这个文件夹中，点击文件浏览器窗口左上角的**“文件”**标签，然后进入**文件>打开 Windows PowerShell >以管理员身份打开 Windows PowerShell。**
6.  当提示允许程序对您的系统进行更改时，单击**“是”**。
7.  在 PowerShell 中键入`.\setup.exe -uninstall -system-level -verbose-logging -force-uninstall`并按**回车**来运行命令并让它运行。

假设一切按计划进行，Edge 现在应该被卸载了。然而，如果这个方法对你不起作用，你可以试试另一个选择。

### **方法二:**

1.  从任务栏或 Windows 开始菜单中搜索“PowerShell”。
2.  从搜索结果中右键单击“Windows PowerShell”，然后选择**“以管理员身份运行”**
3.  当询问是否允许程序对您的系统进行更改时，选择**“是”**。
4.  在 PowerShell 窗口中，键入`get-appxpackage *edge*`并按回车键。
5.  将显示几行信息。查找**“package full name”**并复制列中的文本。
6.  在 PowerShell 中键入`remove-appxpackage`并粘贴从 PackafeFullName 列中复制的文本。
7.  按**回车**运行命令。Edge 现在应该从您的系统中删除。

更新了这篇文章，增加了更多关于为什么微软阻止浏览器被删除的信息，以及删除/禁用浏览器的两种方法。

[ [极客杂志](https://geekermag.com/uninstall-microsoft-edge-if-uninstall-button-is-greyed-out/) ，[appals](https://appuals.com/how-to-uninstall-microsoft-edge/)]