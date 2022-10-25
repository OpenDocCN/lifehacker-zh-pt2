# 如何启用经典的 Mac 启动提示音

> 原文：<https://lifehacker.com/how-to-enable-the-classic-mac-startup-chime-1842026959>

*Donnnnnng。*经典的 Mac 提示音是让你知道你的 Mac 在关机或重启后正在重新启动的一种很好的方式。但如果我是对的，这种友好的声音已经在大多数新的苹果电脑中消失多年了。(我只有一台 MacBook Pro，我可以确认，从我记事起，启动我的 MacBook 就一直很无聊，很安静。)

Watch

如果你错过了经典的 Mac 启动声音——啊，怀旧——你可以在比你的 Mac 启动时间更短的时间内恢复它。我没有在任何其他 Mac 上测试过这个技巧，我相信只有当你的 Mac 内部有一个或芯片时，它才会起作用。然而，这是一个如此短暂的过程，不管怎样，试一试也无妨。

要开始，拉起你的**终端**。一旦载入，输入如下:

`sudo nvram StartupMute=%00`

按下回车键，输入 Mac 的密码，取消静音或将 Mac 的音量调到合理的水平，然后重启笔记本电脑或台式机。当你的系统启动时，你应该会听到熟悉的声音。如果没有，你就不走运了。

<iframe data-src="https://lifehacker.com/embed/inset/iframe?id=youtube-video-fvxOIv7SVPo&amp;start=0" data-chomp-id="fvxOIv7SVPo" data-recommend-id="youtube://fvxOIv7SVPo" id="youtube-fvxOIv7SVPo" data-recommended="false" width="800" height="450" class="core-inset lazyload" frameborder="0" scrolling="no" allowfullscreen="" webkitallowfullscreen="webkitAllowFullScreen" mozallowfullscreen="mozallowfullscreen"><span data-chomp-id="fvxOIv7SVPo" data-recommend-id="youtube://fvxOIv7SVPo" id="youtube-fvxOIv7SVPo" data-recommended="false" class="js_recommend"/></span></div><p class="sc-77igqf-0 bOfvBY">如果你厌倦了启动声音，你可以简单地<span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://support.apple.com/en-us/HT204063&quot;,{&quot;metric25&quot;:1}]]" href="https://support.apple.com/en-us/HT204063" target="_blank" rel="noopener noreferrer">重置你的 PRAM </a> </span>禁用它<em>或</em>回到终端并输入以下内容:</p><p class="sc-77igqf-0 bOfvBY"><code>sudo nvram StartupMute=%01</code></p><p class="sc-77igqf-0 bOfvBY">[ <span> <a class="sc-1out364-0 hMndXN sc-145m8ut-0 fBlGIv js_link" data-ga="[[&quot;Embedded Url&quot;,&quot;External link&quot;,&quot;https://mrmacintosh.com/how-to-enable-the-mac-startup-chime-on-your-2016-macbook-pro/&quot;,{&quot;metric25&quot;:1}]]" href="https://mrmacintosh.com/how-to-enable-the-mac-startup-chime-on-your-2016-macbook-pro/" target="_blank" rel="noopener noreferrer">麦金塔先生</a> </span></p> </body> </html></iframe>