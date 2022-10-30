# 幽灵和熔毁补丁是怎么回事？

> 原文:[https://life hacker . com/what-going-with the-spectre-and-meltdown-patches-1822128503](https://lifehacker.com/whats-going-on-with-the-spectre-and-meltdown-patches-1822128503)

本月早些时候，计算机安全部门在互联网上投下了一枚重磅炸弹。追溯到 1995 年的一对名为 [Spectre 和 Meltdown](https://lifehacker.com/how-to-protect-yourself-from-meltdown-and-spectre-the-1821781392) 的漏洞使各种电脑、智能手机和互联网浏览器面临风险。

Watch

从那以后，像微软和苹果这样的公司，以及像英特尔和 AMD 这样的芯片制造商，一直在竞相发布补丁，但这并不是一个最顺利的过程。一个多星期后，修复这些漏洞的工作还远远没有完成。这里有一个你需要知道的关于幽灵和熔毁补丁状态的纲要。

### Spectre 和 Meltdown 是什么？

如果您仍然不清楚这些漏洞实际上做了什么，这里有一个简单的解释。

Spectre 和 Meltdown 都依赖于一种叫做“推测执行”的东西，即当你的计算机试图猜测你下一步要做什么，以便它可以更快地执行该任务。由于这种数据的存储方式，它产生了一个漏洞，黑客可以访问您计算机上的其他私人信息。

Meltdown 主要影响英特尔处理器，它为包括苹果 MacBook 系列在内的大量计算机提供动力。Spectre 实际上是指两个独立的漏洞，可以影响英特尔、AMD 和 ARM 的芯片。这包括台式电脑和智能手机。

### 修补程序的当前状态

在很大程度上，像谷歌、微软和苹果这样的大公司能够在这些漏洞被公开宣布之前提前摆脱它们。苹果早在 12 月就发布了 macOS 10.13.12 和 iOS 11.2 的补丁。本月早些时候，苹果还为其 Safari 浏览器打了一个 [新更新](https://support.apple.com/en-us/HT208403) 。所以只要你运行最新的苹果软件，你应该是安全的。

微软的努力并不顺利。在一些电脑停止工作后，该公司实际上被迫召回了 的一些版本的补丁，包括 AMD 芯片的补丁。

从好的方面来看，微软已经修补了其 Internet Explorer 和 Microsoft Edge 浏览器，该公司表示，Windows 10 比 Windows 8.1 或 7 更安全，不会受到 Spectre 和 Meltdown 的影响。所以，如果你还没有升级你的操作系统，现在可能是时候了。

谷歌还发布了一个名为 [Retpoline](https://support.google.com/faqs/answer/7625886) 的 Spectre 补丁，该公司称其 Chrome 浏览器的补丁将于 1 月 23 日 发布。同时，公司建议开启 [现场隔离](https://support.google.com/chrome/answer/7623121?hl=en-GB) 作为权宜之计。至于 Android，谷歌声称其最新版本的软件对 Spectre 是安全的，但如果你的设备太旧而无法获得更新，你基本上只能靠自己了。

最后，如果你使用的是火狐浏览器，有一个 [补丁供你下载](https://www.mozilla.org/en-US/security/advisories/mfsa2018-01/) ，尽管该公司也建议 [启用第一方隔离](https://www.ghacks.net/2017/11/22/how-to-enable-first-party-isolation-in-firefox/) 以获得额外保护。

### 需要注意什么

如果你仍然在等待一个补丁来保护你免受幽灵和熔毁，有几件事要注意。

一些黑客已经在利用这种情况传播虚假更新，实际上是在你的电脑上安装恶意软件。这已经在德国 发生了，伪造的电子邮件看起来像是来自政府机构。所以不要下载任何补丁，除非它们直接来自你信任的公司，如微软或英特尔。

Ars Technica 还警告说，研究人员正危险地接近将 Spectre 和 Meltdown 武器化，这意味着黑客可能也很接近了。因此，如果你还在等待补丁，请留意任何官方更新，以免为时过晚。