# 为什么网速测试会报告不同的结果？

> 原文:[https://life hacker . com/why-do-internet-speed-tests-report-different-results-1834814879](https://lifehacker.com/why-do-internet-speed-tests-report-different-results-1834814879)

我道歉。上周在 [**Tech 911**](https://lifehacker.com/c/tech-911) ，Lifehacker 的技术-建议专栏，我接受了 Lifehacker 编辑-in-Chief[Melissa](https://lifehacker.com/im-melissa-kirsch-lifehacker-editor-in-chief-and-this-1829150849)的提问。严格来说，她是 Lifehacker 的读者，所以这仍然符合本专栏的主题，但感觉像是作弊。这周我又在做同样的事情，不是因为你没有提交有价值的问题，而是你提交了！—只是另一个 Lifehacker 的员工有一个关于 [的很好的问题，这是我们最近探讨的一个话题](https://lifehacker.com/top-10-ways-to-deal-with-a-slow-internet-connection-514138634) ，我打赌你们中的一些人会有类似的想法。

Watch

Lifehacker 社交媒体编辑 Tim 写道:

> “网速测试到底是怎么回事，为什么我在不同的测试中得到完全不同的结果？！？!"

我进一步研究了这个问题，结果发现 Tim 在他的家庭连接上运行各种基于网络的速度测试时，看到了相当多不同的数字。一号。178.4 Mbps——不算太寒酸。另一边呢？187.仍然做得很好。然而，在第三种情况下，我们遇到了一个奇怪的问题:22.7 Mbps，这看起来像一场灾难。这也可能是为了转移注意力，让一个人陷入一场他们可能根本不需要的故障诊断风暴中。

首先，所有的速度测试网站计算统计数据的方式都略有不同，比如你的下载/上传速度，但是基本原理是非常相似的。例如，下面是 Speedtest.net[如何描述它的过程](https://support.speedtest.net/hc/en-us/articles/203845400-How-does-the-test-itself-work-How-is-the-result-calculated) 。

为了测量延迟，该网站会查看一条消息从您那里返回到服务器，再返回给您所用的时间，并一遍又一遍地重复这一过程，最低的值就是您的延迟结果。对于下载和上传，Speedtest 测量处理多个数据块需要多长时间，同时在整个测试过程中努力让管道充满数据(就像这样)。

这里的 [为 fast.com](https://medium.com/netflix-techblog/building-fast-com-4857fe0f8adb)为网飞的做法:

> *“根据网络吞吐量，fast.com 客户端使用可变数量的并行连接运行测试。对于低吞吐量网络，运行更多的连接可能会导致每个连接争用非常有限的带宽，从而导致更多的超时，并导致测试时间更长、准确度更低。*
> 
> 然而，当带宽足够高时，运行更多的并行连接有助于更快地使网络链路饱和，并减少测试时间。对于非常高吞吐量的连接，尤其是在延迟较高的情况下，一个连接和一个 25MB 的文件可能不足以达到最大速度，因此需要多个连接。
> 
> 对于每个连接，fast.com 客户端选择它想要下载的 25MB 文件块的大小。在网络层支持定期进度事件的情况下，请求整个文件并使用下载进度计数器估计网络速度是有意义的。在下载进度事件不可用的情况下，客户端将在测试期间逐渐增加有效负载大小，以执行多次下载并获得足够数量的样本。"

即使这对你来说听起来像一堆网络官样文章，那也没关系。关键是你应该科学地对待吞吐量测试，因为除了测试的固有差异之外，还有很多变量会影响典型的互联网速度测试。

也许你有一个到 [的人为的慢速连接，不管测试使用的是什么服务器](http://www.dslreports.com/faq/17927) 或者测试出错了。您的 ISP 可能会优先考虑或限制您的性能，这取决于测试的操作方式。甚至你的浏览器，挤满了插件和扩展，可能会以某种方式干扰一个特定的测试。或者你在不同的时间运行测试，将“差”的互联网连接误解为实际上是由于你邻居中的其他人同时传输网飞而造成的网络拥塞——诸如此类。

不要让我开始在无线连接的设备上运行这些测试。如果可能的话，使用有线连接来消除变量(如果你只是想知道你的房子或公寓是否真的获得了你所支付的速度)。将无线网络添加到组合中会使故障诊断变得相当困难，因为您必须 [运行更多测试](https://lifehacker.com/top-10-ways-to-deal-with-a-slow-internet-connection-514138634) 来将问题隔离到您的 ISP、路由器或设备。

### 像对待科学项目一样对待网速测试

你不想依赖一个服务的测试结果，即使它们看起来很棒。你应该从多个供应商那里进行多项测试，看看你是否能感觉到趋势。你的速度比你支付的速度平均慢 75%吗？有一个问题。

是否有一两个测试报告速度一般，但其他所有网站都是 blazin？你可能做得很好，特别是如果你没有注意到日常使用中的任何重大问题。

你在 yoru 光纤连接上获得千兆下载有困难吗？也许你的笔记本电脑——带有机械硬盘和低内存——无法处理大量数据，这影响了测试结果(到 [大大简化了过程](https://www.reddit.com/r/explainlikeimfive/comments/3wd9qg/eli5_how_can_internet_download_speeds_be_faster/) )。

当我想对自己的网速有一个很好的感觉时，我会进行各种测试，看看事情进展如何，然后才会有压力。该列表包括:

*   Fast.com
*   Speedtest.net
*   [speedof . me](https://speedof.me/)T3】
*   [DSLReports](http://www.dslreports.com/speedtest)
*   testmy.net
*   [M-Lab 无损检测](https://www.measurementlab.net/tests/ndt/)
*   [谷歌光纤速度测试](http://speedtest.googlefiber.net/)

这听起来很多，但是这些测试运行起来都很简单——你按下一个按钮，让它突突作响，然后你去做另一个。很简单。

如果有一两个测试失败了，没什么大不了的。如果我不能在任何一台*电脑上获得我期望的速度，我就会考虑我有多想 [拆掉房子的网络设置](https://lifehacker.com/1827249884) (或者我的桌面系统)，因为我没有获得我和我的室友应该享受的 100+ Mbps 的速度。欢乐时光！*

* * *

*<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找关于应用程序、浏览器扩展或实用程序的建议来完成特定任务？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>

<small></small>