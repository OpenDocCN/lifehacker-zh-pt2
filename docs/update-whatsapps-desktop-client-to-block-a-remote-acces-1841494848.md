# 更新 WhatsApp 的桌面客户端以阻止远程访问漏洞

> 原文：<https://lifehacker.com/update-whatsapps-desktop-client-to-block-a-remote-acces-1841494848>

WhatsApp 通常被认为是一个安全的消息应用程序，但尽管你的消息可能会被安全加密，但该服务的应用程序和其他任何应用程序一样容易出现安全漏洞。最新的 WhatsApp bug 是个大问题。

Watch

安全研究员 [加尔·魏茨曼](https://www.perimeterx.com/tech-blog/2020/whatsapp-fs-read-vuln-disclosure/) 最近在 WhatsApp 的桌面版本中发现了一个重大漏洞，黑客可以通过看似正常的消息发送代码片段来安装恶意软件，查看你的消息，甚至远程访问存储在你电脑上的文件。据发现该漏洞的研究人员称，它似乎已经被黑客利用了。

为了让攻击生效，你必须先阅读一条恶意消息，所以你很可能是安全的，除非你接受并打开随机用户的对话请求。虽然 WhatsApp 在 12 月份通过补丁修复了这个问题，但你需要确保你运行的是最新版本的桌面客户端(尤其是如果你有一段时间没有使用 WhatsApp 的话)。该漏洞影响 WhatsApp 桌面版本 0.3.9309 及更早版本；你可以在这里 下载 WhatsApp Desktop for Windows 和 Mac [的更新版本。](https://www.whatsapp.com/download)

那么，到底是什么导致了如此巨大的漏洞，又是如何被忽视的呢？ [Ars Technica 关于漏洞](https://arstechnica.com/information-technology/2020/02/flaws-in-whatsapps-desktop-app-allowed-remote-access-to-files/) 的报告指出，该漏洞是由于脸书用于 WhatsApp 桌面客户端的电子应用框架中的缺陷造成的，该框架允许在多个平台之间同时进行更容易的开发和推广。

你可以在 Ars Technica 的文章中获得完整的细节，但电子框架使用过时的 Chromium 浏览器代码，存在明显的安全问题，使黑客能够通过 WhatsApp 消息发送和执行恶意代码。Chromium 不久前修补了这些问题，但它们仍然存在于电子版——因此也存在于桌面版 WhatsApp 客户端——直到这个错误在本周最终被发现。所以，再次提醒你，更新你的客户端，永远不要在任何消息应用中打开随机消息。