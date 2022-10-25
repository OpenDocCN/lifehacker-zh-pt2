# 当你的廉价安卓手机带有恶意软件时该怎么办

> 原文：<https://lifehacker.com/what-to-do-when-your-budget-android-phone-arrives-with-1840929271>

美国政府的 [生命线援助](https://www.fcc.gov/consumers/guides/lifeline-support-affordable-communications) 计划的前提没有错。它允许那些收入相当低的人——比联邦贫困指导线低 135%或更低，或者一个单人家庭不到 16862 美元——获得折扣或免费的电话和无线服务。



然而，当提供的一款手机预装了恶意软件时，这就成了一个大问题。至少，MalwareBytes 是这么断言的，它注意到了预装在这样一款手机上的应用程序的一些问题，这款手机是维珍移动公司[Assurance Wireless](https://www.assurancewireless.com/)销售的 Unimax U686CL。而 [下面是它发现的](https://blog.malwarebytes.com/android/2020/01/united-states-government-funded-phones-come-pre-installed-with-unremovable-malware/) :

> *“在 UMX U686CL 上发现的第一个有问题的应用程序伪装成一个名为 Wireless Update 的更新程序。是的，它能够更新移动设备。事实上，这是更新移动设备操作系统(OS)的唯一方法。相反，它也能够在未经用户同意的情况下自动安装应用程序。*
> 
> 因此，我们将该应用程序检测为 Android/PUP。Riskware.Autoins.Fota.fbcvd，对于 Android 客户来说，这是一个 Malwarebytes 应该很熟悉的检测名称。这是因为该应用程序实际上是 Adups 的变种，Adups 是一家总部位于中国的公司，被发现收集用户数据，为移动设备创建后门，是的，开发自动安装程序。"

这还不是全部。在智能手机上发现的第二个应用程序——它自己的设置应用程序——实际上是一个木马下载程序，MalwareBytes 将其归类为“Android/trojan . dropper . agent . umx”。一旦它加载，它就会在用户的手机上下载第二个恶意软件(如果我们计算的话，总共是第三个),然后让你的设备充满烦人的广告。好玩。

在一份声明中，Assurance Wireless 告诉 [ZDNet](https://www.zdnet.com/article/unremovable-malware-found-preinstalled-on-low-end-smartphone-sold-in-the-us/) 他们“意识到了这个问题，并与设备制造商 Unimax 联系以了解根本原因，但是，经过我们的初步测试，我们不认为媒体中描述的应用程序是恶意软件。”

### 有一个简单的解决方法，对吗？

最坏的消息是:在这种情况下，对于这些预先安装的问题，你真的无能为力。理论上，你可以取消无线更新应用，但是你的设备不会收到任何更新，这本身就是一个安全(和功能)问题。去掉设置，连我都不确定你的手机会怎么样。我怀疑它会变得不可操作。

Malwarebytes 确实提供了一些类似弗兰肯斯坦的解决方案，通过这些方案，你可以尝试卸载有问题的应用程序，并用一个干净的、相同版本的应用程序来替换它。这是 [很多工作](https://blog.malwarebytes.com/cybercrime/2019/01/the-new-landscape-of-preinstalled-mobile-malware-malicious-code-within/) 没有成功的保证；以至于 Malwarebytes 也承认，对付智能手机上预装恶意软件的最佳途径就是避免智能手机出现这些问题。

不过，说起来容易做起来难。如果你一直在使用 UMX U686CL，你已经被感染了。目前还不清楚你的设备上是否加载了额外的恶意软件应用程序，但我强烈建议你将关键数据上传到其他地方——要么上传到联网的计算机，要么上传到云端——并重置你的手机出厂设置。在那之后，把它归还到你购买它的地方。如果这是不可能的，回收它，买别的东西。

### 如果你再买一部经济型智能手机...

你应该再买一部廉价手机吗？你当然可以；然而，Malwarebytes 指出，它已经看到最近越来越多的廉价 android 设备预装了恶意软件。我 t 只需要 [快速搜索两个](https://gizmodo.com/a-new-reason-to-not-buy-these-cheap-android-devices-co-1826289219) 就能找到更多关于这种做法的报道。

如果你选择另一个，你应该安装 Malwarebytes 的 [安卓应用](https://play.google.com/store/apps/details?id=org.malwarebytes.antimalware&referrer=af_tranid%3D13r8khvPDPycyJwDlSF4kQ%26shortlink%3D516cebeb%26pid%3DIRIS%26c%3DIRIS-free-download-Oct-18%26af_web_id%3Dadf088c1-ec8d-4ce5-86b5-7bdb4049af41-o) ，看看它是否能找到什么——不要购买高级包，如果你试图根除预装的问题，这是不必要的。否则，我建议为你的智能手机型号设置一个 [谷歌一个 lert](https://www.google.com/alerts) (比如“UMX U686CL”)，这样你就可以在别人发现你的设备有问题时得到快速通知。

和往常一样，如果你注意到手机上有可疑的东西——以前不存在的奇怪命名的应用程序，不知从哪里冒出来的新广告，诸如此类的事情——很可能你手上有恶意软件问题。你可能想要做一些额外的调查，抑制向你的设备提供更多个人数据(如你的社会安全号码或信用卡信息)的冲动，并可能开始购买另一部智能手机。