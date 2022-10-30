# 如何在脸书黑客攻击中生存

> 原文：<https://lifehacker.com/how-to-survive-a-facebook-hack-1825369416>

又来了。Radware 的威胁研究小组 [最近宣布](https://blog.radware.com/security/2018/04/stresspaint-malware-campaign-targeting-facebook-credentials/) 超过 40，000 名脸书用户被骗下载了一个“缓解压力绘画”应用程序，通过一封狡猾的钓鱼邮件，当他们在应用程序中假装绘画时，他们的登录凭据和浏览器 cookies 被盗。更糟糕的是，这种攻击足够聪明，可以避免被典型的反病毒应用程序标记出来。

Watch

那么，在这些情况下，如何保证数据的安全呢？让我们回顾一下:

### 不要下载狗屁应用

说真的。既然你是一个精明的 Lifehacker 读者，当你看到一个类似这样的网站，要求你下载一个听起来有点奇怪的应用程序时，你可能会有很好的蜘蛛侠感觉:

事实上，这是这些钓鱼邮件发送给不太了解的收件人的网站截图。该网站也可以通过谷歌搜索，如果你以某种方式创建了一个足够怪异的查询，导致它出现在你的结果中。

在这两种情况下，恶意软件创建者使用 Unicode 将网站的 URL 显示在电子邮件(或列表)上，看起来更加无辜:aol.net，或者就我而言，picc.com。将鼠标悬停在链接上，或者点击查看地址栏，你会看到很多不同的东西:例如:[【xn—p1aca6f.com】](http://xn--p1aca6f.com/)。

我跑题了。不被恶意软件欺骗的第一条规则是不要下载看起来或听起来完全虚假的东西。我意识到这个建议并不适用于所有人——你不太懂技术的父母，你喜欢点击的孩子，或者你睡着时在键盘和鼠标上走来走去的宠物。

对他们来说，可以考虑使用浏览器扩展或应用程序(如 [OpenDNS](https://support.opendns.com/hc/en-us/articles/227988067-Getting-Started-Blocking-Allowing-Specific-Domains-with-Whitelist-Blacklist) )来 [白名单](http://www.thewindowsclub.com/blacklist-block-websites-browsers-windows) 他们可以访问的少数网站。你甚至可以直接在 [Windows](https://www.bleepingcomputer.com/tutorials/create-an-application-whitelist-policy-in-windows/) 和 [macOS](https://lifehacker.com/use-os-xs-parental-controls-to-encourage-productivity-5713110) 中将应用列入白名单，这可以帮助阻止你的朋友和爱人运行他们不应该运行的应用——从长远来看，这将为他们节省更多压力。

### 但是如果你还是被骗了...

它发生了。如果您后来发现您下载的某些内容可能会将您的脸书凭据暴露给一群黑客或垃圾邮件发送者，您有几个选择。(我们假设你已经删除了恶意软件/用一个 [强力杀毒软件](https://lifehacker.com/the-best-antivirus-app-for-windows-5865356) 和 [恶意软件清除应用](https://lifehacker.com/10-malware-removal-apps-tested-malwarebytes-comes-out-1614046598) / [从 orbit](https://lifehacker.com/how-to-do-a-clean-install-of-windows-10-1720775893) 对你的电脑进行了扫描。)

首先，更改你的脸书密码——这是最简单的。当你使用它的时候，把它变成一个好的、强密码 (或者密码短语)。这不会保护你的数据不被网络共享，但至少其他人不会再以你的身份登录。这是你能做的最好也是最重要的一步。

第二，为您的账户启用 [双因素认证](https://www.facebook.com/settings?tab=security) 。正如 Ars Technica 的 [丹·古丁](https://arstechnica.com/information-technology/2018/04/tens-of-thousands-of-facebook-accounts-compromised-in-days-by-malware/) 指出的，这可能对你最近的恶意软件攻击没有帮助，但它仍然是一项重要的安全措施:

> *“使用多因素身份认证来保护帐户总是一个好主意，但目前还不清楚这种保护是否能防止此次活动中的攻击者访问受损的帐户。因为恶意软件窃取了密码和 cookie，所以 cookie 有可能让攻击者绕过保护。”*

第三，使用同一个页面( [)脸书安全和登录设置页面](https://www.facebook.com/settings?tab=security) )来启用关于未识别登录的警报。然后，点击“登录位置”下的“查看更多”如果您不认识此列表中的任何系统，或者如果您看到某个外国系统的条目，而您昨天没有访问过，那么您已经受到威胁。在这里，滚动到扩展列表的底部，找到“注销所有会话”链接。点击那个。

第四，这是一个让朋友和爱人知道“查看最近来自脸书的邮件”选项的好时机。如果他们收到一封来自社交网络的可疑邮件，他们可以在这一部分检查这是否是来自脸书的真实邮件。我们怀疑脸书会要求别人安装，比如说，一个减压应用程序，但肯定有更多聪明的合法脸书电子邮件的欺骗，可能会说服一个更容易受骗的用户“登录”到一个假的脸书网站。

最后，点击脸书的支付界面，在它的设置页面的左边栏。点击账户设置。如果你曾将信用卡或借记卡输入脸书进行任何支付处理，如应用内购买，如果你不再使用它，请考虑将其移除。如果有人真的进入了你的账户，他们将无法代表你支付任何款项，也无法制作虚假广告来进一步传播恶意软件。