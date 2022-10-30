# 安装树莓派的最新指南

> 原文：<https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054>

所以，你终于拿起了一个树莓，它正坐在你的桌子上，等着你用它做一些令人敬畏的事情。好消息是，设置它是愚蠢的-现在很容易，不到 30 分钟，你就可以在你的 35 美元的小电脑上进行黑客攻击。

Watch

### 什么是树莓派？

Raspberry Pi 是一款 35 美元的小型电脑，可以放在你的手掌里。它运行 Linux 以及一些其他低功耗操作系统。它是由 [树莓派基金会](https://www.raspberrypi.org/) 创建的，目的是让世界各地的孩子们都能使用电脑，并教他们编码。自最初推出以来，它已经成为想要制作自己的电子项目的 DIY 者最受欢迎的电脑，从 [媒体中心](http://lifehacker.com/turn-a-raspberry-pi-into-an-xbmc-media-center-in-under-5929913) 到 [视频游戏系统](http://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) 。树莓派也有自己的官方操作系统， [Raspbian](https://www.raspbian.org/) 。其他操作系统也存在，但 [它们大多是为特定项目](https://lifehacker.com/the-best-operating-systems-for-your-raspberry-pi-projec-1774669829) 而制作的。Raspbian 是大多数人想要开始使用的操作系统，所以我们将在这里详细介绍如何安装它。

自 2012 年推出以来，树莓派已经经历了几次迭代。最新版本是 [**树莓派 3 型**](https://lifehacker.com/the-raspberry-pi-3-adds-built-in-wi-fi-and-bluetooth-g-1761317416)T5。只需 35 美元，你就可以买到一台无外壳电脑，包括一个 HDMI 输出、多达四个 USB 端口、Wi-Fi 和蓝牙。

Raspberry Pi Model 3 并不是目前唯一可用的版本。还有 [**树莓派 A+**](http://lifehacker.com/raspberry-pi-model-a-is-smaller-thinner-and-just-20-1656837626) 型号，更小，只有 20 美元，只有一个 USB 接口。这款 [**树莓派 Zero**](http://lifehacker.com/the-raspberry-pi-zero-is-a-5-computer-the-size-of-a-st-1744253282) 售价仅为 5 美元，大约相当于一块电池的大小，根本不包括普通的 USB 端口。这两种主板都非常适合特定的项目，但对于大多数人来说，我们推荐全尺寸的 Raspberry Pi Model 3，所以这是我们在本指南中坚持的。

#### 你需要什么

*   [**覆盆子**](https://www.amazon.com/Raspberry-Pi-RASP-PI-3-Model-Motherboard/dp/B01CD5VC92/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054&asc_source=&ie=UTF8&keywords=raspberry pi model 3&qid=1465403777&sr=8-1&tag=kinjalifehackerlink-20) :既然我们推荐了 Model 3，下面我们就来给大家演示一下如何设置。
*   HDMI 电视或显示器:你需要将你的 Raspberry Pi 连接到显示器上，这意味着你需要某种支持 HDMI 的屏幕。如果你不想把一个完整的显示器献给 Pi，你可以选择 [和](http://lifehacker.com/the-kano-screen-kit-is-a-fun-to-build-compact-display-1750101508) 这几款紧凑型显示器。还有一些使用显示器的方法，我们将在这篇文章的最后讨论。
*   **USB 键盘和鼠标**:为了控制你的 Pi，你需要一个键盘和鼠标。在这一点上，几乎任何 USB 键盘和鼠标都可以工作。
*   **一个 8GB 的 MicroSD 卡和读卡器**:你把 Raspberry Pi 的操作系统安装在一个 MicroSD 卡上，而不是硬盘。你至少需要一张 8GB 的卡。 [三星 EVO+10 级卡像这种](https://www.amazon.com/Samsung-EVO-Plus-Adapter-MB-MC32DA/dp/B012DT8OJ4?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054&asc_source=&ie=UTF8&keywords=Samsung+Evo++32+GB&qid=1449161771&rawdata=[r|https://www.google.com/[t|link[p|1745961206[a|B012DT8OJ4[au|5716493564230329059[b|lifehacker&ref_=sr_1_3&sr=8-3&tag=kinjalifehackerlink-20) ($12.95) [最好](http://lifehacker.com/microsd-card-quality-makes-a-massive-difference-in-rasp-1745961206) 。如果你的电脑没有读卡器，像这种(6.75 美元)的便宜 [就可以了。](http://www.amazon.com/Transcend-Information-Card-Reader-TS-RDF5K/dp/B009D79VH4?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054&asc_source=&ie=UTF8&keywords=micro sd card reader&qid=1465427763&ref_=sr_1_1&s=electronics&sr=1-1&tag=kinjalifehackerlink-20)
*   **电源**:树莓派由微型 USB 供电，很像你手机上用的那种。由于 Pi 3 有四个 USB 端口，所以最好使用至少可以提供 2.5A 果汁的好电源。 [这款](https://www.amazon.com/CanaKit-Raspberry-Supply-Adapter-Charger/dp/B00MARDJZ4?*Version*=1&*entries*=0&asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054&asc_source=&ie=UTF8&tag=kinjalifehackerlink-20)(9.99 美元)就能做到这一点。

一旦你收集好所有的配件，就该开始安装了。

### 第一步:用 NOOBs 把 Raspbian 安装到你的 SD 卡上

首先，你得把拉斯扁放到 SD 卡上。这意味着您需要将操作系统下载到另一台计算机上，并使用 SD 读卡器将其传输到 SD 卡上。你有两种方法做这件事。 [你可以手动安装 Raspbian](https://www.raspberrypi.org/documentation/installation/installing-images/)，这需要命令行诀窍或外部软件，或者你可以下载并安装 [NOOBs](https://www.raspberrypi.org/downloads/noobs/) ，它代表“新的开箱即用软件”这是一个简单得多的过程，我们将在这里使用。

1.  将您的 SD 卡放入电脑或 SD 读卡器。
2.  下载 [NOOBs](https://www.raspberrypi.org/downloads/noobs/) 。选择“离线和网络安装”选项。这个版本在下载中包含了 Raspbian。
3.  您可能需要将 SD 卡格式化为 FAT。你可以 [在](https://www.raspberrypi.org/documentation/installation/noobs.md) 这里找到 Windows 和 Mac 的操作指南。
4.  解压缩 ZIP 文件，并将文件夹的全部内容复制到 SD 卡上。一旦完成，弹出您的 SD 卡，并将其插入树莓派。

就是这样。您将在 Raspberry Pi 本身上完成剩余的工作，这意味着是时候将它连接到您的显示器上了。

### 第二步:挂上你的树莓派

将你所有的设备连接到 Raspberry Pi 非常简单，但是你要按照特定的顺序来做，这样它就可以在启动时识别你所有的设备。首先，将您的 HDMI 电缆连接到您的 Raspberry Pi 和显示器，然后连接您的 USB 设备。如果您使用以太网电缆连接到您的路由器，请继续连接。

最后，一旦所有的东西都连接好了，继续插入你的电源适配器。Raspberry Pi 没有电源开关，所以一旦你连接电源适配器，它就会自己打开。

### 第三步:设置 Raspbian

当你第一次启动 NOOBs 时，需要几分钟来格式化 SD 卡和设置一些东西，所以让它做它自己的事情吧。最终，你会看到一个要求你安装操作系统的屏幕。这个过程非常简单:

1.  在屏幕底部，选择您所在地区的语言和键盘布局。
2.  点按 Raspbian 旁边的复选框，然后点按“安装”。

现在，让 NOOBs 运行安装过程，这可能需要 10 或 20 分钟。当它完成时，它将重新启动并把你直接送到 Raspbian 桌面，在那里你可以配置其他的东西。

### 第四步:配置你的树莓派

恭喜你，你的树莓派基本上已经准备好了。在 Raspbian 中，你会看到一个开始菜单，在那里你可以选择应用程序，打开一个文件浏览器，以及你期望从操作系统中得到的一切。不过首先，你可能需要设置你的 Wi-Fi 连接和任何你想使用的蓝牙设备。

#### 连接到您的 Wi-Fi 网络

在 Raspbian 中，连接到 Wi-Fi 网络的工作方式与在任何现代操作系统中一样。

1.  点按右上角的网络图标(有两台电脑的那个)。
2.  选择您的 Wi-Fi 网络名称，然后输入您的密码。

好了，你现在已经连接到 Wi-Fi 了。这在命令行和图形界面中都有效，所以您只需要设置一次。如果你有一个旧的 Pi 并且你正在使用一个 Wi-Fi 适配器 [像这个](http://www.amazon.com/Raspberry-Pi-WIFI-Adapter-Dongle/dp/B009FA2UYK?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054&asc_source=&tag=kinjalifehackerlink-20) ，过程是相同的。

#### 连接蓝牙设备

如果你有蓝牙设备，比如鼠标或键盘，你想和你的 Raspberry Pi 一起使用，你需要把它们和你的 Pi 配对。这根据您的设备而有所不同，但这是一个足够简单的过程:

1.  单击右上角的蓝牙图标。
2.  点按“添加设备”
3.  找到您想要配对的设备，点击它，然后按照屏幕上的指示进行配对。

这就是全部了，现在你可以开始和拉斯扁玩了。继续点击并打开你想要的任何东西，如果有任何错误，你搞砸了什么，只需按照上述过程重新安装 Raspbian。

### 远程连接到您的树莓 Pi

虽然 Raspberry Pi 的价格可能只有 35 美元，但需要 HDMI 显示器和 USB 键盘和鼠标的额外要求使成本略有增加。幸运的是，您有办法远程连接到 Pi。如果你家里只有一台笔记本电脑，或者没有显示器，这就特别有用。这两个都不是必须的，但是如果你需要的话，知道它们是很好的。

*   [**通过 SSH 连接命令行**](https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md) :你可以在任何电脑上使用 SSH 连接到你的树莓派的命令行界面。虽然你不会得到一个图形界面，但你可以从另一台计算机上的终端应用程序中运行任何类型的命令，它将在 Raspberry Pi 上执行。如果您正在进行一个不需要屏幕的项目，这是一个不用显示器、键盘或鼠标连接到您的 Raspberry Pi 的好方法。
*   [**用 VNC 把你家的电脑当成远程屏幕**](https://www.raspberrypi.org/documentation/remote-access/vnc/) :如果你确实需要那个图形界面，可以用 VNC(虚拟网络计算)来获得。你会在台式电脑的一个窗口中看到 Raspberry Pi 的桌面，你可以像坐在 Pi 前面一样控制它。如果您只有一台笔记本电脑或一体式台式机，这是远程使用您的 Pi 的一种方式。它不是很适合日常使用，因为它有点慢，但如果你只是需要设置一些东西，而不想购买额外的配件，VNC 是一种方式。

远程连接和控制您的 Raspberry Pi 是一个非常有用的特性，因此您可能希望在某个时候熟悉这两种远程连接方法。

### 用一些我们最喜欢的树莓 Pi 项目来更进一步

设置和安装 Raspbian 只是使用 Raspberry Pi 的第一步。一旦你完成了这些，是时候真正开始挖掘它，做一些新的东西了。以下是一些我们最喜欢的项目和指南:

*   [复古游戏机](http://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192)
*   [初学者命令行入门](http://lifehacker.com/a-command-line-primer-for-beginners-5633909)
*   [媒体中心](http://lifehacker.com/turn-a-raspberry-pi-into-an-xbmc-media-center-in-under-5929913)
*   [带卡莉 Linux 的便携式黑客站](http://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918)
*   [动画 GIF 相框](http://lifehacker.com/make-an-animated-gif-photo-frame-with-a-raspberry-pi-1658839211)
*   [便携式电脑](http://lifehacker.com/build-a-nintendo-ds-sized-portable-raspberry-pi-1767147400)
*   [Alexa 设备](http://lifehacker.com/amazon-has-an-official-guide-for-building-your-own-alex-1766852717)
*   [魔镜](http://lifehacker.com/build-a-magic-mirror-with-a-raspberry-pi-and-an-old-mon-1750468358)

我们已经展示了无数其他的 Raspberry Pi 项目，所以如果你正在寻找使用你的 Pi 做什么的灵感，请继续在 [Raspberry Pi 标签页](http://lifehacker.com/tag/raspberry-pi) 上挖掘。

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=1691368805,1618224502,5978871&title=Eat More Pi)