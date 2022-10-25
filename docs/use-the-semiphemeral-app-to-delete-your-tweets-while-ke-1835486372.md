# 使用半流行应用程序删除你的推文，同时保留你的收藏

> 原文:[https://life hacker . com/use-the-semi phermal-app-to-delete-your-tweets-while-ke-1835486372](https://lifehacker.com/use-the-semiphemeral-app-to-delete-your-tweets-while-ke-1835486372)

删除你的推文有很多很好的理由，但我一直犹豫要不要扣动扳机。虽然这个想法在纸上是有道理的，但我知道有些事情我会后悔抹去。我们之前推荐过清除你 Twitter 的服务，但据我所知，它们都是删除你的全部历史。要么全有，要么全无。

Watch

由科技记者 [米卡·李](https://twitter.com/micahflee) 制作的程序[semi phermerial](https://micahflee.com/2019/06/semiphemeral-automatically-delete-your-old-tweets-except-for-the-ones-you-want-to-keep/)，对于那些想从他们的推特账户中挑选出被大量删除的内容的人来说是完美的。当你运行它时，它可以删除你所有的推文*，除了你选择保留的推文*——这听起来很棒，但有一个小问题。要在上使用应用程序，你必须注册一个 Twitter 开发人员账户，并进入一个比按一个按钮然后屏蔽你所有的推文更复杂的程序。

不过，如果你想要删除你的推文的安全性，但在提交之前需要更多的控制，这是一个很好的方法。我们将带您了解如何设置它，这样就不会让人不知所措。

### **第 1 部分:入门所需安装的一切**

你需要访问 Twitter API 来使用 Semiphemeral，在你告诉他们你在做一个应用程序后，公司会分配给你。首先，登录 Twitter，然后进入 Twitter 开发者网站的应用部分，点击“创建应用”按钮。如果需要，按照说明注册一个免费的 Twitter 开发者账户。(如果你需要的话，Twitter 会帮你完成注册过程。)

在制作应用程序工具中，将要求您提供名称、描述、网站和回拨。名字和描述由你决定，如果你没有一个正在开发的实际应用程序，李开复在他的博客上慷慨地建议你列出他的 [GitHub](https://github.com/micahflee/semiphemeral) 页面。最后，对于网址，你要使用 app 生成的地址—[http://127 . 0 . 0 . 1:8080/](http://127.0.0.1:8080/)。一旦你把它交上来，你就会得到一些你需要在应用程序中使用的证书代码:

*   API 密钥
*   API Token
*   访问令牌密钥
*   访问令牌秘密

把这些写下来(或者复制并粘贴到文本文件中)。你以后会需要它们的。你还需要下载 [Pip](https://pypi.org/project/pip/) ，这个安装程序可以让你运行用 [Python](https://www.python.org/) 编写的程序。

### **第二部分:使用半卤素**

现在你已经有了你需要的东西，你可以从李的 [GitHub 页面](https://github.com/micahflee/semiphemeral) 下载半个。接下来，打开 Pip 并输入以下命令来安装 Semiphemeral:

`$ pip3 install semiphemeral`

你现在有两个任务:为你想要删除的推文设置参数——例如，超过两周的所有推文——然后从你想要保存的组中选择推文。

要开始清除您的 Twitter 历史记录，请在 Pip 中运行以下命令。

```
$ semiphemeral Configure
```

设置好之后，程序会生成一个本地网站——那就是[http://127 . 0 . 0 . 1:8080/](http://127.0.0.1:8080/)，我们之前说过的那个网站。在你的网络浏览器中打开它，进入半参数配置菜单。输入 Twitter API 凭证和用户名后，您将能够设置您想要保留哪种 Twitter 记录，并为清除过程编写一些广泛的例外情况——比如有很多赞和转发的推文。

在您设置例外之前，Semiphemeral 首先需要下载您的 Twitter 时间表，因此在 Pip 中运行下一个字符串。Lee n 在他的博客中提到，这可能需要很长时间，尤其是你第一次运行它的时候。耐心点。

```
$ semiphemeral Fetch
```

一旦你完成了“抓取”，你就可以手动选择要保存的推文。该列表是可搜索的，所以你不需要一条一条地浏览每条推文。一旦你选择了参数并选择了你想要保存的推文，你可以用 Pip 中的最后一行删除你的推文:

```
$ semiphemeral Delete
```

关于这个过程，你需要知道的一件事是，它不会自动重复。如果你发了更多的 tweets，你将不得不返回到 Pip 并重新运行删除命令来删除它们。如果你想变得更有趣，你可以设置 Semiphemeral 以你想要的任何间隔自动运行，但是这可能比你需要的过程更激烈。每隔几个月(或一年)运行一次删除命令，你就万事俱备了。

关于删除推文的更多信息，请看这个视频。