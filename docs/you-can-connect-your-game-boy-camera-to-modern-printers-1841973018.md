# 你可以用这个 20 美元的适配器将你的 Game Boy 相机连接到现代打印机上

> 原文：<https://gizmodo.com/you-can-connect-your-game-boy-camera-to-modern-printers-1841973018>

尽管它的图像质量(最大分辨率仅为 160x144 像素)，Game Boy 相机仍然是一个 [受欢迎的附件](https://gizmodo.com/an-old-school-film-trick-finally-brings-color-to-the-ga-1831339272) ，这在一定程度上要归功于一个可以打印出微小照片的廉价配件。但是，如今为 Game Boy 打印机寻找纸张并不是一件容易的事情，所以 Vaclav Mach 发明了一种[【20 美元】的适配器](https://www.tindie.com/products/xx0x/gbpxl-game-boy-printer-xl-kit/) ，它可以让 Game Boy 相机与现代打印机配合工作。



复兴 Game Boy 打印机并非不可能，这种打印机在易贝，甚至在专门销售复古硬件的视频游戏商店都很容易找到。这是一台热敏打印机，所以更换墨盒不是问题，但找到 1.5 英寸大小的热敏纸卷并不容易(切割自己的 [看起来像是一种痛苦](https://www.instructables.com/id/How-to-Make-Game-Boy-Printer-Paper/) )如果你这样做了，你经常需要拆开它们，以便将纸卷放入 Game Boy 打印机的进纸机构中。仅仅是打印出低分辨率的黑白照片，就要经历很多困难——即使你喜欢高保真的美感。

任天堂几年前就停止销售 Game Boy 相机了，但热敏打印机仍然随处可见，最常用于收银台打印纸质收据。你可以在网上找到价格低至 30 美元的的基本单元，替换热敏纸卷也同样实惠。

唯一缺少的要素是一种将游戏机连接到现代热敏打印机的方法，因为任天堂选择了主机和打印机配件之间的专有接口，这就是 Mach 的 gbpxl (也被称为游戏机打印机 xl)适配器的作用。gbpxl 是围绕 ATmega4809 微控制器构建的，最初是为了与 Epson 的热敏打印机一起工作而开发的，但 Mach 对其进行了重新编程，以兼容更广泛的打印机，假设它们仍然使用 RS232 串行接口，此时该接口已有近 60 年的历史。

对于那些熟练使用烙铁和熟悉编程微控制器的人，马赫在他的 [GitHub 页面](https://github.com/xx0x/gbpxl) 上分享了原理图和必要的代码，这样任何人都可以为自己构建一个 gbpxl 适配器的副本。对于那些能力较弱的人来说，马赫的 20 美元套件，可通过 T5】TindieT7】获得，包括 RS232 适配器和再次打印你的游戏机相机照片所需的所有电缆，但你需要自己组装。但这是一个 BYOGBC 套件，这意味着你需要提供自己的游戏机和游戏机相机。