# 保持你的 ZigBee 智能家居设备更新，以防止这种黑客攻击

> 原文:[https://life hacker . com/keep-your-ZigBee-smart-home-devices-updated-to-protect-1841476278](https://lifehacker.com/keep-your-zigbee-smart-home-devices-updated-to-protect-1841476278)

被一个电灯泡黑了？这听起来很傻，但 Check Point Software 的安全研究人员最近证明，如果有人利用灯泡用于与网桥通信的 ZigBee 协议中的漏洞，未经修补的飞利浦 Hue 智能灯将被用作进入您网络的攻击媒介。

Watch

我意识到这有点拗口。黑客的实际操作要有趣得多——呃，读一读吧。一旦攻击者设法将修改过的固件上传到一个受损的旧灯泡，Check Point 描述了其余的乐趣:

> 1.  *Hackers control the color or brightness of the light bulb, making users mistakenly think that the light bulb is faulty. The light bulb is displayed as "untouchable" in the user's control application, so they will try to "reset" it.*
> 2.  *The only way to reset the light bulb is to delete it from the app and then instruct the control bridge to rediscover the light bulb.*
> 3.  *The bridge found the damaged light bulb, and the user added it back to their network.*
> 4.  *The hacker-controlled light bulb triggers the heap-based buffer overflow on the control bridge by updating the firmware, then using the ZigBee protocol vulnerability and sending a large amount of data to it. This data also enables hackers to install malicious software on the network bridge, and then connect to the target enterprise or home network.*
> 5.  *Malware connects back to hackers and exploits known vulnerabilities (such as* [*Eternal Blue*](https://en.wikipedia.org/wiki/EternalBlue) *). They can infiltrate the network bridge into the target IP network to spread ransomware or spyware.*

飞利浦在 1 月中旬更新了 Hue Hub 的补丁，以修复这一特定漏洞，但值得快速查看一下，以确保它运行的是最新的固件。为此:

1.  在 Android 或 iOS 上打开你的 Hue 应用
2.  点击“设置”
3.  向下滚动一点，点击“软件更新”
4.  比你应该等待的时间更长
5.  寻找你的“飞利浦 hue”集线器，并确保它至少运行“1935144040”，即 1/24/20 更新，如果我没记错的话。

如果不是，并且您的设备没有任何可用的更新，请耐心等待。你应该(希望？)快收到吧。与此同时，我建议你确保使用 Hue 应用程序中的“自动更新”功能，这样你就不必再亲自检查更新了。

如果你碰巧拥有任何其他智能家居设备，也给他们看看；如果他们使用 ZigBee 进行通信，你会想要保持在他们更新的顶部(或者告诉他们自动更新)，这样任何未来的漏洞都不会让你或你的家措手不及。

如果你的灯开始像幽灵一样闪烁，不要冲动去重置你的设置。考虑换一个普通的灯泡，在你排除故障的时候隔离 VLAN 上的 Hue Hub 之类的东西——这可能需要打电话给客户支持，因为我真的不知道如何用正确的、更新的固件来覆盖被黑的灯泡...如果有可能的话。正如 [濒临](https://www.theverge.com/2020/2/5/21123491/philips-hue-bulb-hack-hub-firmware-patch-update) 所言:

> *...看来，灯泡本身仍然容易受到黑客攻击。Check Point 写道，当那架飞行无人机在 2016 年引发一种微型物联网病毒时，公司找到了一种方法，通过限制灯泡之间的跳跃来解决最糟糕的情况。但是“由于设计限制”，灯泡的脆弱性仍然存在，导致了新的黑客攻击——也许在我们的未来还有其他尚未发现的黑客攻击，只要这些灯泡仍然在使用。让这些灯泡易受攻击可能比让黑客随意开关你的灯更危险。”*