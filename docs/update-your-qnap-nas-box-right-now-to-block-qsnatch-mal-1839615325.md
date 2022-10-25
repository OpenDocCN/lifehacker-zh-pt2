# 立即更新您的 QNAP NAS 盒，以阻止“QSnatch”恶意软件

> 原文:[https://life hacker . com/update-your-qnap-nas-box-right-now-to-block-qsna tch-mal-1839615325](https://lifehacker.com/update-your-qnap-nas-box-right-now-to-block-qsnatch-mal-1839615325)

我将继续下去，为我自己为“Qnap”和“恶意软件”这两个词设置了一个谷歌警报而感到自豪。我使用该公司的一个 NAS 盒，就像许多其他人一样，现在我有机会为我的设备接种疫苗，抵御正在传播的一种令人讨厌的新恶意软件。

Watch

这种恶意软件被称为 QSnatch，它将代码注入到 QNAP NAS box 的固件中，然后 QNAP NAS box 有能力调用命令控制服务器将*额外的*代码转储到您的设备上。最终，写到[芬兰国家网络安全中心](https://www.kyberturvallisuuskeskus.fi/en/news/qsnatch-malware-designed-qnap-nas-devices)写到，QSnatch 可以执行以下操作:

> *   *Operating system scheduled job and script are modified (cronjob, init script)*
> *   *Firmware update is blocked by completely covering the update source*
> *   *QNAP malware remover application is blocked from running*
> *   *All user names and passwords related to the device are retrieved and sent to C2 server*
> *   *Malware has modular ability, and can load new functions from C2 server for further activities*

换句话说，你的 NAS 盒基本上已经被冲洗干净了。

你如何防止这种情况？启动你的 NAS 盒，登录到基于网络的界面(你可以通过安装 [Qfinder Pro](https://www.qnap.com/en-us/utilities/essentials) 在简单模式下完成)，更新你设备的固件。如果有可用的更新，当您登录时，可能会提示您这样做。如果没有，在 NAS 盒的设置屏幕中会有一个检查更新的选项:

我会点击它，以确保您的设备运行的是最新版本的 QNAP 固件。但是，您的 NAS 盒可能很旧，像我的一样，没有更新。呃。在这种情况下，您可以尝试其他一些步骤。

首先，确保你使用的是 Qnap 安全顾问的最新版本——如果适用的话。调出 Nas 盒的“应用中心”如果安装了安全顾问，您应该能够更新它；如果没有，您应该能够找到并安装它。无论哪种方式，打开应用程序的最新版本，并在您的系统上运行全面扫描。

您的旧 NAS 盒可能无法运行安全顾问。如果是，那我们继续。你也应该能够从 Qnap 的应用中心的安全部分安装和运行“恶意软件清除程序”应用。这至少是从您的 NAS 设备中删除 QSnatch 的一个很好的方法(即使还没有人知道它最初是如何感染 NAS 设备的)。确保您运行的是版本“3.5.4.0”或“4.5.4.0”QNAP 建议，确保它能够检测并消除 QSnatch。

QNAP 还建议您启用“IP 和帐户访问保护”，如果您不使用这些连接，请禁用 SSH 和 Telnet，并且不要在您的 NAS 机器上使用默认端口号——所有设置都可以通过 [QNAP 的有用说明](https://www.qnap.com/en/security-advisory/nas-201911-01) 轻松更改。

否则，如果这些解决方案都没有帮助，并且您发现您的系统被感染了，完全的工厂重置应该可以清除恶意软件。在清除所有数据之前，不要忘记在其他地方备份数据。