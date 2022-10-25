# 检查您的华硕和华为路由器以修复此 Wifi 漏洞

> 原文：<https://lifehacker.com/check-your-asus-and-huawei-routers-to-fix-this-wifi-vul-1841958252>

然而 [另一个主要的固件漏洞](https://lifehacker.com/how-to-check-your-usb-devices-for-unsafe-firmware-1841773522) 被发现，使得*数十亿*来自苹果、谷歌、亚马逊的手机、路由器和其他无线设备暴露在间谍活动之下。

Watch

这个被称为“Kr00k”的漏洞是由 ESETt 数据安全公司发现的，并在最近的一篇论文 中披露。Kr00k 影响某些 wifi 芯片加密数据的方式；当受影响的 wifi 设备断开连接时，正在进行的通信会被错误地加密，密钥仅为 0，很容易被解密。黑客可以破坏 wifi 信号的稳定性来触发漏洞，然后拦截并读取易受攻击的数据。( [Ars Technica 关于 Kr00k bug 的报道](https://arstechnica.com/information-technology/2020/02/flaw-in-billions-of-wi-fi-devices-left-communications-open-to-eavesdroppng/) 对感兴趣的人有更进一步的技术细节。)

虽然以这种方式收集的信息很难被黑客成功利用，但它仍然是一个很大的安全威胁，用户应该采取必要的措施，通过安装最新的更新来确保他们的设备安全。虽然你的大多数设备都可以(或已经)通过软件补丁进行修复，但你至少要确保你的 wifi 路由器使用的是最新的固件，因为它们通常不会自动更新

以下是确认存在 Kr00k 漏洞的产品列表:

### **手机和平板电脑**

*   亚马逊 Kindle 第八代
*   谷歌 Nexus 5、6 和 6S
*   iPad mini 2
*   iPhone 6，6S，8，XR
*   三星 Galaxy S8 和 S4 GT-I9505
*   小米 Redmi 3S

### **路由器**

*   华硕 RT-N12
*   华为 B612S-25d
*   华为 EchoLife HG8245H
*   华为 E5577Cs-321

### **其他设备**

*   亚马逊 Echo 第二代智能音箱
*   苹果 MacBook Air Retina 13 英寸(2018)
*   树莓 Pi 3

其他设备也可能携带该漏洞，因此您应该确保您的 wifi 设备使用制造商提供的最新固件或软件更新。如果最近没有可用的，记下一个月左右再来查看(以防万一)。

还建议用户在其设备的 web 浏览器上打开 HTTPS 域名系统(DoH )(如果有),以防止任何攻击者看到您访问的网站。您可以查看我们的 DoH 和 [wifi 安全](https://lifehacker.com/introducing-lifehackers-complete-guide-to-wifi-1836980730) 指南了解更多信息。