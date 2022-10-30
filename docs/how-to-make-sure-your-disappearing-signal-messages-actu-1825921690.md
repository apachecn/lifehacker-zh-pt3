# 如何确保你的消失信号真的消失了

> 原文:[https://life hacker . com/how-to-make-assure-your-missing-signal-messages-actu-1825921690](https://lifehacker.com/how-to-make-sure-your-disappearing-signal-messages-actu-1825921690)

当谈到消息应用程序时，是最安全的选择之一，但事实证明，如果你在 Mac 上使用它，这项服务实际上有一个相当大的漏洞。

Watch

你的 [消失的信息](https://www.tomsguide.com/us/signal-disappearing-messages-how-to,news-23660.html) (你知道，那些被认为是*在一段时间后自毁*的信息)实际上是默认存储在你的 Mac 上的。这里是你需要知道的，以确保任何通过信号发送的敏感信息实际上像它应该的那样消失了。

### 有什么问题？

这一切都归结于 Mac 上的通知中心。如果你在电脑上使用 Signal，每条新信息都会以提醒的形式出现，储存在通知中心，内容和发件人姓名都清晰可见。

有点令人惊讶的是，这是真的，即使你收到的信息应该是自毁的。即使它们从信号应用程序中消失，它们仍会在通知中心和电脑上的其他地方可见。这个问题最初是由安全研究员亚历克·穆菲特发现的，他在推特 上分享了他的发现 [。在](https://twitter.com/AlecMuffett/status/993917102791766016?ref_src=twsrc%5Etfw&ref_url=https%3A%2F%2Ftwitter.com%2FAlecMuffett%2Fstatus%2F993917102791766016) [主板](https://motherboard.vice.com/en_us/article/kzke7z/signal-disappearing-messages-are-stored-indefinitely-on-mac-hard-drives) 注意到这条推文后， [帕特里克·沃德尔](https://objective-see.com/blog/blog_0x2E.html) (另一位 Mac 安全研究员)对 Signal 的安全漏洞进行了更深入的挖掘。

Lifehacker 也发出了评论信号，如果我们收到回复，它将更新这个故事。

在 [的一篇博客文章](https://objective-see.com/blog/blog_0x2E.html) 中，沃德尔解释道，黑客仍然需要进入你的电脑(无论是远程的还是物理的)才能看到你的信号信息。因此，对大多数人来说，这不是问题，但如果你真的使用信号来分享敏感或有价值的信息，这可能是一个真正的问题。谢天谢地，有一个简单的方法可以解决这个问题。

### 解决方案

为了确保你消失的信号信息确实消失了，只需在 Mac 上打开应用程序，进入首选项(点击屏幕右上角的信号，该选项应该会弹出)。在“通知”部分，选择“既不是姓名也不是信息”如果你还想知道一些有用的信息而不需要透露所有信息，你也可以选择“仅发件人姓名”。

下次你在 Mac 上收到信号通知时，它不会在你的电脑上储存任何敏感信息。不幸的是，这并没有解决 Mac 已经记录的信息“消失”的问题，这就是事情变得复杂的地方。

### 检查你的数据库

沃德尔发现，只要稍加编码，所有这些自毁信号信息也会保存在 Mac 电脑内部的数据库中。实际上，访问这些信息可能超出了大多数人(包括我自己)的技能范围，但是如果你准备好迎接挑战，你可以在这里跟随 Wardle(专业 Mac 安全研究员) [。](https://objective-see.com/blog/blog_0x2E.html)T3】

为了让事情变得简单一点，他还设置了一个脚本，它可以扫描你的 Mac 并显示所有隐藏的通知数据。通过这种方式，您将知道在进行实际清除数据库的困难工作之前，有值得删除的数据。然而，对我们大多数人来说，简单地确定你将来收到的任何消失的信息确实消失了，这就足够让你安心了。