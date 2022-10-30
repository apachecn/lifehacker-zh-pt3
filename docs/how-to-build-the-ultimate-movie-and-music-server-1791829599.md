# 如何构建终极电影和音乐服务器

> 原文:[https://gizmodo . com/how-to-build-the ultimate-movie-and-music-server-1791829599](https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599)

如果你像我一样，你有数百千兆字节的数字媒体文件，从电影、音乐到电视节目，存储在便携式硬盘、旧笔记本电脑和各种 PC 上。如果所有的媒体都可以放在一个地方*并且*可以被你的其他电脑和智能设备轻松访问，那不是很好吗？借助合适的应用和网络连接存储设备，您可以做到这一点。

Watch

### 步骤 1:购买或构建 NAS

要构建自己的终极家庭媒体服务器，你需要某种网络连接存储系统，通常称为 NAS。这基本上是一个迷你电脑，里面有一个硬盘，这将有助于收集你所有的媒体。它连接到您的家庭网络，因此您可以在其他设备上访问该媒体。

您可以从旧电脑和硬盘构建自己的 NAS，也可以购买机箱系统。你选择哪个选项由你决定，但除非你想花很多时间配置设置(你可能会！)或者预算非常紧张，我建议购买现成的 NAS。你买的现成产品不仅更小(这很好)，而且大多数都配有易于使用的软件。

Synology、QNAP 和 Western Digital 等公司都销售存储多个硬盘的 NAS 设备。您需要多少个驱动器取决于您的存储空间和目标。普通用户可能对将存储两个 3.5 英寸硬盘的两舱系统没有问题。您使用什么大小的驱动器由您决定，但要知道大多数系统都要求您在两个位置使用相同大小的驱动器。

我们在 [的朋友 Wirecutter](http://thewirecutter.com/reviews/best-network-attached-storage/) 推荐[QNAP Turbo NAS TS–251](https://www.amazon.com/dp/B00L8GHOQ8?asc_campaign=InlineText&asc_refurl=https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599&asc_source=&tag=kinjagizmodolink-20)作为他们最好的 NAS。亚马逊上的售价为 250 美元，不过内存更大的新版 售价为 340 美元，还有一款[【320 美元 TS–251 a](https://www.amazon.com/TS-251A-personal-direct-display-TS-251A-2G-US/dp/B01JHHGJJ2?asc_campaign=InlineText&asc_refurl=https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599&asc_source=&tag=kinjagizmodolink-20)，它配有遥控器，并针对媒体播放进行了优化。QNAP 251 系列的一个优点是它带有一个 HDMI 端口，这使得它可以非常容易地连接到电视或大显示器上。我个人在 Synology 的 NAS 系统上取得了很多成功，售价 250 美元的 [DS216](https://www.amazon.com/dp/B0185ZU0O2/?asc_campaign=InlineText&asc_refurl=https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599&asc_source=&tag=kinjagizmodolink-20) 非常出色。它不像 QNAP 那么强大，所以对于你的钱来说，你可能更喜欢那个单位，但它绝对值得考虑。

请记住，这些价格不包括硬盘。那要额外付费...

### 第二步:选择你的硬盘

有了机箱后，您需要为 NAS 准备硬盘。无需过多了解 RAID 系统的工作原理，只需知道对于两机架系统(或任何具有多个驱动器的系统)，最好用相同的驱动器填充它。

你不需要得到 NAS 认证的硬盘，从技术上来说，任何 3.5 英寸的台式机硬盘都可以，但根据我的经验，NAS 硬盘往往更好，因为它们被设计为全天候运行。而且，既然您大概希望您放在 NAS 上的数据保持安全，那么多花一点钱买一个 NAS 驱动器也不是一个坏主意。

我喜欢 [西部数位红系列硬盘](https://www.amazon.com/dp/B00EHBERSE/ref=dp_cerb_1?asc_campaign=InlineText&asc_refurl=https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599&asc_source=&tag=kinjagizmodolink-20&th=1) ，但 [希捷铁狼系列](https://www.amazon.com/Seagate-IronWolf-3-5-Inch-Internal-ST4000VN008/dp/B01LOOJBQY/ref=sr_1_5?asc_campaign=InlineText&asc_refurl=https://gizmodo.com/how-to-build-the-ultimate-movie-and-music-server-1791829599&asc_source=&ie=UTF8&keywords=nas+hard+drive&qid=1485878086&s=pc&sr=1-5&tag=kinjagizmodolink-20&th=1) 也获得好评。

我的建议是购买尽可能多的空间，因为一旦您开始将 NAS 用作媒体服务器，您可能会发现自己使用它的次数会超出您的预期。

### 步骤 3:设置和配置您的 NAS

 [https://gizmodo.com/embed/inset/iframe?id=youtube-video-6vrFS0Md0Tk&start=0](https://gizmodo.com/embed/inset/iframe?id=youtube-video-6vrFS0Md0Tk&start=0) 

每个 NAS 的设置过程都是不同的，但是设备附带的说明应该可以帮助您。一般来说，你只需要安装硬盘驱动器(这通常只是意味着连接一根电缆并将其放在外壳中)，将其插入电源，并通过以太网将其连接到路由器。

大多数现代 NAS 系统都可以使用无线 USB 适配器(有些甚至内置了 wi-fi)，但最好直接将其连接到路由器或交换机。别担心，通过软件的配置方式，您的所有无线设备仍将能够远程访问内容。

然后，只需按照 NAS 制造商提供的说明继续设置过程。这通常意味着访问另一台计算机上的网址(除非您想将其连接到本地显示器)。如果你曾经安装过互联网路由器，过程是相似的。

系统可能会询问您希望如何设置 RAID 配置。手册应该给你一个很好的概述你想要什么，但你也可以看看 [这本指南](https://outsourcedatarecovery.com/raid-for-individuals/) 提供了一个很好的概述。

### 第 4 步:传输您的数据

您可能已经有大量文件和数据分散在硬盘、旧电脑和其他设备上。NAS 的伟大之处在于，你可以将所有数据放在那里，然后网络上的每一台计算机都可以访问它。

将数据传输到您的 NAS 会因系统而异，但是一旦您的 NAS 在网络上正确配置，您应该会在 macOS 或 Windows 的文件管理器中看到它。然后，您可以通过 wi-fi(较慢)或以太网(较快)在网络上传输文件。

大多数 NAS 也有 USB 端口，这意味着您可以插入外部硬盘，并使用 NAS 内置的文件管理器以这种方式传输数据。

[QNAP](https://forum.qnap.com/viewtopic.php?t=103399) 和 [Synology](https://www.synology.com/en-us/knowledgebase/DSM/help/DSM/FileBrowser/copymove) 如果你搞不清楚的话都有指南。

### 第五步:安装应用程序

一旦你设置好了 NAS，就该安装应用程序让它唱歌了。应用程序真的会将 NAS 从一个美化的时间胶囊变成某种东西，可以让您非常容易地在许多不同的设备上欣赏您的许多文件。

安装应用程序的方法会因 NAS 而异，但一般来说，您可以使用包管理器(就像应用程序商店一样)来挑选您想要的应用程序。

我们谈论的大多数应用程序都在 QNAP 和 Synology 应用程序商店中，所以你可以搜索这些解决方案并直接从软件中安装它们。

这是你最想做的事情的概要。

#### **使用丛**创建故障媒体服务器

使用 NAS 的最佳理由之一是作为一种拥有自己的音乐、电影和照片媒体服务器的方式。 [丛](http://www.gizmodo.com/tag/plex#_ga=1.147310135.1242900246.1450837061) 很容易就是最佳方案。您可以在 NAS 上安装和配置 Plex 介质服务器。配置完成后，Plex 将获取您的 NAS(甚至整个网络)上的所有内容，并使其易于提供和播放。

Plex 在 QNAP 和 Synology 的应用商店中都有，但有时版本可能会过时。如果您想手动安装应用程序，您可以从 Plex 的网站下载文件。我们已经运行了一个 [少数指南](http://fieldguide.gizmodo.com/how-to-build-your-own-private-netflix-1787437400#_ga=1.226912091.73804277.1472045787) 关于如何让 [最大限度地利用 Plex](http://fieldguide.gizmodo.com/6-reasons-to-use-plex-to-create-your-own-personal-netfl-1705440916#_ga=1.226912091.73804277.1472045787) 。

Plex 是最容易设置的媒体服务器，它拥有几乎所有已知平台的应用程序，这意味着你可以从几乎任何设备上轻松访问内容——从你的 Android 手机到你的 iPad，再到连接到电视的机顶盒。

丛是免费的，但如果你支付丛通行证(45 美元一年)，你甚至可以远程访问你的所有内容。没错，你可以在办公室一边看《办公室》的老剧集一边放松。你可以看*飞机！*从飞机上。

#### 使用 Sonarr 自动获取内容

好了，您已经在 NAS 上安装了 Plex，现在您可能需要一些附加内容。很明显，你可以购买或 [抓取你的媒体](http://lifehacker.com/the-hassle-free-guide-to-ripping-your-blu-ray-collectio-5559007) 到你的系统，但是有一些应用程序可以让获取额外内容的过程变得更好。

一如既往，遵循您所在国家或地区的版权法。咳咳。

有一个很棒的应用程序叫做 [Sonarr](https://sonarr.tv/) ，它可以让你轻松下载任何你想要的电视节目。它甚至会在每集播出时自动继续下载。Sonarr 有 [安装包](https://github.com/Sonarr/Sonarr/wiki/Installation) 用于包括 QNAP 和 Synology 在内的主要 NAS 平台。安装该服务后，您可以添加不同的信号源来监控您想要的电视节目。然后，这些内容可以自动摄取到 Plex 中，这样您就可以在自己的时间观看电视节目。如果 Sonarr 不是你的菜，一个类似的名为 [Sickbeard](http://sickbeard.com/install.html) 的应用程序也是如此。

#### BitTorrent 客户端

BitTorrent 很棒，但在 PC 上保持持续连接可能是一件痛苦的事情。您可以在 NAS 上设置自己的 BitTorrent 客户端。Synology 和 QNAP 都提供了一款名为下载站的应用，用户可以从 BitTorrent、FTP、NZB(新闻组)等网站下载文件。

当你做其他事情时，该应用程序可以继续在后台运行，因此你可以下载新内容并上传给其他人，同时访问文件或流媒体到你的电视。

#### 备份解决方案

除了存储您的媒体，您还可以使用所有硬盘空间来备份您的文件。使用 NAS 的最佳方式之一是作为您家中所有其他文件的备份解决方案。

如果你是 Mac 用户，你甚至可以使用你的 [Synology](https://www.synology.com/en-us/knowledgebase/DSM/tutorial/Backup_Restore/How_to_back_up_files_from_Mac_to_Synology_NAS_with_Time_Machine) 或 [QNAP 设备](https://www.qnap.com/en-us/tutorial/con_show.php?op=showone&cid=58) 和时间机器。这意味着你所有的数据都将被安全地存储起来，以防你的主机发生故障。

如果你使用 Windows，Synology 和 [QNAP](https://www.qnap.com/en-us/family_apply_v2/con_show.php?op=showone&cid=3) 都有备份你的机器的指南。

### 第六步:开心

设置需要一些时间，但是一旦您配置了 NAS，它就应该像设备一样运行了。随意添加新的应用程序——也许你想运行自己的网络服务器，甚至《我的世界》服务器——然后到处玩玩。