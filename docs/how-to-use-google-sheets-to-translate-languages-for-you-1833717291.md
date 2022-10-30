# 如何用 Google Sheets 翻译语言

> 原文：<https://lifehacker.com/how-to-use-google-sheets-to-translate-languages-for-you-1833717291>

有比手持字典更有效的方法来记录重要的外语词汇。如果你正在学习一门新语言或进行基本的翻译，尝试使用 Google Sheets 中的 Google Translate 公式，轻松获取你知道或想知道的内容列表。



这个 [方法是由 r/LifeHacks 上的](https://www.reddit.com/r/lifehacks/comments/b81zqh/using_google_sheets_to_translate_batches_of_words/) [u/mk4rim](https://www.reddit.com/user/mk4rim) 发布到 Reddit 上的 ，但原始信息实际上来自科技作家兼教育家杰克·米勒。米勒在 2018 年分享了这个视频，但它在 Reddit 上获得了新的生命。当时，他制作了这个视频，展示了插入到谷歌工作表中的基本公式，这些公式将你的电子表格连接到谷歌翻译:

 [https://lifehacker.com/embed/inset/iframe?id=twitter-998716364339675137&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-998716364339675137&autosize=1) 

在一篇关于主题 的文章中，米勒写道:

> 在一个单元格中输入一种语言的单词，然后在另一个单元格中使用公式 *=GoogleTranslate(text，source_language，target_language)* 进行自动逻辑翻译！您甚至可以向下拖动公式单元格底部的*填充柄*，将该公式应用于多个单元格。
> 
> 这个公式似乎适用于谷歌翻译支持的所有语言，其中有 100 多种！它甚至用正确的字母和字母表输出结果——不仅仅是我们的 *ABC* 英文字母。你只需要知道这种语言的两个字母的代码，你可以在 [这个列表](https://www.loc.gov/standards/iso639-2/php/code_list.php) 中找到。

为此，你需要学习一些基本的代码。在一个共享屏幕上观看米勒浏览它会有所帮助，但如果你没有抓住它，还有一个链接到 Reddit 帖子的 u/ [bar10005](https://www.reddit.com/user/bar10005) 的 [支持文档](https://support.google.com/docs/answer/3093331) :

> 示例用法
> 
> Google translate(“Hello World”、“en”、“es”)
> 
> 谷歌翻译(A2，B2，C2)
> 
> 谷歌翻译(A2)
> 
> 句法
> 
> GOOGLETRANSLATE(文本，[源语言，目标语言])
> 
> 文本-要翻译的文本。文本值必须用引号括起来，或者是对包含适当文本的单元格的引用。
> 
> source_language - **[** 可选-默认为“自动” **]** -源语言的双字母语言代码，例如“en”代表英语，“ko”代表韩语，或“auto”代表自动检测语言。如果省略 source_language，也必须省略 target_language。
> 
> target_language - **[** 可选-默认为系统语言 **]** -目标语言的两个字母的语言代码，如英语的“en”或日语的“ja”。

人们可能如何使用这一功能各不相同；许多人可能只是想把它作为笔记本电脑上的学习辅助工具，但如果你在旅途中使用它，你可以为你的手机下载谷歌工作表应用程序 。如果你作为一名游客遇到新单词，这将使你能够检查和编辑。

电子表格翻译在语言学习过程中是一个很好的补充，但一旦你进入短语和口语的领域，它就很有限。例如，u/ [danielks_13](https://www.reddit.com/user/danielks_13) 指出某些概念不能逐字翻译:

> Bienvenido 不翻译成不客气，更像是欢迎。用西班牙语说不客气的恰当方式是“不客气”。

一定要检查那些比“汉堡包”更复杂的词汇否则，这是一个跟踪你的进步和囤积所有那些新名词的简单方法。