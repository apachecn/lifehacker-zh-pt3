# 勒索软件攻击还没有结束，以下是保护自己的方法

> 原文:[https://life hacker . com/the-ransomware-attack-not-over-heres-how-to-protect-yo-1795219005](https://lifehacker.com/the-ransomware-attack-isnt-over-heres-how-to-protect-yo-1795219005)

如果你的电脑运行的是微软视窗系统，你需要马上采取这些步骤。

Watch

原因如下:如果你还没听说，黑客利用旧的微软 Windows 服务器中的一个漏洞，在周五利用勒索软件(一种恶意软件，将你的电脑作为人质索要赎金)和从美国国家安全局(NSA)偷来的黑客工具 [实施了一次大规模的全球网络攻击](http://www.cnbc.com/2017/05/14/cyber-attack-hits-200000-in-at-least-150-countries-europol.html) 。大规模攻击让受害者被锁在他们的电脑外面，并承诺如果支付 300 美元的数字货币比特币，就可以恢复访问——如果不满足赎金，就威胁要销毁文件。

迄今为止，在超过 150 个国家至少有 20 万台电脑被感染，从企业、政府到学术机构、医院和普通人都受到了影响。

## 它是如何工作的

“ [像蠕虫](https://blogs.technet.microsoft.com/mmpc/2017/05/12/wannacrypt-ransomware-worm-targets-out-of-date-systems/) 一样传播的恶意软件，通过包含压缩、加密文件的网络钓鱼电子邮件传播。由于文件是加密的，安全系统无法识别名为 Wanna Decryptor 的勒索软件，直到它被下载。WannaCry 勒索软件的下一代版本 Wanna Decryptor 一旦下载了充满恶意软件的文件，就可以访问给定的设备:然后加密数据，锁定系统并索要赎金。

勒索软件通常不会这么快见效。但是由于一个被盗的美国国家安全局网络武器名为 EternalBlue，上个月由一个被称为“影子经纪人”的黑客组织公开了，该恶意软件通过利用微软 Windows 服务器的安全漏洞迅速传播。

## 用户需要做什么

简而言之:确保你的微软视窗服务器是最新的。微软 [在 3 月中旬发布了一个补丁](https://technet.microsoft.com/en-us/library/security/ms17-010.aspx) 修复了 Windows 7 和其他支持版本 Windows 的漏洞:Vista、Server 2008、Server 2008 R2、8.1、Server 2012、**T5、RT 8.1、10、Server 2012 R2 和 Server 2016。但是那些没有应用软件更新的人仍然暴露在黑客攻击之下。**

鉴于这次攻击， [微软推出了补丁](https://blogs.technet.microsoft.com/msrc/2017/05/12/customer-guidance-for-wannacrypt-attacks/) 来保护 Windows XP、Windows 8 和 Windows Server 2003 等公司“不再得到主流支持”的旧版本 Windows。那些运行 Windows 10 的软件没问题，因为它们的软件不容易受到这种特定的网络攻击。可能受影响的设备是 Windows 7 和 Windows Server 2008 以及更早的操作系统。

微软建议用户升级到 [Windows 10](https://www.microsoft.com/en-us/windows/windows-10-upgrade) 并安装安全更新 [MS17-010](https://technet.microsoft.com/en-us/library/security/ms17-010.aspx) 。随着 *1.243.297.0* 更新，[Windows Defender anti virus](https://technet.microsoft.com/en-us/itpro/windows/keep-secure/windows-defender-in-windows-10)将恶意软件检测为 Ransom:Win32/WannaCrypt。该公司还为企业推荐了 [设备卫士](https://technet.microsoft.com/itpro/windows/keep-secure/device-guard-deployment-guide) ，为拦截携带恶意软件的电子邮件推荐了 [Office 365 高级威胁防护](https://blogs.office.com/2015/04/08/introducing-exchange-online-advanced-threat-protection/) 。

美国计算机应急准备小组(CERT) [发布建议](https://www.us-cert.gov/security-publications/Ransomware) 用户如何最好地保护自己免受最近 WannaCry 勒索软件的威胁。除了“特别警惕压缩或 ZIP 文件附件”，CERT 建议在直接点击电子邮件中的链接时要小心，即使发件人是你认识的人。他们建议尝试独立验证网址。

## 如果不采取保护措施会怎么样？

即使您没有主动从网络钓鱼电子邮件下载文件，您的设备也可能面临风险——勒索软件还会通过网络上的文件共享系统传播。微软 [解释](https://blogs.technet.microsoft.com/mmpc/2017/05/12/wannacrypt-ransomware-worm-targets-out-of-date-systems/) 称，该勒索软件类似蠕虫的功能会感染“本地网络中未打补丁的 Windows 机器”，“对互联网 IP 地址执行大规模扫描，以找到并感染其他易受攻击的计算机”

受感染的设备会发现桌面背景图像被一条消息取代，要求用户按照指示操作，直到他们到达勒索屏幕。这里有两个计时器——一个显示文件被删除前的剩余时间，另一个显示赎金从 300 美元开始增加前的时间。

在这一点上，人们有两个选择:支付并希望他们的设备被恢复，或与他们的电脑内容分道扬镳。美国政府 [建议](https://www.fbi.gov/news/stories/incidents-of-ransomware-on-the-rise) 不要支付赎金，因为支付金钱并不保证数据会被恢复，向网络犯罪分子屈服可能会鼓励未来的攻击。但是，当你自己的文件被劫持时，说起来容易做起来难。

## 勒索软件不是被制止了吗？

周五晚上，由于无意中发现了恶意软件代码中的“”终止开关，疫情有所减缓。这一发现是由一名来自英国的网络安全研究人员发现的，他自称是 [MalwareTech](https://twitter.com/MalwareTechBlog) 。

虽然这阻止了恶意软件的传播，但攻击背后的策划者可以很容易地修改代码，让球再次滚动。自周五以来， [已经检测到该恶意软件的两个新变种](http://www.nbcnews.com/news/us-news/blockbuster-wannacry-malware-could-just-be-getting-started-experts-n759356) 。因此，人们保护自己的电脑势在必行。

## 勒索软件有多普遍？

比你想象的更常见。[](http://www.npr.org/sections/thetwo-way/2017/05/14/528355526/repercussions-continue-from-global-ransomware-attack)*报道称，去年*40%的垃圾邮件*包含勒索附件。与勒索软件相关的勒索行业正在发展壮大。2015 年，勒索软件受害者报告的年度总成本(如赎金、技术支持、安全软件)为 2400 万美元， [*路透社*](http://www.reuters.com/article/us-usa-cyber-ransomware-idUSKCN0X917X) 去年报告。仅在 2016 年的前三个月，报告的费用就已经达到 2.09 亿美元。*

*一般明智的建议: [定期远程备份你的文件](http://abcnews.go.com/US/simple-things-protect-ransomware-attacks/story?id=47410339) 。这样，当您的设备受到威胁时，您将永远不会屈服于勒索请求。当然，始终保持计算机软件的最新状态。*