# 如何创建可搜索的 pdf 文档？

> 原文：<https://lifehacker.com/how-do-i-create-a-searchable-archive-of-pdfs-1831845468>

在 Lifehacker 本周的 [技术建议专栏](https://lifehacker.com/c/tech-911) 中，各位，继续提问吧！—我们正在帮助一位读者，他有太多的重要文件需要神奇地过渡到数字领域。至少，这听起来比“光学字符识别”要令人兴奋得多，因为“光学字符识别”并没有真正脱口而出。



Lifehacker 的读者菲尔写道:

> “大卫，你的专栏内容丰富，很有帮助，写得很好。谢谢你。
> 
> 我正在复印(通过扫描数字化)一份非营利组织的会议记录。该组织每月开两次会。代表一次会议的每一组会议记录，通常只有一两页打字稿，组成一个文件。我有大约 20 年的时间可以做。我会将一年会议的所有文件合并成一个“年度”文件，然后将其中的 10 个文件合并成另一个单独的“十年”文件。我知道，信息太多了。
> 
> 无论如何，我希望这些文件是可搜索的。

> 你能推荐一个免费或低价的桌面 OCR 程序或任何其他可以搜索会议记录的方法吗？我非常希望保留原始会议记录的格式。会议记录从不包含照片。我用的是 Windows 10。"

谢谢你的美言，菲尔！我很乐意帮忙——不是因为奉承，而是因为你的问题可能是很多读者(包括我自己)都想过的。我有一大堆东西想从现实世界转移到数字世界，这样我就可以把原始文件和照片遗忘。成堆的纸不能带给我快乐。

你有几个选择可以尝试。我想从一个明显的例子开始:谷歌。假设您正在创建 pdf，请将您的文件上传到 Google Drive。右键单击任何单个 PDF，将鼠标悬停在“打开方式”上，然后选择“谷歌文档”然后，Google 将尝试在您的 PDF 上运行一些 OCR，您应该能够将结果文件保存为文档。然后，您可以通过 Drive 本身搜索该文档(以及您转换的任何其他文档)。

然而，我越想越觉得，考虑到您必须处理这么多文件，这个解决方案似乎有点不优雅。相反，我可能会尝试一款软件，比如 TesseractStudio.Net 的[](https://github.com/OpaitSoftware/TesseractStudio.Nethttps://github.com/OpaitSoftware/TesseractStudio.Net)**——或者只是 [**宇宙魔方 OCR**](https://github.com/tesseract-ocr/tesseract) ，如果你不害怕命令行的话。您应该能够使用它从您的文件中创建 OCR 数据，然后您可以通过 Windows 或 macOS 直接搜索它们。[**ocrmy pdf**](https://github.com/jbarlow83/OCRmyPDF)是另一个类似于 Tesseract OCR 的选项，但是，同样，您将使用键入的命令对文件应用 OCR。没有 GUI，也没有(直接的)Windows 支持。**

**还有 [**文书**](https://openpaper.work/en-us/) ，这是一个内置 OCR 的开源文档编目工具，我肯定会考虑它，因为它被设计成一个用于归档、排序和搜索文档的一体化软件。听起来这可能正是你想要的。**

**我没有用过[**PDF-XChange Viewer**](https://www.tracker-software.com/product/pdf-xchange-viewer#features)，但是其他人都推荐它作为选项。免费版会在你的 pdf 文件中加入水印，但它可以从图像中创建 pdf 文件，如果我没猜错的话，还可以为你现有的这些*和*pdf 文件添加 OCR。这值得探索，即使它不是理想的(免费的)解决方案。同样，[**free OCR**](http://www.paperfile.net/)可以拍摄您的图像或 pdf，应用 OCR，并将结果导出为纯文本文件或 Word 文档。如果你不介意这样搜索你的档案，这是一个选择。**

**至于付费解决方案，总有[**Adobe Acrobat Pro**](https://acrobat.adobe.com/us/en/acrobat/acrobat-pro.html)或[**Foxit PhantomPDF**](https://www.foxitsoftware.com/pdf-editor/)。两者都允许您将 OCR 添加到 pdf 中，并且您应该能够大批量处理您的所有文档(或者创建一个脚本来处理一个文件夹的内容)。如果他们不限制他们的 OCR 能力，你甚至可以在应用的免费试用期间完成这一切。我还见过其他有你这种特殊问题的人使用像[**PDF OCR**](http://solutions.weblite.ca/pdfocrx/)这样的应用程序获得成功，这可能是一种更便宜的替代方法。**

**这是我能想到的所有东西(还需要一点研究)。希望这些解决方案中有一个适合你——而不会花费你一大笔钱。回信让我知道哪个应用程序最适合你！**

***<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>**

**<small></small>**