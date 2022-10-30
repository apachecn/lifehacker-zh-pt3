# 云出血是一个问题，但它变得更糟

> 原文:[https://gizmodo . com/cloud bleed-is-a-problem-but-that-be-worse-1792721147](https://gizmodo.com/cloudbleed-is-a-problem-but-it-gets-worse-1792721147)

像 Cloudbleed 这样的巨大安全灾难 [从来都不是好玩的。然而，随着关于新报告的漏洞的更多信息变得可用，我们可以理解错误对搞砸互联网有多危险。幸运的是，对于 Cloudbleed 来说，情况并没有想象中那么糟糕。但是也不好。](https://gizmodo.com/everything-you-need-to-know-about-cloudbleed-the-lates-1792710616)

Watch

如果你没听说过的话，Cloudbleed， [是一个主要的漏洞](https://gizmodo.com/everything-you-need-to-know-about-cloudbleed-the-lates-1792710616) ，它可能会影响由安全和性能服务 Cloudflare 提供服务的数百万个网站。Cloudflare 代码中的一个小错误导致不确定数量的数据(包括加密密钥、聊天日志、cookies 和密码)泄露到公开的网络上，并被谷歌等搜索引擎缓存。Cloudflare 的客户包括优步、OKCupid 和 Fitbit 等大型网站，这意味着大量用户发现自己处于不知道自己的个人数据有多少(如果有的话)被泄露的不幸境地。

太糟糕了。Cloudflare 的联合创始人兼首席执行官马修·普林斯(Matthew Prince)周五在 Gizmodo 的一次采访中也说了同样的话。“这对我们来说是一件大事，”普林斯说。“这是一个非常糟糕的错误。我们的客户应该非常清楚这一点，并认真对待。”

然而，普林斯称这也是终端用户的光明面。根据 Cloudflare 的说法，大多数易受该漏洞攻击的网站很少被交易，“被遗忘的 WordPress 博客”普林斯声称，在 Heartbleed fuckup 最严重的时候，只有 3500 个域名最终遭到破坏，而且那些只是在涉及破损 HTML 标签的非常特殊的情况下泄露信息。普林斯还说，这些网站 90%的流量来自像谷歌这样简单索引网页的来源。

谷歌抓取的细节让 Cloudbleed 变得特别可怕。被 Cloudflare 的 bug 吐到页面上的数据确实包括私人聊天的片段和随机观看的视频帧。普林斯也承认了。事实上，无数的搜索引擎保存了隐私数据，这确实令人不安。更令人不安的是，我们不知道有多少数据留在野外，也不知道 Cloudflare 在搜索引擎的配合下能够销毁多少数据。

普林斯表示，在谷歌安全研究员塔维斯·奥曼迪通过 Twitter 向该公司通报漏洞后仅 44 分钟，泄露就被阻止了。普林斯告诉 Gizmodo:“在那条推文发布七个小时后，我们已经完全修复了我们的系统，防止了数据泄露。”。该公司继续与搜索引擎合作，清除存储在搜索引擎缓存中的数据。

尽管如此，Cloudflare 还无法量化到底有多少数据被泄露。Prince 确实说过 150 个 Cloudflare 客户(理解为:150 个网站或服务)遭遇了泄露。Prince 还声称，从去年 9 月开始泄露到今天，对 Cloudflare 支持的网站的请求没有明显增加。这意味着该公司相当有信心黑客没有在谷歌的研究人员之前发现这个漏洞。

安全企业家兼前 Cloudflare 员工 Ryan Lackey 自该漏洞公开以来一直在报道该漏洞。在接受 Gizmodo 采访时，Lackey 表示，Cloudbleed 最令人恐惧的是揭示了小错误如何导致大问题。此外，还有更大的威胁。

“我不认为这是任何人的最高风险或最高暴露程度，”Lackey 告诉 Gizmodo，引用更常见的网络攻击，如网络钓鱼，是更危险的。“这对单个客户造成影响的可能性非常低。”

这听起来是个好消息。任何想要确保其数据完全安全的人都应该更改其密码并启用双因素身份验证。这更像是对安全风险的哲学回应。但 Lackey 继续解释说，Cloudflare 的影响范围与这一新发现的漏洞相结合，表明更具侵略性的利用可以有效地使互联网停止运行。

“这是 Cloudflare 最微小的妥协，”Lackey 说。“对 Cloudflare 的适度妥协可能会成为威胁互联网的(事件)。”

因此，从好的方面来看，据 Cloudflare 的首席执行官和一名前 Cloudflare 员工称，大多数用户可能都很好。焦虑的用户应该更改他们的密码，不管有没有安全威胁，这确实是一件很棒的事情。话说回来，Cloudbleed 说明了一个更大的互联网安全问题。如果一个主要玩家被 pwn，后果可能是灾难性的。

看起来 Cloudbleed 更像是一次警告而不是致命一击。这是好消息。但坏消息是，这一事件表明，在保护个人信息方面，互联网用户应该比以往任何时候都更加警惕。有时，像 Cloudflare 这样的大公司会搞砸。在这种情况下，避免成为受害者的最好方法就是小心自己的屁股。

使用良好、安全的密码。( [这里有一个生成一个](http://gizmodo.com/create-an-ultra-secure-easy-to-remember-passphrase-usi-1694021321) 的好策略。)使用双因素身份验证。如果一切都失败了，祈祷吧。