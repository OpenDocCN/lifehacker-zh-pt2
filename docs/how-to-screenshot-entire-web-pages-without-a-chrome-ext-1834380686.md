# 如何在没有 Chrome 扩展的情况下截屏整个网页

> 原文:[https://life hacker . com/how-to-screen-whole-web-pages-without-a-chrome-ext-1834380686](https://lifehacker.com/how-to-screenshot-entire-web-pages-without-a-chrome-ext-1834380686)

无论你是在 [Windows](https://support.office.com/en-us/article/copy-the-window-or-screen-contents-98c41969-51e5-45e1-be36-fb9381b32bb7?ocmsassetID=HP001038284&CorrelationId=74acf2a3-0c32-44e1-9463-746b15eab356&ui=en-US&rs=en-US&ad=US) (点击键盘上的打印屏幕按钮)还是[Mac](https://support.apple.com/en-us/HT201361)(Shift-Command-5)，捕捉屏幕截图都很容易。虽然你可以使用各种键盘命令或屏幕选项将活动窗口隔离开来，这样可以更容易地拍摄你正在做的事情，但如果你试图拍摄整个网站的照片，这仍然不是理想的——当然，不是你屏幕上的任何内容。

Watch

承诺为你拍摄整页截图的浏览器扩展并不缺乏，其中一些相当不错(假设你在使用它们时没有任何疯狂的渲染问题)。然而，你并不真的需要一个扩展来截图一个网页。我们已经在 Firefox 中介绍过如何做到这一点，现在轮到 Chrome 了。

首先，快速向开发者[Max bck](http://Max Böck)脱帽致敬，这也是我偶然发现这个方法的地方。首先，你可以通过键盘上的 F12 键(Windows)或 Command+Option+i 键(Mac)打开 Chrome 的开发者工具。然后，点击平板电脑前看起来像智能手机的小图标，进入设备模式:

下面是它对您在浏览器中查看的页面的影响:

### 以前

### 在...之后

然后，您需要确保选择了“响应式”预设——默认情况下，当我这样做时。然后，单击同一工具栏最右边的三点图标(就在您之前单击的设备模式按钮的左边一点)。您需要选择“添加设备像素比率”选项，然后在出现的栏中将该比率(DPR)从默认的 2 更改为 3。

从那里，你所要做的就是按下 Control/Command+Shift+P，然后输入“捕捉全尺寸截图”选择那个选项，Chrome 会自动创建一个可爱的。PNG 的网页，并把它放在您的下载文件夹。

如果您想要调整屏幕截图的外观，请随意调整尺寸，方法是输入您自己的高度和宽度(以像素为单位),或者将鼠标悬停在设备模式选项下方的灰色栏上来浏览可用的预设。

我倾向于使用“笔记本电脑”模式，将屏幕宽度设置在令人愉快的 1440 像素——这有利于我试图存档的网站的截图。