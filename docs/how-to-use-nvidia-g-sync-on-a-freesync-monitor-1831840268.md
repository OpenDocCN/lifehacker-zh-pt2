# 如何在 FreeSync 显示器上使用 Nvidia G-Sync

> 原文：<https://lifehacker.com/how-to-use-nvidia-g-sync-on-a-freesync-monitor-1831840268>

上周，英伟达宣布计划推出纯软件版本的 G-Sync，其用于 PC 显示器的 [自适应同步工具](https://lifehacker.com/learn-the-basics-of-nvidias-g-sync-and-amds-freesync-mo-1831578473#_ga=2.255835912.1014487321.1547747405-396842925.1520800403) 。现在，随着 [GeForce 驱动程序 417.71](https://www.geforce.com/drivers/results/141906) 的公开，将 Nvidia 显卡与 FreeSync 显示器混合使用的一小群人可以尝试 G-Sync 的新实现。



英伟达表示，它正在测试自适应同步兼容显示器，看看哪些与 G-Sync 兼容。在测试了 400 台显示器之后——现在可能更多——该公司发布了一份 12 英寸 [G-Sync 兼容](https://www.nvidia.com/en-us/geforce/news/g-sync-ces-2019-announcements/) 显示器的短名单。如果你有其中的一个，那么你将自动享受“GeForce 兼容的可变刷新率体验”，正如 Nvidia 所说，如果你用最新的 GeForce 驱动程序玩游戏。

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-jqkIrhG0TcE&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-jqkIrhG0TcE&start=0) 

从技术上来说，Nvidia 新实施的 G-Sync 意味着你应该能够在任何支持 FreeSync 的显示器上使用该技术。但是，在开始游戏之前，您还需要进行一些配置:

### 如何让 G-Sync 在 FreeSync 显示器上工作

首先，你需要在你的电脑中安装英伟达 GTX 10 系列或更高版本的显卡，你需要使用 DisplayPort 电缆而不是 HDMI 将显示器连接到显卡。此外，请务必按下显示器上的菜单按钮，浏览其屏幕菜单，并确认“自由同步”或“自适应同步”已打开。

接下来，进入你电脑上的 Nvidia 控制应用程序。打开“显示”设置，点击“设置 G-Sync”在那里，选中“启用 G-Sync，G-Sync 兼容”旁边的框你可能应该坚持默认选项“启用全屏模式”，因为你可能会遇到在窗口游戏中运行 G-Sync 的问题— [，如果它甚至可以工作的话](https://www.reddit.com/r/pathofexile/comments/8inin9/gsync_poe_windowed_fullscreen_no_gsync/) 。

选中所有复选框后，单击“应用”

如果您有多台显示器，请确保在 Nvidia 控制面板中更改正确显示器的功能。支持自适应同步技术的显示器将在“设置 G-Sync”屏幕中显示绿色屏幕(以及 Nvidia 徽标的一部分)。

### 自由同步时 G-Sync 故障排除

如果您在让 G-Sync 与非 G-Sync 显示器配合使用时遇到问题，请不要惊慌。你可能需要先调整一些 Nvidia 控制面板的设置。尝试转到左侧面板中的“3D 设置”，然后单击“全局”向下滚动到“监视器技术”下拉菜单，并将其设置为“G-Sync 兼容”

如果这不起作用，请转到“显示器”部分的“更改分辨率”,尝试降低显示器的刷新率。你应该首先尝试将 G-Sync 设置为显示器的最大刷新率，但[pcgamens](https://www.pcgamesn.com/nvidia/how-to-enable-freesync-nvidia-graphics-card-gsync-compatible)发现 G-Sync 可能不总是支持显示器的全范围刷新率。如果你仍然有问题，请咨询 Reddit Nvidia 社区的 [众包测试电子表格](https://docs.google.com/spreadsheets/d/1YI0RQcymJSY0-LkbjSRGswWpJzVRuK_4zMvphRbh19k/edit#gid=1455257716)——他们有大量关于各种显示器可能需要更改的设置的注释，你可以交叉引用，看看其他人是否已经在你的特定 FreeSync 显示器上使用了 G-Sync。

要明确的是，有一个非零的机会，你会设置这个，并发现 G-sync 不能正常工作。如果你想在玩任何游戏之前尝试一个中立的测试，下载 Nvidia 的 [钟摆演示](https://www.nvidia.com/coolstuff/demos#!/g-sync) 用于测量图形性能，看看它看起来如何。(例如，用户报告说，一些未经批准的显示器在 G-Sync 下闪烁更多。)

PCWorld 在 CES 上的 Nvidia 展台测试了这项技术，它也有一个视频，可以帮助您了解当未经批准的显示器无法工作时，您会看到什么:

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-6yCiBbQh2fA&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-6yCiBbQh2fA&start=0)