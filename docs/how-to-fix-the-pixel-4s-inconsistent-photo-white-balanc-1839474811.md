# 如何“修复”Pixel 4 的照片白平衡不一致的错误

> 原文：<https://lifehacker.com/how-to-fix-the-pixel-4s-inconsistent-photo-white-balanc-1839474811>

Pixel 4 和 4 XL 拥有任何智能手机上最好的相机硬件，但“最好”并不一定意味着“完美”正如 [Android Police](https://www.androidpolice.com/2019/10/28/pixel-4-white-balance-bad-images/) 、Reddit 海报和谷歌支持用户所报告的，Pixel 4 的白平衡算法似乎导致了一个奇怪的色彩校正错误。Pixel 3 用户过去也出现过类似的问题，但这是一个非常罕见的问题，似乎只影响夜间模式下拍摄的照片。另一方面，在谷歌相机应用程序的各种相机模式下拍摄时，甚至在使用替代应用程序时，Pixel 4 白平衡错误都会发生。

Watch

没错:即使更换不同的应用程序也无法解决白平衡问题，因为这个问题是由操作系统级软件引起的，而不是相机硬件或应用程序本身。虽然这意味着谷歌表面上可以通过未来的 Android 更新来解决这种奇怪的行为，但尽管有 [用户投诉](https://support.google.com/pixelphone/thread/16921343?hl=en) ，但没有迹象表明这种行为会很快出现。

然而，Reddit 用户已经 [发现了一个潜在的修复方法](https://www.reddit.com/r/GooglePixel/comments/dmpv8i/anyone_with_color_hue_lights_and_a_pixel_4_xl/) ，用于修复受 Pixel 4 白平衡计算错误影响的照片。

似乎通过导出 RAW 照片文件(本质上是您的相机在拍摄照片时创建的未动图像数据)，然后将其转换为不同的文件类型，您可以绕过像素的白平衡校正，这可能会产生更准确的颜色数据。一些用户报告说原始图像颗粒更大，缺乏清晰度，这是有道理的，因为他们没有经过 Pixel 4 的各种后期处理放大，但这是目前唯一真正的解决方案。

### 如何导出和转换保存在 Pixel 4 上的原始照片

为了从您的 Pixel 4 或 4 XL(或任何其他 Pixel 设备)导出原始照片，您首先需要在 stock Pixel 相机应用程序中启用原始拍摄。

1.  打开应用程序，滑动到中心菜单的最右侧，然后点击**“更多”>“高级”**
2.  向下滚动并启用**“RAW+JPEG 控制”**
3.  点击**“查看原始文件夹”**查看手机上保存的所有原始文件。
4.  虽然你可以通过这种方式查看原始照片，但你需要在支持原始照片的照片编辑应用程序中打开它们，如 [谷歌的 Snapseed](https://play.google.com/store/apps/details?id=com.niksoftware.snapseed&hl=en_US) ，然后将它们导出为更适合网络或共享的格式，如 JPEG——这可能是在社交媒体上发布或在文本或电子邮件中附加它们的最佳选择。

您还可以在 PC 上将 RAW 文件转换为其他照片格式。你需要通过 USB 或使用云驱动服务将文件从手机传输到 PC，然后使用 Photoshop、Lightroom 或这些免费开源软件之一的编辑/导出它们。