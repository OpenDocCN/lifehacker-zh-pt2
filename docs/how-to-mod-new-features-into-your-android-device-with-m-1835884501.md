# 如何用 Magisk 和 Xposed 框架定制你的 Android 设备

> 原文：<https://lifehacker.com/how-to-mod-new-features-into-your-android-device-with-m-1835884501>

在 Android 与 iOS 的辩论中，Android 通常因其开放性和灵活性而获得主要优势——Android 平台允许用户做很多 iOS 不能做的事情，甚至最基本的开箱即用的 Android 设备也可以根据你的喜好进行调整和定制。然而，发烧友想要的不仅仅是调整系统设置，这也是 Xposed Framework 和 Magisk 等工具发挥作用的地方。



有了这些工具，你可以安装 mod，以疯狂的方式改变你的设备，允许你加入杜比全景声、更多表情符号或对设备 wifi 功能的高级控制等功能。你可以使用 mods 为你的智能手机设计定制的界面，如果你够大胆的话，还可以提升你的设备的性能，使其超越默认值。

## 首先，你必须扎根

在我们继续之前，一个简短的声明:你需要 root 你的设备来安装 Xposed。 [给你的手机找根并不难](https://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) ，但它仍然有风险，因为从技术上来说，它会使你的保修失效。虽然现在做起来比过去容易，但一团乱可能会导致令人不快的故障，甚至损坏你的设备(尽管不太可能)。

其他不那么可怕的副作用包括触发谷歌的 SafetyNet API，这是 Android 操作系统中的一项安全措施，将停止一些应用程序/功能的工作，如谷歌 Play 商店、Google Pay、网飞，当然还有口袋妖怪。

我们将使用 Magisk 来隐藏系统的根目录，这应该会保持这些功能的完整性，但即使您按照正确的步骤操作，有些功能也可能无法正常工作。好消息是什么？如果某些东西停止工作，卸载 Magisk 并解除你的设备 是很容易的。

## 安装 Magisk 和 Xposed 框架

乍一看，这一长串的步骤似乎让人不知所措，但是一旦你正确地设置好一切，整个过程就很容易了。

### 步骤 1:准备好你的设备

收集适当的材料。您将需要:

*   您想要修改的 Android 设备
*   个人电脑
*   一根 USB 电缆将两者连接起来

准备好工具后，是时候准备您的 Android 设备了:

1.  首先，通过进入**设置>关于**(或者无论如何你在你的特定设备 上到达 [)来启用开发者模式。向下滚动并连续点击**“Build number”**七次。](https://www.greenbot.com/article/2457986/how-to-enable-developer-options-on-your-android-phone-or-tablet.html)
2.  一旦进入开发者模式，进入**设置>系统>高级>开发者选项**。找到并启用**[**USB 调试**](https://developer.android.com/studio/debug/dev-options) **。”****
3.  **接下来，下载并安装最新的 [Magisk Manager。来自 Github](https://github.com/topjohnwu/Magisk/releases/)T3 的 apk 文件(如果询问，点击允许从未知来源安装)。**

**现在还不要担心打开 Magisk 管理器。现在，我们将转到指南的 PC 部分。**

### ****第二步:使用 TWRP 安装 Magisk，并安全地为您的手机设置根目录****

1.  **通过 USB 将您的手机连接到 PC。**
2.  **在您的 PC 上，下载 ADB、Fastboot 和必要的驱动程序。最简单的方法就是使用 XDA 开发者论坛 的这个 [一体化安装包。按照下载页面上的说明操作，完成后返回这里(最多只需要几秒钟)。](https://forum.xda-developers.com/showthread.php?p=48915118#post48915118)**
3.  **接下来， [进入这个页面，为你的安卓设备下载](https://twrp.me/Devices/)TWRP 的正确版本。然后，解压并打开 TWRP 文件夹。**
4.  ****Shift +右键点击**TWRP 文件夹白色区域内的任意位置，打开命令提示符。**
5.  **在命令提示符窗口中，键入:`adb reboot bootloader`。**
6.  **如果您的设备请求允许 USB 调试，点击**“是”**您的设备应该以引导模式重启。**
7.  **键入`fastboot flash recovery twrp-2.8.x.x-xxx.img`，确保更改。IMG 文件名来匹配。TWRP 文件夹里的 IMG 文件。**
8.  **命令完成后，在命令提示符下运行命令`fastboot reboot`结束 PC 步骤。**

**您现在可以断开您的 Android 设备，我们将进入安装 Magisk 的最后步骤。**

1.  **当您的 Android 设备重新启动时，打开 Magisk manager 应用程序**
2.  **在“Magisk 未安装”旁边，点击**“安装”****
3.  **点击**“仅下载 Zip 文件”**等待下载完成，并记下其位置。**
4.  **关掉你的手机。然后，引导进入恢复模式。(执行此操作的过程因设备而异，但通常需要按住音量和电源按钮，直到设备打开。)**
5.  **当 TWRP 恢复模式菜单出现时，点击**“安装”****
6.  **导航到 Magisk。ZIP 文件位置，然后滑动滚动条进行安装。**
7.  **安装完成后，重新启动您的设备。**
8.  **设备重新启动后，再次打开 Magisk 管理器。您应该在 Magisk 和 Magisk manager 旁边看到绿色复选标记。**
9.  **通过点击 Magisk 管理器左上角的汉堡包图标，验证您的手机已成功根入并通过 SafetyNet 的检查。向下滚动并点击**“开始安全网检查”**如果您获得绿色复选标记，则一切就绪。**

### **步骤 3:安装 Xposed 框架**

**我们在最后冲刺阶段。剩下要做的就是使用 Magisk Manager 将 Xposed 作为一个模块安装。**

1.  **转到 Magisk 管理器中的“下载”部分。**
2.  **向下滚动并轻按“曝光”**
3.  **从列表中选择您的 Android 版本，然后安装 Xposed。**
4.  **重新启动设备以完成安装。**

### **有趣的部分:安装 Android mods**

**咻！如果你做到了这一步，你就已经成功地在手机上安装了 Magisk 和 Xposed，现在你可以开始修改 Android 了。就像我们一开始说的，这是令人兴奋的地方。(也很容易。)**

**打开手机上的 Magisk Manager 或 Xposed 应用程序，导航到它们的菜单以下载模块。每个应用程序的安装过程可能略有不同，但都需要您在安装每个模块后重新启动。**

**如果你想知道从哪里开始，这里有一些可用的最佳 Xposed 和 Magisk 模块的快速列表，你可以参考 XDA 开发者的列表 [最佳 Magisk](https://www.xda-developers.com/magisk-modules/) 和 [Xposed 模块](https://www.xda-developers.com/best-xposed-modules/) 以获得建议(注意:一定要检查这些模块是否与你的 Android 版本兼容，因为支持可能会有所不同)。**

**<iframe data-src="https://lifehacker.com/embed/inset/iframe?id=youtube-video-9xfgg4fHH-E&amp;start=0" data-chomp-id="9xfgg4fHH-E" data-recommend-id="youtube://9xfgg4fHH-E" id="youtube-9xfgg4fHH-E" data-recommended="false" width="800" height="450" class="core-inset lazyload" frameborder="0" scrolling="no" allowfullscreen="" webkitallowfullscreen="webkitAllowFullScreen" mozallowfullscreen="mozallowfullscreen"><span data-chomp-id="9xfgg4fHH-E" data-recommend-id="youtube://9xfgg4fHH-E" id="youtube-9xfgg4fHH-E" data-recommended="false" class="js_recommend"/></span></div><ul data-type="List" data-style="Bullet" class="sc-1lmbno3-0 dpuHif"><li><span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/xposed/modules/mod-nlpunbounce-reduce-nlp-wakelocks-t2853874&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/xposed/modules/mod-nlpunbounce-reduce-nlp-wakelocks-t2853874" target="_blank" rel="noopener noreferrer"> <strong>【放大电池(x 曝光)</strong> </a> </span>:可以增强您的电池寿命和设备性能，并让用户实时跟踪哪些应用和进程消耗的电量最多。</li><li><span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/android/development/howto-install-xposed-dolby-atmos-best-t3509649&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/android/development/howto-install-xposed-dolby-atmos-best-t3509649" target="_blank" rel="noopener noreferrer"> <strong>杜比全景声</strong> </a> </span> <strong> (Magisk): </strong>为一些正常情况下不具备杜比全景声的 Android 设备增加了支持。</li><li><span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/xposed/modules/app-gravitybox-v8-0-0-beta-1-tweak-box-t3739929&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/xposed/modules/app-gravitybox-v8-0-0-beta-1-tweak-box-t3739929" target="_blank" rel="noopener noreferrer"> <strong>【重力盒(Xposed) </strong> </a> </span> <strong> : </strong>这个流行的 mod 可以让用户自定义 Android OS 界面的很多方面。</li><li><span><a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/apps/magisk/module-tethering-enabler-testers-t3476625&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/apps/magisk/module-tethering-enabler-testers-t3476625" target="_blank" rel="noopener noreferrer"><strong>【Magisk】</strong></a></span><strong>:</strong>允许您覆盖制造商的设备共享设置，以防您的设备被禁止这样做(无论出于何种原因)。</li><li><span><a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/showthread.php?t=2191223&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/showthread.php?t=2191223" target="_blank" rel="noopener noreferrer"><strong>【viper 4 Android(Magisk)</strong></a></span><strong>:</strong>允许用户定制和增强许多音频相关的设置和功能，包括音量、扬声器输出和蓝牙设置。</li><li><span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://forum.xda-developers.com/xposed/modules/mod-xuimod-v2-3-listview-anim-t2477558&quot;,{&quot;metric25&quot;:1}]]" href="https://forum.xda-developers.com/xposed/modules/mod-xuimod-v2-3-listview-anim-t2477558" target="_blank" rel="noopener noreferrer"> <strong> XUI 系统 UI </strong> </a> </span> <strong> (Xposed): </strong>又一个 UI 编辑器，给你新的动画玩，让你自定义系统时钟、锁屏、通知等等。<br/></li></ul> </body> </html></iframe>**