# 这些愚蠢的“物联网”黑客是我们自找的

> 原文:[https://life hacker . com/we-ve-bring-things-internet-of-things-hacks-u-1793313692](https://lifehacker.com/we-ve-brought-these-stupid-internet-of-things-hacks-u-1793313692)

无论是报道不多的关于 [黑掉三星电视](https://www.wired.com/2017/03/worried-cia-hacked-samsung-tv-heres-tell/) 的故事，还是令人悲伤的关于 [黑掉泰迪熊](https://arstechnica.com/security/2017/02/creepy-iot-teddy-bear-leaks-2-million-parents-and-kids-voice-messages/) 的爆笑故事，甚至是更多关于窃听微波炉 的 [离奇说法，真实的、虚假的、夸大的关于我们选择用来连接互联网的设备可能发生的所有事情的报道都占据了新闻。我们给自己带来了这个愚蠢的未来。](http://theslot.jezebel.com/kellyanne-when-asked-about-trump-wiretapping-claims-b-1793211096) 

Watch

在过去的几年里，我们打着简单的幌子，尽可能地将任何东西连接到互联网上。可以连接 [灯泡](https://www.lifx.com/)[冰箱](http://www.samsung.com/us/explore/family-hub-refrigerator/)[情趣用品](http://we-vibe.com/)[宠物喂食器](http://www.petnet.io/) 等等。这些设备通常被称为物联网(IoT)。他们的想法是多么糟糕，已经成为一个笑话，但是这并没有阻止他们以更快的速度出现。

物联网设备有很多潜在的问题，但最普遍和值得讨论的两个问题是安全性和可用性。

### 物联网设备的安全性已经很差，消费者似乎也不关心如何改善

物联网设备的安全性如此糟糕，以至于当我们听到被黑客攻击的物联网设备时，我们通常会集体耸耸肩。这还不是什么大不了的事，但将来会是。

让我们先倒回去一点。这里有几个不同的安全场景。侵入你的物联网设备以进入你的网络，侵入你的设备以创建僵尸网络，并监视你。

首先，物联网设备很难保护。出于可用性的考虑，它们往往安全性较弱。使用双因素认证和强密码连接到联网灯泡将是一件痛苦的事情，因此，他们使用易于颠覆的简化防御系统。开箱后，一个灯泡会广播一个 Wi-Fi 信号，并要求您连接到它并输入您的 Wi-Fi 网络信息。如果黑客有很好的时机，并且靠近你的房子， [他们可以很容易地欺骗那个灯泡来获得你的 Wi-Fi 登录](http://www.bbc.com/news/technology-28208905) 。这种情况很少见，尤其是考虑到他们需要靠得有多近。不过这个距离已经在扩大，包括纽约时报报道的一个灯泡黑客在 229 英尺之外工作。

我们已经看到了类似的安全漏洞，从无线连接的芭比娃娃 到吉普车。三星有一款智能冰箱没有 [检查 SSL 证书](http://www.theregister.co.uk/2015/08/24/smart_fridge_security_fubar/) ，这意味着有人可以利用 [中间人攻击](http://hackerspace.kinja.com/how-to-defend-yourself-against-mitm-or-man-in-the-middl-1461796382) 窃取你的谷歌登录信息。这一切都很小众，直到 2016 年 10 月的一次黑客攻击使用物联网设备关闭了互联网的大部分。

原来这些中断是一次 [分布式拒绝服务攻击](http://lifehacker.com/this-video-explains-everything-you-need-to-know-about-d-1709485477) (DDoS)的结果。这时黑客会用虚假流量淹没网站，导致网站崩溃。10 月，受害者是一家名为 Dyn 的公司，这是路由网络流量的实体之一。被黑的物联网设备助长了分布式拒绝服务。黑客使用了一个名为 Mirai 未来组合僵尸网络的系统，该系统扫描网络，寻找仍具有出厂默认用户名和密码的物联网设备。然后，它入侵该设备，用它来冲击网站的流量。在 Mirai 未来组合事件中，我们自己的疏忽暴露无遗。数量惊人的人不会改变他们设备上的默认登录。

* * *

间谍活动有几种不同的方式。我们大多数人更传统的想法是类似于 [中情局使用三星电视来窥探人们的谈话](http://gizmodo.com/wikileaks-just-dumped-a-ton-of-alleged-cia-hacking-docu-1793042726) 。考虑到去年前美国国家情报目录 [称](https://www.theguardian.com/technology/2016/feb/09/internet-of-things-smart-home-devices-government-surveillance-james-clapper) “在未来，情报部门可能会使用[物联网]进行身份识别、监视、监控、位置跟踪，并锁定招募目标，或者获取网络或用户凭据，这应该不会令人惊讶。”

整个中情局的事情有点夸张，因为它需要一个拇指驱动器连接到电视上，整个事情都用固件更新补丁，但它为监控树立了一个可怕的先例。不仅政府对间谍活动感兴趣，制造这些设备的公司也是如此。

例如， [We-Vibe 情趣用品](http://we-vibe.com/) 最近在研究人员发现其未经用户同意非法收集数据后，达成了375 万美元的和解。这种侵犯隐私的行为之所以被发现，是因为 [安全研究人员发现了一个软件漏洞](https://www.cnet.com/news/vulnerable-vibrator-security-researchers-find-flaws-in-connected-toy/) ，这个漏洞可能会让黑客远程控制振动器。然后他们发现用户偏好和统计数据被发送到 We-Vibe 的服务器上。We-Vibe 并不是唯一一家这样做的公司， [Vizio 最近因非法收集智能电视](http://gizmodo.com/tv-maker-vizio-to-pay-out-millions-after-secretly-colle-1792056140#_ga=1.46895396.2073333045.1479846166) 上的用户数据而达成和解，亚马逊正在移交 [一起谋杀案](http://gizmodo.com/amazon-agrees-to-hand-over-data-in-echo-murder-case-1793039360) 中 Echo 录制的音频。

很多问题都是我们自己的错。尽管我们并不需要这些设备，但我们还是会购买。我们正在将带麦克风的电视连接到互联网，尽管我们有几十种其他设备比任何智能电视都要好。然后，更糟糕的是，我们忽略了更改这些设备上的密码。

除此之外，我们自己的偏执让事情变得更糟。我认识的每个人都开始接受政府通过电视监视我们的观点。因此，当维基解密公布中情局利用三星电视监视人们的信息时，没有人在意。这也不是什么新想法。 [斯诺登的泄密事件](http://io9.gizmodo.com/all-the-leaked-nsa-documents-rounded-up-into-one-place-1468650331) 带来了同样的反应。这种无忧无虑的疏忽态度已经导致了一些基本无害的黑客攻击。但随着时间的推移，情况肯定不会变得更好。

### 未来会变得更加愚蠢，你的生活不会变得更好

除了安全问题，还有一个可疑的说法，即这些设备首先需要存在。大多数物联网设备似乎都是从头脑风暴会议中产生的，这些会议会问一个问题:“如果我能在手机上查看这个，那不是很好吗？”

比如，如果我能从手机上 [控制一个瓦罐](https://www.crock-pot.com/wemo-landing-page.html) 岂不是很好？或者如果我的 [直肠温度计在线存储数据](https://www.amazon.com/dp/B00UFOBDNY/ref=olp_product_details?_encoding=UTF8&asc_campaign=InlineText&asc_refurl=https://lifehacker.com/we-ve-brought-these-stupid-internet-of-things-hacks-u-1793313692&asc_source=&hsCtaTracking=7d458fc8-d850-4016-b149-dfb9becbbc6d|164daf40-5450-4266-8fc3-fea97b04ada2&tag=kinjalifehackerlink-20) 不是很好吗？也许你想知道冰箱里有多少鸡蛋，在这种情况下，如果一些 [神奇的装置存在](https://www.amazon.com/Quirky-Egg-Minder-Enabled-Smart/dp/B00GN92KQ4/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/we-ve-brought-these-stupid-internet-of-things-hacks-u-1793313692&asc_source=&tag=kinjalifehackerlink-20) 可以告诉你，那不是很好吗？

将一台设备连接到互联网，只不过是一个让你购买你已经拥有的东西的新版本的计划。瓦罐锅最大的好处之一就是你可以把它放好，然后忘记它。你(希望)没有充分使用直肠温度计，以至于你需要在线跟踪这些数据。如果你需要一个应用程序来告诉你冰箱里有多少鸡蛋，你会遇到比决定在杂货店买什么更大的问题。你的冰箱里有无线信号吗？

即使有用的物联网设备仍然存在严重的问题。如果网络瘫痪，你就无法控制你的智能恒温器。更糟糕的是，你可能无法用价格昂贵的联网宠物喂食器给你的猫 喂食。如果一家公司倒闭了， [就像 Nest 收购的智能家庭中心初创公司 Revolv](http://gizmodo.com/nest-owned-smart-hub-gets-permanently-killed-1768977505) 一样，你所有的设备都变得一文不值。即使你喜欢物联网的想法，但事实仍然是，这些设备几乎都不能相互通信。即使是你的黑房子也需要 25 个应用程序来触发你从来没有用过的愚蠢的“派对模式”。

* * *

我还没有看到一个物联网设备真正大规模地提高了我的生活质量。当谈到可访问性时，像 Echo 这样的东西可以让一些人的生活更容易，但很难看到它如何帮助广大消费者。当然，现在设置我的恒温器比在那个垃圾的液晶屏幕上要稍微容易一些，但是它需要互联网吗？我可以在设备上使用触摸屏。除了把一个无聊的设备变成一天的有趣玩具之外，额外的互联网相关功能似乎收益递减。

没有迹象表明这一切会改变。事实上，所有迹象都表明物联网变得越来越愚蠢，直到最终一切都在线。

物联网似乎势不可挡。一名研究人员建议，到 2025 年 T3，互联网上将会有超过 800 亿台智能设备。这意味着你家里的所有东西都将联网。从冰箱到办公椅。我们一直在购买这些设备，因为我们要么相信追加销售，要么仍然梦想着*杰特森夫妇*向我们承诺的智能家居。物联网设备制造商没有尝试创新。他们把一台准系统电脑塞进一个预先存在的设备，制作一个不安全的应用程序，然后就收工了。

接下来会发生什么至少部分取决于我们。你可以要求更好的安全措施。或者你可以拒绝购买这些垃圾。这是否真的会改变设备制造商的做法还不确定，但至少你不用担心政府会监视你的微波炉。

如果没有别的，改变你的默认密码。