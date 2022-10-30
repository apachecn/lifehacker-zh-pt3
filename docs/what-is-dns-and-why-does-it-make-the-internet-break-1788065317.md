# 什么是 DNS，为什么会让互联网断网？

> 原文：<https://gizmodo.com/what-is-dns-and-why-does-it-make-the-internet-break-1788065317>

今天， [美国一半的互联网关闭了](http://gizmodo.com/this-is-probably-why-half-the-internet-shut-down-today-1788062835) ，当时黑客对主要 DNS 主机 Dyn 的 [服务器发动了大规模分布式拒绝服务(DDoS)攻击。目前还不清楚到底是谁实施了这次攻击，以及为什么，但不管怎样，这次事件证明了如果受到坚定的黑客攻击，大面积的网络可以多么容易地被清除。](https://www.dynstatus.com/incidents/nlr4yrr162t8) 

Watch

在大修之后，Dyn [发布了此声明](https://www.dynstatus.com/incidents/nlr4yrr162t8) :

> 从 2016 年 10 月 21 日 11:10 UTC 开始，我们开始监控和缓解针对 Dyn 托管 DNS 基础设施的 DDoS 攻击。在此期间，一些客户可能会经历 DNS 查询延迟和延迟的区域传播。一旦有新的信息，我们会及时发布。

要知道像 Twitter、Spotify、Reddit、Etsy、Wired、PayPal 这样的主要网站都有可能在瞬间被下线，这是很恐怖的。除了 DDoS 细节之外，黑客使用的确切过程目前还不得而知，但这对每个互联网用户来说都很重要，因为它与互联网的具体工作方式有关。考虑到这一点，以下是一些世界上最受欢迎的网站如何在瞬间离线。

* * *

### 技术是什么？

域名服务器(DNS)充当互联网的电话簿，方便对特定网页的请求。它们可以确保你每次在浏览器中输入网站时都在正确的位置。黑客偶尔会攻击 DNS 提供商，以关闭他们所服务的网站。今天，这恰好是 Twitter，Reddit，PayPal 和更多。

这是一个非常基本的概述。但是如果你真的想在更深层次上理解 DNS 是如何工作的，你必须遵循完整的操作顺序。一个典型的互联网用户从通过地下电缆连接的大型网络中的一台计算机开始(比如你的笔记本电脑)。这些网络上的单个节点通过称为 IP 地址的数字来相互联系。DNS 用于将 URL 等请求转换为 IP 地址。

当你输入一个网址——比如[【www.Gizmodo.com】](http://www.gizmodo.com/#_ga=1.2176624.1573483110.1468589968)——你的浏览器开始试图通过查验一系列服务器来找出那个网站在哪里。它非常详细，我们不会用完整的事件链来烦你。还有 [解析域名服务器](https://www.dnsknowledge.com/whatis/resolving-name-server/) [s](https://www.dnsknowledge.com/whatis/resolving-name-server/) ， [权威域名服务器](https://www.dnsknowledge.com/whatis/authoritative-name-server/) ， [域名注册商](https://en.wikipedia.org/wiki/Domain_name_registrar) [s](https://en.wikipedia.org/wiki/Domain_name_registrar) 等等。该系统是精确配置，让你从浏览器栏到网站无缝连接。这个过程有点疯狂，但也许最疯狂的是，这一切几乎是瞬间发生的。任何时候你浏览网页，打开几十个标签，请求一堆不同的网站，你的电脑都在 ping 世界各地的服务器，为你获取正确的信息。它就这样工作着——直到它不工作。

* * *

### **怎么破？**

DDoS 攻击是一种常见的黑客行为，在这种攻击中，多台被入侵的计算机被用来通过使服务器请求过载来攻击单个系统。在 DDoS 攻击中，黑客通常会使用受感染的计算机来创建来自许多不同来源的大量流量，可能有数千甚至数十万个来源。通过使用所有被感染的计算机，黑客可以有效地避开任何可能放在单个 IP 地址上的拦截。与来自攻击者的请求相比，这也使得识别合法请求更加困难。

在今天早上的攻击中，黑客摧毁了 Dyn 的服务器，这是一个非常受欢迎的 DNS 主机，管理着 Basecamp，CNN，Etsy，Github，Grubhub，HBO Now，Imgur，Paypal，Playstation Network，Reddit，Squarespace 和 Twitter 等网站。

当 Dyn 的服务器被关闭时，浏览器基本上不知道去哪里找到要加载到屏幕上的信息。这种类型的攻击时有发生，黑客创建了一个感染了恶意软件的小型私人电脑大军，称为 [僵尸网络](http://searchsecurity.techtarget.com/definition/botnet) 。经常参与攻击的人没有意识到他们的计算机已经被入侵，他们是僵尸攻击者大军的一员。2014 年，一个名为蜥蜴小队 [的黑客组织使用这种方法关闭了 Playstation 网络和 Xbox Live](http://gizmodo.com/hackers-who-shut-down-psn-and-xbox-live-now-attacking-t-1675331908) 。2015 年，一种名为 [XOR DDoS](http://gizmodo.com/a-new-botnet-hits-servers-with-150-gbps-ddos-attacks-1733743786) 的木马病毒帮助黑客创建了一个强大的僵尸网络，能够瘫痪几乎任何服务器或网站。

保护服务器免受 DDoS 攻击可能很困难，但有一些方法可以防止宕机。据 [网络世界](http://www.networkworld.com/article/2905115/network-security/the-best-way-to-stop-ddos-attacks.html) 报道，最常用的方法之一是流量采样，系统对数据包进行采样，并识别网络流量的趋势。流量分析设备评估业务流并识别潜在的不良业务。

* * *

### 我们如何保护自己？

展望未来，一个大问题凸显出来。我们如何才能避免像这样的攻击，窃取数百万美国人的互联网接入，并使公司损失数百万美元的收入？

答案很复杂。一旦安全公司想出新的方法来保护像 Dyn 这样的公司，黑客就会想出新的方法来攻击它们。然而，就 DNS 基础设施而言，许多人指出，网站避免被一台主机上的攻击搞垮的最佳方式就是订阅多台主机。这就是所谓的 DNS 冗余，也可能是一些网站( [，如 Pornhub](https://news.ycombinator.com/item?id=12759653) )毫发无损地躲过攻击的原因。

在 Dyn 服务器的情况下，还不清楚他们是如何解决问题的，但该公司现在报告说 [问题已经解决](https://www.dynstatus.com/incidents/nlr4yrr162t8)——大约在问题开始后一个小时。