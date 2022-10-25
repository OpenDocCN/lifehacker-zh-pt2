# 更新 Android 以修复一个主要的蓝牙错误

> 原文:[https://life hacker . com/update-Android-to-fix-a-major-bluetooth-bug-1841523530](https://lifehacker.com/update-android-to-fix-a-major-bluetooth-bug-1841523530)

任何拥有运行 Android 8 或 9 的旧 Android 设备的人都需要警惕使用蓝牙。网络安全公司 ERNW 发现了一个漏洞，该漏洞允许蓝牙 Android 设备范围内的任何人访问该设备的存储。

Watch

黑客需要知道一些关于设备的额外细节——特别是它的蓝牙 MAC 地址——才能完全远程访问内部存储，但正如 [ENRW 的错误报告所解释的](https://insinuator.net/2020/02/critical-bluetooth-vulnerability-in-android-cve-2020-0022/) ，这相对容易解决。一旦他们进入，攻击者可以轻松地窃取个人文件，并在设备上安装恶意软件或其他间谍软件，而不会提醒手机用户。

2020 年 2 月发布的 [安卓安全补丁](https://source.android.com/security/bulletin/2020-02-01.html) 包含了对这个 bug 的修复，所以你应该通过标准的安卓 [系统更新流程](https://support.google.com/android/answer/7680439?hl=en) 下载并安装这个补丁。

ENRW 的错误报告还指出，早于 8.0 的 Android 版本也可能受到蓝牙漏洞的影响，但这些版本尚未经过测试。Android 10 上也存在该漏洞，但它无法被利用，所以没有风险(尽管 Android 10 用户仍然应该安装安全更新，因为它包括其他修复)。

如果因为你的 Android 太旧而无法安装 2020 年 2 月的安全更新，那么退而求其次的解决方案就是停止使用蓝牙。这使得黑客无法利用漏洞攻击你，尽管它也使你无法使用蓝牙配件。(希望你的设备还有一个 3.5 毫米耳机插孔。)

否则，如果可能的话，考虑关闭设备的蓝牙发现功能，或者在不使用蓝牙时，记住通过状态栏或从屏幕顶部向下滑动时看到的内容来关闭蓝牙。