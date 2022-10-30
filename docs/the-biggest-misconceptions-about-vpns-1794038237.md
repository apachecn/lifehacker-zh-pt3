# 关于 VPN 的最大误解

> 原文：<https://lifehacker.com/the-biggest-misconceptions-about-vpns-1794038237>

你听说了吗？ [互联网服务提供商想要出售你的数据](https://lifehacker.com/senate-votes-to-let-internet-providers-sell-your-web-hi-1793574677) 和一个 [虚拟专用网络(VPN)是告诉他们滚蛋的最好方式](https://lifehacker.com/why-is-everyone-talking-about-vpns-1793768312) 。但是有一个问题。VPN 是出了名的可疑，比它们看起来更复杂，它们不受监管，如果你不正确设置它们，可能比它们的价值更有安全风险。



在 之前，我们已经多次讨论过什么是 [VPN，但是让我们花点时间快速复习一下。VPN 会在数据离开您的设备之前对其进行加密，当数据通过您的本地网络和互联网服务提供商(ISP)到达 VPN 提供商的服务器之前，它会保持加密状态。这个过程被称为“隧道效应”当流量到达 VPN 的服务器时，它被解密并被发送到整个互联网。如果你在公共场所使用互联网，这通常是有用的，比如咖啡店的 Wi-Fi 网络，在那里有人可能试图监视你的流量。如果你想对你的 ISP 隐藏你的流量或者绕过政府的防火墙，它也是有用的，因为他们不会看到你访问的网站。](https://lifehacker.com/why-you-should-be-using-a-vpn-and-how-to-choose-one-5940565)

### “VPN 保护您免受广告跟踪”

VPN 会屏蔽你的 IP 地址，让你的 ISP 相对看不到你，但他们不会阻止互联网上数以百万计的其他广告追踪器。广告网络通常使用 cookies 而不是 IP 地址来识别你的身份，所以如果你使用 VPN 来逃避广告跟踪，你会非常失望。更糟糕的是，一些 VPN 提供商实际上提供他们自己的广告或者出售你的浏览数据。这方面最臭名昭著的例子是 Hola Better Internet，用户 [被抓到注入自己的广告](https://lifehacker.com/many-browser-extensions-have-become-adware-or-malware-1505117457) 。

如果你想阻止广告追踪器，你应该使用关注隐私的浏览器扩展，像 [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en) 和 [Privacy Badger](https://www.eff.org/privacybadger) 。这将防止广告跟踪者跟踪你，也不会像 VPN 那样减慢你的网络浏览速度。

### “使用 VPN 时，您甚至不会注意到差异”

安全是以速度为代价的，使用 VPN 几乎总是会使你的网络连接速度变慢一点。在安全协议和加密之间，这是无法回避的。

这有多重要取决于你在互联网上做什么，你的 VPN 提供商的速度，以及其他一些潜在的瓶颈。对于一般浏览来说，这不会有很大的不同，但是你会注意到大文件下载或上传和视频流的速度会变慢。

一些服务和网站完全阻止 VPN，因为他们不想让你绕过地区限制。网飞最臭名昭著的就是这个 ，不过 Hulu 也尝试过。这可能会有不同的效果，取决于你在世界上的位置。

### “使用 VPN 使您自动变得安全和私密”

VPN 的全部目的是安全，但是如果你设置错误(或者提供商设置错误)，那么你可能会失去安全。同样，您的 VPN 提供商可以看到您的所有流量，这意味着它可能会记录您所做的一切，甚至修改流量。

[高科桥公布的研究发现](https://www.htbridge.com/blog/90-percent-of-ssl-vpns-use-insecure-or-outdated-encryption.html) 许多 VPN 使用了几种不同的过时加密方法中的一种，包括非常过时的 [点对点隧道协议](https://en.wikipedia.org/wiki/Point-to-Point_Tunneling_Protocol) (PPTP)。这是假设他们正在加密数据，VPN 可以做他们想做的任何事情，直到有人叫出他们的 BS。不相信我？今年早些时候， [安全研究人员发现](https://lifehacker.com/researchers-issue-security-warnings-about-several-popul-1791617644)Android 上 18%的 VPN 应用程序没有做 VPN 应该做的一件基本事情:加密流量。84%的人还泄露了用户数据。那只是在安卓上。

如果 VPN 设置不正确，它还可能泄露你的 IP 地址，这将把你的所有数据链接回你，如果你出于隐私使用 VPN，这将是一个问题。在你设置好 VPN 后，测试它到 [确保它没有泄露你的 IP 地址](https://lifehacker.com/how-to-see-if-your-vpn-is-leaking-your-ip-address-and-1685180082) 。泄露可能是由于 [一个旧的网络漏洞](https://lifehacker.com/stop-opera-s-new-vpn-from-leaking-your-ip-address-1773359437) ，或者是由于一个基本的 [安全漏洞当它的](https://lifehacker.com/how-to-make-your-vpn-even-more-secure-5902397) 设置不正确的时候。

当涉及隐私时，日志也是一个至关重要的问题。有些 [VPN 提供商会记录你所有的流量](https://lifehacker.com/how-do-i-know-if-my-vpn-is-trustworthy-508866499) ，这违背了出于隐私目的使用 VPN 的目的。如果你搜索一个 VPN 提供商，并在谷歌查询中“登录”，你应该调出他们的隐私政策。在那里，你会发现他们是否记录了你所有的流量，你的访问日志，或“任何执法要求”，这是一种逃避，因为这可能包含了广泛的事情。对于真正的隐私*和*匿名， [Tor 是比 VPN](https://lifehacker.com/what-is-tor-and-should-i-use-it-1527891029) 更好的选择，因为它使得任何数据都很难追溯到你。

### “有一个最好的 VPN”

如果有人能编制一份最佳 VPN 列表，这将使每个人的生活更轻松，对吗？但事实证明，选择一个值得信赖和可靠的 VPN 几乎是不可能的。在最基本的层面上，*你为什么使用 VPN 会影响你寻找一个可靠的 VPN。有些更多的是关于安全，有些是关于绕过区域街区，而其他的更多的是关于隐私。有些在美国，许多不在。所有这些因素都会改变这项服务的运作方式。*

与我们使用的许多服务不同，VPN 不受监管，也不会通过安全审计。一个 VPN 可以说任何他们想说的关于隐私和安全的事情，但是没有人让他们负责。他们唯一的公共责任来自用户揭露的不正当行为。

也就是说，你必须做你的研究。除了在谷歌上快速搜索之外，安全还需要做功课。 [我们在](https://lifehacker.com/how-do-i-know-if-my-vpn-is-trustworthy-508866499) 之前已经讨论过这个问题了:你需要搜索一个 VPN 提供商的登录规则，看看论坛上的帖子，看看是否有人在谈论它们，并在设置好之后测试你的 VPN。如果你在网上找不到任何关于 VPN 提供商的信息，或者如果一个交易听起来“好得不像真的”，它可能就是真的。令人欣慰的是，一项服务越受欢迎，就有越多的人对这项服务负责。

今天，VPN 可能进入了公众的视野，但这并没有使它们比两周前更容易理解。它们很复杂，很无聊，虽然设置一个很简单，但找到一个合法的需要和其他 50-100 美元/年的购买一样多的努力，所以把它当成一个。

对于我们来说，我们长期以来一直推荐、 [SlickVPN](https://www.slickvpn.com/) 、 [NordVPN、](https://nordvpn.com/)[Hideman](https://www.hideman.net/)和 [Tunnelbear](https://www.tunnelbear.com/) ，因为它们多年来一直享有盛誉，但这不是一个包罗万象的列表，也不是一个我们可以不断更新的列表。 [隐私网站试图根据 VPN 的位置、登录规则等对其进行分类，但即使如此，这也是一项非常复杂的任务，永远不会完全更新。](https://thatoneprivacysite.net/vpn-comparison-chart/)

无论你选择哪种服务，确保你提前做了必要的研究，然后花一些额外的时间来确保一切都已设置好并正常工作。