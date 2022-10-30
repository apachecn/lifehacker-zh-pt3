# 当我启动电脑时，为什么我的显示器不打开？

> 原文:[https://life hacker . com/why-wont-my-monitor-turn-on-when-I-start-my-PC-1828881307](https://lifehacker.com/why-wont-my-monitor-turn-on-when-i-start-my-pc-1828881307)

在本周的[Tech 911](https://lifehacker.com/c/tech-911)——解决你所有技术问题或疑问的专栏中——一位 Lifehacker 读者正在处理你在构建全新的桌面系统后可能面临的更令人烦恼的问题之一:有些东西工作不正常。

Watch

我会让罗恩解释:

> *我最近使用组件列表完成了我自己的 PC 构建，在这里找到了*[](https://techbuyersguru.com/1250-quiet-gaming-pc-build)**。我还给它买了* [*这个显示器*](https://www.amazon.com/gp/product/B017EVR2VM/ref=oh_aui_detailpage_o04_s00?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/why-wont-my-monitor-turn-on-when-i-start-my-pc-1828881307&asc_source=&ie=UTF8&psc=1&tag=kinjalifehackerlink-20) *(通过 DisplayPort 线连接)。除了一个小问题，一切似乎都很好:大约有一半时间，当我从关机状态开机时，显示器没有显示，我不得不关机再试一次。据我所知，这似乎是一种随机现象。**

### *失踪显示器的神秘案件*

*当我第一次阅读这封电子邮件时，我的脑海中立即跳转到所有不同的故障诊断技术，您可能想要使用这些技术来隔离这个问题，例如，通过系统地消除原因来缩小潜在的答案。*

*首先，这很可能不是软件问题。如果你的显示器只是在你启动电脑的时候偶尔打开，那么这对于显卡驱动之类的东西来说还为时过早。这并不是说你*不应该*尝试重新安装 [最新的英伟达驱动](https://www.nvidia.com/Download/index.aspx) ，但我不认为这是这里的问题，我会把这个选项放在我的“尝试”列表的较低位置。*

*我认为硬件相关的东西是罪魁祸首。这并不是说你的显示器坏了。事实上，我认为你的显示器工作正常，除了一个触发一些问题的小设置。在我过去作为硬件评测人员的生活中，我曾经使用过华硕 ROG Swift PG279Q，我相信有一个 [one，简单的设置](https://dlcdnets.asus.com/pub/ASUS/LCD%20Monitors/PG279/PG279_English_V1.pdf) 隐藏在它的屏幕显示中，你可以对你的问题负责。*

*调出显示器设置，向下滚动至“系统设置”在那里，你会想要向下滚动*经过*“全部重置”选项，这看起来像是列表上的最后一件事，但不是。您会发现一个名为“显示端口深度睡眠”的设置关掉它，我想你不会再有显示器拒绝开机的问题了。*

*如果你这样做了，你可以尝试更多的事情。你可以拔下两端的 DisplayPort 连接，然后再插回两端，以防连接松动。您可以尝试使用完全不同的 DisplayPort 电缆。切换到 HDMI，看看你是否遇到了同样的问题。切换回来，并确保您的显示器正确选择了 DisplayPort 作为其连接端口——我怀疑它是正确的，但检查一下也无妨。*

*您可以尝试使用前面提到的“全部重置”命令来重置显示器的设置。这也许不能解决问题，但是，这是一个想法。您也可以尝试通过 BIOS 将主板设置重置为出厂默认值。你可以关闭你的系统，取出 [CMOS 电池](https://lifehacker.com/why-do-motherboards-have-batteries-1825773436) ，等待几分钟，然后再插回去，以防一些奇怪的设置导致这些问题。*

*如果您仍然有问题，您可以更进一步:重新拔插您的图形卡(取出并插回)。拔下连接显卡的所有电源线，然后重新插上。重新拔插内存。拔下连接到主板的电源线(粗的 24 针连接器和细的 4 针或 8 针连接器),然后插回。*

*我很难想到此时你还能做什么，但我的直觉是，DisplayPort 深度睡眠设置是你的问题的罪魁祸首。毕竟这是一台全新的 PC。虽然有故障的硬件可能随时发生故障，但我认为这不是问题所在。我认为这种恼人的环境让你感到悲伤。*

**<small>你是否有一个让你夜不能寐的技术问题？厌倦了对您的 Windows 或 Mac 进行故障诊断？寻找可以用来完成特定任务的应用程序、浏览器扩展或实用程序的建议？让我们知道！在下面的评论或者邮件中告诉我们</small>*[*<small></small>*](mailto:david.murphy@lifehacker.com?subject=Tech%20911)<small>*<small>。</small>T15】*</small>*

*<small></small>*