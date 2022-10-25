# 如何使用英特尔全新的一键式实用程序对您的系统进行超频

> 原文：<https://lifehacker.com/how-to-overclock-your-system-with-intels-new-one-button-1835656310>

**Windows:** 英特尔让你的 CPU 超频变得容易多了——把它推到超过它的默认时钟速度，让它甚至更快，冒着潜在烧焦你的芯片的风险。只有一个大警告:你将需要六个受支持的第九代 CPU 中的一个(都在 Coffee Lake 家族中)才能享受其新的简单的超频实用程序。你还需要在你的一个驱动器上有 16GB 的空闲空间，但我怀疑这对大多数寻求超频系统的系统构建者来说是个问题。



首先说一下 CPU。不要安装(仅限 Windows)[**英特尔性能最大化器**](https://www.intel.com/content/www/us/en/products/docs/processors/core/performance-maximizer.html) ，除非您正处于以下状态之一:

*   酷睿 i9-9900K
*   酷睿 i9-9900KF
*   酷睿 i7-9700K
*   酷睿 i7-9700KF
*   酷睿 i5-9600K
*   酷睿 i5-9600KF

如果你不知道你的系统里有什么，首先，超频 T2 可能不适合你。假设你是健忘的，你可以随时打开 Windows 控制面板的系统部分，它会告诉你你到底在用什么 CPU:

如果你在想，“哦，我不认为英特尔检查这些东西；我可能可以在任何旧的 CPU 上使用这个应用程序，”你就错了。本着“生活黑客”的精神，我尝试了完全相同的方法，但甚至无法完成应用程序的安装:

一旦你进入，性能最大化应用程序会让你知道超频是一件严肃的事情。如果你(或实用程序)搞砸了什么，它可能会伤害或破坏你的 CPU。(英特尔还提供了一个链接，链接到它的 [性能调整保护计划](https://click.intel.com/tuningplan/) ，这是一个 20 美元的第九代处理器标准保修升级，如果你的超频出现问题，它可以让你用坏的 CPU 换一个工作的 CPU。)

在你选择了你想让实用程序消耗 16GB 的保留空间来发挥它的魔力之后，它会“在你的系统上运行一些测试来定制你的超频。”根据该实用程序，在此过程中，您可能要进行“几个小时”的测试，并且系统会多次重启。

此外，如果您在主板的 BIOS 中定制了任何与性能相关的设置，如果您已经在 BIOS 中启用了某种自动超频功能，或者如果您使用了其他超频应用程序来调整 CPU 的频率，整个过程可能不会工作(或者您可能不会获得您希望的超频)。(使用该应用程序的其他 BIOS 要求可以在英特尔的 [用户指南](https://downloadmirror.intel.com/28772/eng/Intel(R)_Performance_Maximizer_1.0.1_User_Guide.pdf) 中找到。)

Wccftech 的基思·梅(Keith May)指出，当实用程序完成时——这个过程需要相当长的时间——你的结果可能不会像最初看起来那样令人惊叹。例如，当 May 运行该实用程序时，它将他的 Core i9-9900K 处理器从 4.7GHz(全核，turbo)超频到 5.10GHz，增加了 8.5%。这听起来可能不多，但在超频世界中这是一个相当不错的提升(特别是如果你不需要自己摆弄任何设置的话)。

问题？正如 May 所描述的，他的系统可能已经达到了 5.1GHz，但并没有保持很长时间:

<iframe data-src="https://lifehacker.com/embed/inset/iframe?id=youtube-video-MarU1t5R4mU&amp;start=350" data-chomp-id="MarU1t5R4mU" data-recommend-id="youtube://MarU1t5R4mU" id="youtube-MarU1t5R4mU" data-recommended="false" width="800" height="450" class="core-inset lazyload" frameborder="0" scrolling="no" allowfullscreen="" webkitallowfullscreen="webkitAllowFullScreen" mozallowfullscreen="mozallowfullscreen"><span data-chomp-id="MarU1t5R4mU" data-recommend-id="youtube://MarU1t5R4mU" id="youtube-MarU1t5R4mU" data-recommended="false" class="js_recommend"/></span></div><p class="sc-77igqf-0 bOfvBY">虽然他在他的<span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://www.maxon.net/en/products/cinebench-r20-overview/&quot;,{&quot;metric25&quot;:1}]]" href="https://www.maxon.net/en/products/cinebench-r20-overview/" target="_blank" rel="noopener noreferrer"> Cinebench </a> </span>基准测试中看到了一些轻微的性能提升，但英特尔超频也将他最热的测量核心的温度提高了 10 摄氏度。同样，这些都是超频的预期结果，但 May 听起来对最终结果并不太兴奋:他的芯片平均增加了约 100 MHz 的全核心。</p><p class="sc-77igqf-0 bOfvBY">“也许你的里程会比我多，一开始我真的很兴奋——我想，伙计，5.1 英里。那很酷。我只把这个东西推到了 5 千兆赫，”梅说。</p><p class="sc-77igqf-0 bOfvBY">我们的建议？和往常一样，如果你想超频你的系统，就拿一些<span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;Internal link&quot;,&quot;https://lifehacker.com/how-to-create-a-portable-version-of-cinebench-r20-1833201374&quot;,{&quot;metric25&quot;:1}]]" href="https://lifehacker.com/how-to-create-a-portable-version-of-cinebench-r20-1833201374">前后基准</a> </span>来看看额外的损耗是否值得。使用<span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://www.hwinfo.com/download/&quot;,{&quot;metric25&quot;:1}]]" href="https://www.hwinfo.com/download/" target="_blank" rel="noopener noreferrer"> <strong> HWiNFO </strong> </a> </span>等实用程序来了解系统运行前后的情况(电压、时钟速度和温度)，这样您就可以更好地了解英特尔的实用程序对您的帮助有多大。</p><p class="sc-77igqf-0 bOfvBY">如果你手动超频，你可能会看到最好的结果，但这不是每个人都愿意做的事情。英特尔的工具很简单，即使它可能不会将您的系统推向巅峰。确保你做了一些调查，看看是否值得。</p> </body> </html></iframe>