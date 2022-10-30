# 如何让您的 Mac 尽可能安全

> 原文：<https://lifehacker.com/how-to-make-your-mac-as-secure-as-possible-1829531978>

[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)) : title[![](../Images/80a55aae3a4e6ac59b23fae8fccddf22.png)](https://applemacos.kinja.com)[Lifehacker's Complete Guide to macOS](https://applemacos.kinja.com)Many people turn to Macs because they're incredibly easy to operate. That's true, but there's still plenty worth knowing before you can truly master your Mac.

在最近一篇名为“ [强化 macOS](https://blog.bejarano.io/hardening-macos.html) 的博客文章中，“Ricard Bejarano 提供了一个广泛的设置列表，您可以调整这些设置以使 macOS 尽可能安全。这是一份全面的任务清单——我们很喜欢——但重要的是，你也要理解他的建议背后的“为什么”。以下是他的一些提示和解释，解释了为什么要这样调整、安装或修改 Mac:

### 系统偏好设置是你新的最好的朋友

**Ricard 的建议:** *“让你的系统保持最新，包括 macOS 和安装的软件”*

Watch

苹果经常发布安全更新，并经常迅速为新威胁提供补丁。保持软件更新是系统安全性的一个重要组成部分，并不是每个人都会一直检查“系统偏好设置”来获取最新更新。如果你没有运行 macOS Mojave，你应该经常查看软件更新。甚至在你的日历上把它变成两周一次的待办事项。

如果你*运行的是*Mojave，你可以将 Mac 更新设置为自动安装。前往**系统偏好设置>软件更新**，勾选“自动保持我的 Mac 最新”如果该复选框没有被完全选中(它有一个连字符而不是勾号)，请打开“高级”并确保所有复选框都被选中(尤其是“安装系统数据文件和安全更新”)。

### 使用两个帐户而不是一个

**理查德的建议:**

*   *"创建一个具有强密码且无提示的管理员用户帐户。该用户仅用于管理目的。*
*   *“进入系统偏好设置>用户&群组，创建一个非特权用户账户供日常使用，这是苹果自己认为的最佳做法”*

当你大部分时间只使用一个帐户时，为自己建立两个帐户可能会感觉有点奇怪，但这是一个加强日常使用系统安全性的好方法。

设置一个具有强密码的管理员帐户，当您需要修改软件、更新钥匙串等时，您将使用该帐户。然后，建立一个单独的非特权账户作为你的默认账户，这将在你安装软件或使用一些“超级用户”应用程序(例如自动化)时设置一些限制。

这通过限制能力来限制你的曝光率。(你可以随时使用你的管理员帐户，通过超级安全的密码，来批准你的用户帐户在默认情况下无法执行的活动。)

### 让已确定的开发人员的应用程序也能工作

**Ricard 的建议:** *“前往系统偏好设置>安全&隐私>常规，并设置允许应用程序从下载到 App Store 或 App Store 并识别开发者”*

虽然 App Store 提供了最好的应用安全性([](https://bgr.com/2015/09/24/iphone-apps-xcodeghost-malware/)*)，但你最喜欢的很多应用可能直接来自第三方开发者。“确定的开发者”是指应用程序的开发者使用了代码签名，这是一个由苹果公司监管的过程，要求开发者拥有苹果公司的账户，并提供验证其真实性的应用程序。*

*这不是一个万无一失的安全措施，因为任何人都可以获得一个开发者帐户并签署他们的应用程序，尽管 butApple 可以撤销开发者的证书，如果它在他们的应用程序中检测到恶意软件活动或其他不当行为。如果你只想运行苹果自己检查和批准的应用，只选择“应用商店”——但是我们和 Ricard 认为也可以扩展到“确定的开发者”。*

### *保护您的隐私*

***Ricard 的建议:** *“进入系统偏好设置>安全&隐私> FileVault 并打开 FileVault(注意:可能需要一些时间)”**

*FileVault 是 Apple 加密数据的内置方法，如果其他人可以物理访问您的系统，它可以防止其他人访问您的数据。真的没有什么好理由*不*使用 file vault——如果你运行的是相当新的东西(在过去几年左右),它不会影响你的系统性能。*

*你还应该确保你的备份(你*正在*备份，对吗？)ar 经过加密和密码保护，无论你是在制作 Time Machine 备份，还是将数据发送到云服务。幸运的是，大多数流行的备份服务会自动加密你发送给他们的数据——确保你选择了一个强密码(如果可能的话，使用双重认证)。*

### *也许不要把你的位置分享给每个应用*

***李嘉图的建议:** *“进入系统偏好设置>安全&隐私>隐私>位置并取消选中启用位置服务”**

***位置服务**是一个需要你用便利换取隐私的领域。你想让 Spotlight(和 Siri)根据你的位置提供建议吗？如果你在 Spotlight 中输入“天气”，你想要当地的天气预报吗？这些都是相当无害的用例，但还有其他应用程序可能会利用定位服务进行更邪恶的手段。当你在你的系统上使用他们的应用时，你真的想让某个随机的开发者(或公司)知道你在哪里吗？*

### *停止您的 Mac 的建议*

***李嘉图的建议:** *“进入系统偏好设置> Spotlight >搜索结果，取消选择 Spotlight 建议并允许在 Look up 中使用 Spotlight 建议”**

*当 OS X Yosemite 中引入 Spotlight 建议时，相关的 [隐私问题](https://intego.com/mac-security-blog/spotlight-suggestions-in-os-x-yosemite-and-ios-are-you-staying-private/) 很快出现。Spotlight 查询不仅向苹果发送有限的个人数据，还向微软的 Bing 搜索引擎发送数据。来自苹果的隐私声明:*

> **当您使用 Spotlight 时，您的搜索查询、您选择的 Spotlight 建议以及相关的使用数据将被发送到 Apple。在 Mac 上找到的搜索结果将不会被发送。如果您在 Mac 上打开了定位服务，当您搜索 Spotlight 时，您的 Mac 的位置将被发送到 Apple。对常用词和短语的搜索将从苹果转发到微软的必应搜索引擎。这些搜索不由 Microsoft 存储。发送给苹果公司的位置、搜索查询和使用信息将仅由苹果公司用于提高 Spotlight 建议的相关性以及改进其他苹果产品和服务。**

*如果您使用 Safari，您还需要在浏览器中前往**偏好设置>搜索**，取消选中*包括 Spotlight 建议*。*

### *使用不同的 DNS 安全冲浪*

***Ricardo 的建议:** *“进入系统偏好设置>网络>高级> DNS，为 1.1.1.1 和 1.0.0.1 的 DNS 服务器添加两个条目并移除任何其他服务器”**

*在 Ricard 的列表中有一个完整的列表，列出了为安全和隐私设置网络浏览器的方法。值得进一步解释的一点是第三方 DNS 解析器的使用。里卡多推荐`1.1.1.1` ( [Cloudflare 的服务](http://blog.cloudflare.com/dns-resolver-1-1-1-1/) )和`8.8.8.8` ( [谷歌的](https://en.wikipedia.org/wiki/Google_Public_DNS) )。Cloudflare 和 Google 都有自己的二级地址，还有像 [OpenDNS](https://opendns.com) 这样的附加选项。*

*第三方 DNS 是比你的 ISP 更好的选择，因为它可能会(稍微)快一些。一般来说，第三方 DNS 记录更新更频繁，需要更少的反弹来找到你要找的域名。你可以使用像 [域名速度基准](https://www.grc.com/dns/benchmark.htm) 这样的工具来检查你的 ISP 的性能(以及你选择的任何新 DNS 服务的性能)。*

*更重要的是，上面列出的服务器(Cloudflare、Google、OpenDNS)提供了网络钓鱼保护和更强的安全性，可以抵御诸如 [DNS 中毒、欺骗和 DDoS 攻击](https://www.calyptix.com/top-threats/3-common-dns-attacks-and-how-to-fight-them/) 之类的攻击。所有列出的 DNS 服务器都提供 DNSSEC 或 DNSCrypt 安全功能，保护您的请求不被窥探、劫持或重定向。*