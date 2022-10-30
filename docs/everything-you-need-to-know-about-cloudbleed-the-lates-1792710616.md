# 关于最新的互联网安全灾难 Cloudbleed，你需要知道的一切

> 原文：<https://gizmodo.com/everything-you-need-to-know-about-cloudbleed-the-lates-1792710616>

你听说了吗？Cloudflare 代码中的一个小错误导致了数量不明的数据——包括密码、个人信息、消息、cookies 等等——[泄露到整个互联网](https://www.theregister.co.uk/2017/02/24/cloudbleed_buffer_overflow_bug_spaffs_personal_data/) 。如果你没有听说过所谓的 Cloudbleed 漏洞，那就继续读下去吧。这是一件可怕的大事。

Watch

让我们从好消息开始。世界上最大的互联网安全公司之一 Cloudflare 在谷歌 Project Zero 的安全研究员塔维斯·奥曼迪发现该漏洞后迅速采取了行动。

坏消息是，在奥曼迪注意到这个漏洞之前，Cloudflare 支持的网站已经泄露数据*个月*了。Cloudflare 表示，最早的数据泄露可以追溯到 2016 年 9 月。目前还不清楚在 Cloudflare 修复代码之前，blackhat 黑客是否已经发现了这个漏洞并秘密利用了它。Cloudflare 的客户包括像优步、OKCupid、1Password ( *更新* : 1Password 声称其用户数据 [是安全的](https://blog.agilebits.com/2017/02/23/three-layers-of-encryption-keeps-you-safe-when-ssltls-fails/) )和 FitBit 这样的大公司。这意味着他妈的一大堆敏感数据可能已经被泄露了。

与任何重大安全漏洞一样，我们需要一段时间才能完全理解 Cloudbleed 造成的破坏程度。现在， [你应该更改你的密码](https://gizmodo.com/cloudbleed-password-memory-leak-cloudflare-1792709635)——所有的密码——并且在你能实现的任何地方实现双因素认证。当你读到这个讨厌的小安全灾难是如何发生的时候，你就会明白为什么这是一个好主意。

### 什么是 Cloudflare？

您可能不熟悉 Cloudflare 本身，但该公司的技术正在许多您喜欢的网站上运行。Cloudflare 将自己描述为一家“网络性能和安全公司”。最初是一个追踪垃圾邮件来源的应用程序，该公司现在向网站提供一整套产品菜单，包括基于性能的服务，如内容交付服务；注重可靠性的产品，如域名服务器(DNS)服务；和安全服务，如防止直接拒绝服务(DDoS)攻击。

事实上，Cloudflare 是一家安全公司，这使得围绕这一新漏洞的争论极具讽刺意味。毕竟，无数公司向 Cloudflare 付费以帮助保护其用户数据的安全。Cloudbleed 的错误恰恰相反。

“我已经告诉了 Cloudflare 我在做什么。我发现了来自主要约会网站的私人信息，来自一家知名聊天服务的完整信息，在线密码管理器数据，来自成人视频网站的帧，酒店预订，”塔维斯·奥曼迪 [在一篇咨询](https://bugs.chromium.org/p/project-zero/issues/detail?id=1139) 中写道。“我们谈论的是完整的 https 请求、客户端 IP 地址、完整的响应、cookies、密码、密钥、数据，一切。”奥曼迪还表示，Cloudbleed 漏洞在 2 月份的五天时间里泄露了 3438 个不同域的数据。

### Cloudbleed 是如何工作的？

对于你们这些极客来说，Cloudbleed 尤其有趣，因为 Cloudflare 代码中的一个字符就会导致漏洞。这似乎是一个简单的编码错误，尽管我们已经联系了 Cloudflare 来了解到底发生了什么。( *Updat* e: Cloudflare 叫我们回来T3】解释了一些事情 T5】。)根据报道，Cloudbleed 在某些过程中泄露信息的方式似乎与 Heartbleed 有点类似。Cloudbleed 的规模看起来也像 Heartbleed 一样影响许多用户，因为它影响了许多网站使用的公共安全服务。

根据 Cloudflare 博客文章 的说法，这个问题源于该公司决定使用一种新的 HTML 解析器 cf-html。HTML 解析器是一个应用程序，它扫描代码以提取相关信息，如开始标记和结束标记。这使得修改代码更加容易。

Cloudflare 在格式化 cf-html 的源代码和它的旧解析器 Ragel 以配合自己的软件时遇到了麻烦。代码中的一个错误造成了所谓的缓冲区溢出漏洞。(错误涉及代码中的“==”，而代码中应该有“> =”。)这意味着当软件将数据写入缓冲区时，有限的临时数据空间将填满缓冲区，然后继续在其他地方编写代码。(如果你渴望一个更技术性的解释，Cloudflare 在一篇博客文章 中给出了所有的解释 [。)](https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/)

说白了，Cloudflare 的软件试图将用户数据保存在正确的地方。那个地方已经满了。因此，Cloudflare 的软件最终将这些数据存储在了其他地方，比如一个完全不同的网站。同样，数据包括从 API 密匙到私人消息的所有内容。谷歌和其他网站也缓存了这些数据，这意味着 Cloudflare 现在必须在黑客发现之前将其全部搜索出来。

### 你被 pwn 了吗？

目前还不清楚到底是谁被邀请了。Cloudlfare 声称，只有极少数的请求导致了数据泄露，但由于该漏洞已经存在了近六个月，谁知道有多少信息在外面。此外，如此多的数据被缓存在不同的站点上这一事实意味着，尽管 Cloudflare 的初始补丁阻止了泄露，但该公司需要在网络上进行大量搜索，以确保所有泄露的数据都得到清除。更糟糕的是，即使是不使用 Cloudflare 服务但拥有大量 Cloudflare 用户的网站，也可能在其服务器上泄露数据。

企业家和安全专家 Ryan Lackey 在博客文章 中提供了一些好的建议 [。莱基知道他在说什么，因为他的公司 CryptoSeal 在 2014 年被 Cloudflare 收购了。](https://medium.com/@octal/cloudbleed-how-to-deal-with-it-150e907fd165#.3dzt5g3zx)

“Cloudflare 是许多最大的消费者网络服务(优步、Fitbit、OKCupid 等)的背后，所以与其试图确定哪些服务在 Cloudflare 上，最谨慎的做法可能是利用这个机会轮换所有网站上的所有密码，”Lackey 写道。“用户也应该在此更新后注销并登录他们的移动应用程序。当你在做的时候，如果有可能的话，在你认为重要的网站上使用 2FA 或 2SV。”

更改密码很糟糕，但不管怎样，你应该半定期地这么做。正如我们过去所争论的，你也可以在所有的 上启用双因素认证，因为这是对抗黑客的最佳第一道防线。也就是说，互联网上没有什么是真正安全的，Cloudbleed 可能会危及一些使用。双因素身份验证。

这就是说:你无法控制像 Cloudflare 这样的网站和公司背后发生的事情。但是你可以小心自己的屁股——祈祷黑客神保佑你安全。什么都行。