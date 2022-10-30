# 通过调整路由器来防止 DNS 重新绑定攻击

> 原文：<https://lifehacker.com/prevent-dns-rebinding-attacks-by-adjusting-your-router-1827022291>

程序员 [艺术家](https://brannondorsey.com/) ) Brannon Dorsey 写了一篇关于前几天 [DNS 重新绑定](https://medium.com/@brannondorsey/attacking-private-networks-from-the-internet-with-dns-rebinding-ea7098a2d325) 的危险的有趣且相当技术性的文章。如果你对网络浏览器如何阻止一个网站(比如说一个诈骗网站)向另一个网站(你的银行)发送请求、清空你的账户或操纵你的凭证(没有网站的明确许可)有一丁点兴趣，这本书就值得一读。

Watch

他的研究主要集中在 [DNS 重新绑定](https://www.wired.com/story/chromecast-roku-sonos-dns-rebinding-vulnerability/) 如何让恶意网站(或其背后的人)篡改设备，如你的 Google Home、Roku、智能恒温器或路由器等。至于后果，你可能要面对的不仅仅是一个网站强迫你的智能音箱播放 [the trololo song](https://www.youtube.com/watch?v=GGgLG2kxFD4) :

> 到目前为止，我发现无线恒温器 CT50 & CT80 设备具有最严重的物联网设备漏洞。这些设备是目前市场上最便宜的“智能”恒温器。CVE 2013–4860 报告称，这款设备没有任何形式的身份验证，可以被网络上的任何人控制，在得知他们缺乏安全性后，我买了一台来玩。[...]
> 
> 这个假设被证明是正确的，恒温器的控制 API 为 DNS 重新绑定的诡计大开方便之门。如果你的建筑的恒温器能被远程攻击者控制，这种损害可能是相当明显的。位于[*http://rebind . network*](http://rebind.network)*的 PoC 在将目标温度设置为 95°f 之前，从恒温器中过滤一些基本信息。在夏季的几个月中，该温度对于老年人或残疾人来说可能是危险的，甚至是致命的。更不用说，如果你的设备在度假时成为攻击目标，你回家时可能会收到一大笔水电费。*

虽然许多主要的设备制造商 Dorsey 在防止 DNS 重新绑定攻击的路上进行了某种修补或更新，但您现在也应该采取一些措施来锁定您(可能)不太安全的无线路由器。正如 Dorsey 所说:“我应该提到的是，到目前为止，我基本上没有将我的 DNS 重新绑定研究应用到路由器上...主要是因为我几乎不敢看😨."

### 更改路由器上的这些设置以增强安全性

如果你的路由器带有任何一种基于网络的用户界面的默认登录信息(T1)——如果你有一个用智能手机或平板电脑上的应用程序设置的更好的网状路由器，情况可能就不一样了——这是你现在想要改变的事情。你应该已经把它换掉了，因为没有什么比拥有一台和*公司生产的其他设备共用一个登录名和密码的设备更不安全的了。*

如果您在登录路由器设置(基于网络或应用程序)时输入了“admin”和“admin”作为您的用户名和密码，或者类似的通用设置，请立即更改这两个设置。让它们变得独一无二，比如“Routermaster81”和“password123jk”什么的。

现在你在路由器的设置菜单中，寻找一个处理 UPnP 的部分——这可能很容易在路由器的主设置菜单中标记出来，或者它可能是隐藏在某个高级设置菜单中的一个选项。如果它存在的话，做一些挖掘(或查阅你的路由器手册)来找出它在哪里。一旦你找到它，**考虑关闭 UPnP】。正如多尔西写道:**

> *“这些 UPnP 服务器通过 HTTP 为网络上任何未经认证的机器提供类似管理员的路由器配置控制。通过 DNS 重新绑定，网络上或公共互联网上的任何机器都可以使用 IGD/UPnP 来配置路由器的 DNS 服务器，添加&删除 NAT 和 WAN 端口映射，查看网络上发送/接收的字节数，并访问路由器的公共 IP 地址(查看*[*【upnp-hacks.org*](http://www.upnp-hacks.org/upnp.html)*了解更多信息)。”*

您使用的某些软件(如游戏服务或 BitTorrent 客户端)可能需要您手动转发路由器上的端口，以便它们有效工作。如果您是其中一个的重度用户，您可能不想为了方便而牺牲安全性。如果你只是用笔记本电脑浏览网页和与朋友聊天，你可能不需要启用 UPnP。更糟糕的是，如果你发现它的缺失给你(或你最喜欢的应用)带来了很多痛苦，你可以随时重新启用它。

多尔西还建议**将你路由器的 DNS 切换到 OpenDNS** 之类的服务，而不是使用你的 ISP 的 DNS，因为你可以使用 [OpenDNS](https://lifehacker.com/speed-up-your-web-browsing-in-a-few-clicks-a-brief-int-5848823) 从 DNS 响应中过滤掉可疑的 IP 地址。

假设您已经完成了开设(免费)OpenDNS 帐户的过程， [设置您的路由器以使用它](https://support.opendns.com/hc/en-us/sections/206253627) ，并且已经安装了 OpenDNS 软件(对于 [Windows](https://www.opendns.com/download/windows) 或 [macOS](https://www.opendns.com/download/mac) )，您将想要访问 OpenDNS’[设置页面](https://dashboard.opendns.com/settings/) 并点击您网络的 IP 地址。在那里，点击左侧边栏上的“安全”,确保选中“阻止内部 IP 地址”。选中“应用到我的所有网络”并单击“应用”按钮。

一旦你完成了所有这些，看看多尔西创建的网站[，它可以帮助你判断你的联网“智能”设备是否仍然易受攻击。](http://rebind.network/)