# 如何确保您的 VPN 对其国际出口服务器诚实

> 原文：<https://lifehacker.com/how-to-make-sure-your-vpn-is-honest-about-its-internati-1760243121>

使用 VPN 的最好理由之一是绕过流媒体电影和其他内容的讨厌的位置限制，但在你付钱给一个承诺在几十个国家提供服务器的 VPN 之前，请确保他们说的是实话。信任，但要核实。



大多数 VPN 服务提供商都提供试用期，无论多短，你都可以在试用期内测试服务，如果你不喜欢，可以在你成为高级用户的第一个月内取消服务。幸运的是，这是你所需要的所有时间来确保那些他们承诺生活在澳大利亚、德国或英国的服务器确实存在，而不仅仅是代理服务器，或者更糟的是，标有“布鲁塞尔”或“开普敦”的美国 IP 地址

SlickVPN 的人最近在他们的博客 上发布了 [这个故事，提醒我们看穿 VPN 的出口服务器承诺的最简单的方法是自互联网出现以来一直由我们支配的工具:](https://www.slickvpn.com/the-truth-about-vpn-providers-and-international-locations/) [traceroute](https://en.wikipedia.org/wiki/Traceroute) 和 [ping](https://en.wikipedia.org/wiki/Ping_(networking_utility)) 。

> 如果您有技术知识，您可以执行跟踪路由/ping 来判断网关的实际位置。这个测试/实验的结果看起来像这样:
> 
> 示例假设 VPN 位于新西兰的奥克兰。如果从美国芝加哥执行到其主机名的 traceroute (tracert ):

> *在 TCP 端口 80 (http)上追踪到示例 VPN 新西兰 IP 位置(104.250.161.3)的路径，最大 30 跳*
> 
> 1.  *10.1.2.25 0.479 毫秒 0.428 毫秒 0.556 毫秒*T2】
> 2.  [【10ge-2.ge146.chi1.colocrossing.com】](http://10ge-2.ge146.chi1.colocrossing.com/)*【108.174.54.217】0.684 ms 0.633 ms 0.595 ms*
>     
> 3.  [【ae16-386.chi11.ip4.gtt.net】](http://ae16-386.chi11.ip4.gtt.net/)*【173.205.55.141】1.156 ms 1.163 ms 1.137 ms*
>     
> 4.  [【xe-9-1-0.chi11.ip4.gtt.net】](http://xe-9-1-0.chi11.ip4.gtt.net/)*【89.149.131.229】1.148 ms 1.161 ms 1.166 ms*
>     
> 5.  [【be3027.ccr41.ord03.atlas.cogentco.com】](http://be3027.ccr41.ord03.atlas.cogentco.com/)*【154.54.10.21】1.675 ms 1.621 ms 1.440 ms*
>     
> 6.  [【be2461.rcr12.b002281-5.ord03.atlas.cogentco.com】](http://be2461.rcr12.b002281-5.ord03.atlas.cogentco.com/)*【154.54.29.238】2.011 ms 2.192 ms 2.087 ms*
>     
> 7.  *38.122.181.114 1.695 毫秒 18.736 毫秒 2.145 毫秒*T2】
> 8.  *104.250.161.3【公开赛】1.565 ms 1.565 ms 1.513 ms*T2】
> 
> 从 ping 次数和 traceroute 可以明显看出，服务器位于芝加哥，而不是新西兰。在 1.5 毫秒内从芝加哥到新西兰是不可能的，因为那比光速还快。
> 
> 当您连接到 ExampleVPN 的新西兰 IP 位置并跟踪路由输出时:
> 
> *traceroute:警告:*[](http://www.google.com/)**有多个地址；使用 74.125.138.103**
> 
> **traceroute 到*[*www.google.com*](http://www.google.com/)*(74 . 125 . 138 . 103)，最大 64 跳，52 字节数据包**
> 
> 1.  **104.250.161.129(104.250.161.129)1533.225 毫秒 67.066 毫秒 61.497 毫秒*T2】*
> 2.  **23.227.197.137(23.227.197.137)60.668 毫秒 61.971 毫秒 60.919 毫秒*T2】*
> 3.  **33 . 154 . 21 . 46 . in-addr . arpa(46.21.154.33)61.250 ms 72.902 ms 69.437 ms*T2】*
> 4.  *[【ip81.208-100-42.static.steadfastdns.net】](http://ip81.208-100-42.static.steadfastdns.net/)*【208.100.42.81】69.190 ms 67.959 ms 70.124 ms** 
> 5.  *[【xe-0-0-1.core4.chi02.steadfast.net】](http://xe-0-0-1.core4.chi02.steadfast.net/)*【208.100.32.54】74.908 ms 65.975 ms 61.235m** 
> 6.  *[【eqix-ch-100g.google.com】](http://eqix-ch-100g.google.com/)*【206.223.119.21】62.341 ms 61.326 ms 60.149 ms** 
> 
> *开始的几次跳跃证实了你在芝加哥。*

*我们在本帖 中解释了 [如何使用 traceroute 和 ping，所以如果你不熟悉，不用担心，这并不难。](https://lifehacker.com/how-to-troubleshoot-a-flaky-internet-connection-5319976)*

*当然，整个故事继续强调 SlickVPN 的新西兰出口服务器实际上是如何在新西兰的*，所以这意味着让他们看起来不错。在这种情况下，没关系，因为他们对他们的服务器的位置是诚实的。**

*这是 [的另一个步骤，在你每个月给他们钱之前，确保你的 VPN 是值得信任的](https://lifehacker.com/how-do-i-know-if-my-vpn-is-trustworthy-508866499) 。在 [亚马逊网络服务](https://aws.amazon.com/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-make-sure-your-vpn-is-honest-about-its-internati-1760243121&asc_source=&tag=kinjalifehackerlink-20) 或其他 [虚拟私人服务器](https://en.wikipedia.org/wiki/Virtual_private_server) (VPS)提供商上运行一个实例太容易了，免费下载 [OpenVPN](https://openvpn.net/) ，安装它，然后称自己为 VPN 提供商。然后你可以从那些认为他们得到了一个安全的多站点 VPN 的用户那里获得每月的订阅费(通常是昂贵的),而实际上他们得到的是一个漏洞隧道，任何有时间、耐心和一点技术技能的人都可以自己完成。*

*采取这一微小的额外步骤，以及检查评论，查看 VPN 的取消和计费政策，并检查他们的日志记录和数据保留政策，对于确保您在使用 VPN 时保护您的隐私和安全以及确保您获得付费的基本服务至关重要。*

*|如何知道你的 VPN 对国际网关位置是诚实的*

**<small>图像由</small>* [*<small>素颜照片</small>*](http://www.shutterstock.com/pic.mhtml?id=127208879&src=id)*<small>(</small>*[*<small>Shutterstock</small>*](http://www.shutterstock.com/)*<small>)和</small>* [*<small>音乐人</small>*](http://www.shutterstock.com/pic-153874961/stock-vector-lock-icon.html?src=lPL0BreMtTHX71WByri8SQ-1-21) *T51】**