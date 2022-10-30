# 以下是 Chrome 新安全警告的实际含义

> 原文：<https://lifehacker.com/heres-what-chromes-new-security-warnings-actually-mean-1827836754>

Chrome 粉丝可能已经注意到他们的浏览器今天有了一点变化。假设你运行的是 Chrome 的最新版本 68， [现在每当你打开一个以 http://而不是 https://开头的网站时，你都会在地址栏看到一个大大的“不安全”按钮](https://www.troyhunt.com/why-no-https-heres-the-worlds-largest-websites-not-redirecting-insecure-requests/) 。(值得一提的是，我使用的是 Chrome 版本 67.0.3396.99，每当页面有数据输入字段时，它也会在那里弹出。)

Watch

你会忽略这个警告吗？大概吧。你应该吗？大概不会。网络安全专家 Troy Hunt 在下面的视频中解释了为什么网站使用 HTTPS(即“安全的”超文本传输协议)很重要。它绝对值得一看，但这里有一个简短的版本:对于公司、黑客或其他任何在你的网络旅行中有既得利益的人来说，注意到你的 HTTP 请求并不困难，就像当你想访问一个特定的网站时；拦截此请求；然后用你不想要的东西修改它，比如广告、弹出窗口或完全不同的网站。

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-_BNIkw4Ao9w&start=66](https://lifehacker.com/embed/inset/iframe?id=youtube-video-_BNIkw4Ao9w&start=66)

<figcaption class="sc-1ptbguh-0 hxeMec caption">“Here’s Why Your Static Website Needs HTTPS” — Troy Hunt</figcaption> 

当你输入一个简单的域名时，大多数网站都会很好地将你重定向到他们的 HTTPS 版本:亚马逊、微软、Tumblr、Lifehacker 等等。但是有很多网站不这么做，亨特创建了一个自己的网站来追踪这些罪犯——[为什么没有 HTTPS？](https://whynohttps.com/)T3】

在上面，他列出了世界上 100 个当你输入域名时不会自动重定向到 HTTPS 版本的网站。违规者(及其 Alexa 排名)包括 Baidu.com(排名第 4)、qq.com(排名第 6)、bbc.com(排名第 105)、espn.com(排名第 136)、foxnews.com(排名第 211)，甚至 speedtest.net(排名第 237)，仅举几例。

令人沮丧的是，其中一些网站实际上有安全版本；你只需要输入 https://和域名，而不仅仅是 websitename-dot-com 就可以访问它(除非它有某种偏好或设置，你可以在访问该网站时检查自动重定向到 https 版本)。然而，这个技巧并不适用于所有的网站。你可以 https://www.espn.com 所有你想要的，你仍然会被重定向到一个不太安全的 HTTP 网站。

### 当你最喜欢的网站不支持 HTTPS 时——或者你是这么认为的

我推荐抢浏览器扩展 [HTTPS 无处不在](https://www.eff.org/https-everywhere) 。这是一个很棒的小工具，由 Tor 项目和电子前沿基金会创作，试图通过尽可能将您的浏览器连接到 HTTPS 版本的网站来解决这些问题。它并不完美，也不神奇。正如 EFF 指出的，它不能凭空创造网站安全:

> 只有当您使用受支持网站的加密部分时，HTTPS Everywhere 才会保护您。在受支持的站点上，它会自动激活站点所有已知受支持部分的 HTTPS 加密(对于某些站点，这可能只是整个站点的一部分)。例如，如果您的网络邮件提供商根本不支持 HTTPS，HTTPS 无处不在就不能保证您访问网络邮件的安全。同样，如果一个网站允许 HTTPS 显示文本，但不允许显示图片，那么有人可能会看到你的浏览器加载了哪些图片，并猜测你在访问什么。
> 
> 任何地方的 HTTPS 都完全取决于您使用的各个网站的安全特性；它会激活这些安全功能，但如果它们不存在，它就无法创建它们。如果您使用不受 HTTPS Everywhere 支持的站点或以不安全的方式提供某些信息的站点，HTTPS Everywhere 无法为您使用该站点提供额外的保护。在发送或接收机密信息(包括密码)之前，请记得检查特定网站的安全性是否达到您预期的水平。"

如果你只是在浏览器中漫不经心地点击网站，你可能不需要太在意 HTTP 和 HTTPS 的区别——除非你在浏览过程中开始经历一些奇怪的事情。至少，SecurityMetrics 分析师布兰德巴尼在 2014 年的博客文章中是这样表述的:“如果你只是在浏览网页，看看猫的迷因，梦见那件 200 美元的电缆针织毛衣，HTTP 是没问题的。”

所以，在家里查看 ESPN 的体育比分——在网站不太安全的连接上可能没问题。如果你在咖啡店登录你的 ESPN 账户，我会 [稍微紧张一点](https://www.reddit.com/r/web_design/comments/7wxvia/so_espns_website_is_not_only_not_https_but_even/) (可能不会这么做)。如果我实在忍不住，我会确保我的 ESPN 登录凭证与我在任何其他网站或服务上使用的任何东西都不一样，而且我绝对 [不会输入我的信用卡信息](https://lifehacker.com/what-should-i-do-if-my-credit-card-gets-hacked-1552850022) 在 ESPN 的网站上购买任何东西(如果你甚至能做到这一点的话)。

换句话说，HTTP 不太可能给你带来随意浏览的问题，但是一旦你开始输入你不想让别人知道的信息——密码、支付信息、你的地址、你的社会保险号等等。—在不安全的连接上这样做是愚蠢的。更糟糕的是，你不希望在一个开放的无线网络上通过不安全的 HTTP 连接发送信息，在你的咖啡店，或者在同一网络上你不认识的许多人可能在网络上窃听你的任何地方。

尽管大多数网站 已经转移到 HTTPS，但你还是要确保更加关注谷歌在 Chrome 中的标注。在一个完美的世界中，当你要在一个不安全的网站上做一些你不应该做的事情时，谷歌会让“不安全”图标变红并闪烁以引起你的注意，但我们认为，地址栏中更大的指示器总比没有好。下次你打算在网上买东西时，一定要快速浏览一下你的浏览器。