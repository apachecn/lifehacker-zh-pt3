# 更新你的 Tor 浏览器，防止它泄露你的真实 IP 地址

> 原文：<https://lifehacker.com/get-tor-s-browser-update-to-stop-leaking-your-real-ip-a-1820190316>

某些注重隐私的 [Tor 网络浏览器](https://lifehacker.com/what-is-tor-and-should-i-use-it-1527891029) 的用户应该下载 [该应用程序的最新更新](https://blog.torproject.org/tor-browser-709-released) ，该更新添加了一个临时补丁，以防止浏览器泄露身份信息，即 IP 地址。发现该漏洞的安全研究公司命名为 [的 TorMoil 漏洞，我们称之为](https://www.wearesegment.com/news/the-tormoil-bug-torbrowser-critical-security-vulnerability/) 段，它可以利用浏览器中的一个缺陷来发现用户的真实 IP 地址，从而在匿名浏览器点击特定类型的链接时将其暴露。

Watch

### **你的真实 IP 可能会被泄露**

IP 地址泄露问题只影响 Mac 和 Linux 设备上的 Tor 浏览器(Windows 和 Tails Tor 用户目前是安全的)。We Are Segment 首席执行官 Filippo Cavallarin 认为这个问题是 Tor 浏览器(基于 Firefox 版本构建)处理以“file://”处理程序开头的链接的方式中的一个错误。为什么 Windows 或 Tails Tor 用户不受影响还不清楚，但 Cavallarin 计划在实施适当的修复后分享关于该缺陷的更多细节。Tor 处理 http://和 https://链接的方法是，通过 Tor 的志愿者运营的虚拟隧道网络发送流量，使其匿名。点击 file:// URL 将允许操作系统直接连接到远程主机，暴露用户的 IP 地址，而不是通过适当的注重隐私的服务器进行路由。

### **现在更新，但期待下一次更新**

最新更新 Tor 浏览器 7.0.9 修复了 TorMoil bug，防止你选择文件://链接时 IP 地址泄露。然而，根据 Tor 的说法，您的浏览器可能会以不同的方式处理这些文件，直到采取适当的修复措施:

> “我们部署的修复只是阻止泄漏的变通办法。因此，浏览器中的导航文件://URL 可能不再像预期的那样工作。特别是在 URL 栏中输入 file:// URLs 并点击产生的链接会被破坏。在新标签页或新窗口中打开它们也不起作用。解决这些问题的方法是将链接拖到地址栏或选项卡上。

简而言之，你需要开始拖动 file://链接到地址栏或标签，而不是简单地点击它们。无论您是否经常点击 file:// links，您都应该将您的 Tor 浏览器更新到最新的稳定版本，以防止您自己成为暴露身份漏洞的潜在受害者。

[关键 Tor 漏洞泄露用户真实 IP 地址—现在更新](https://arstechnica.com/information-technology/2017/11/critical-tor-flaw-leaks-users-real-ip-address-update-now/) | Ars Technica