# 如何用一个树莓派和 Kali Linux 构建一个便携式黑客站

> 原文：<https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918>

[、破解 Wi-Fi 密码](http://lifehacker.com/how-to-crack-a-wi-fi-password-5953047) 、 [、欺骗账户](http://lifehacker.com/how-to-tap-your-network-and-see-everything-that-happens-1649292940#_ga=1.63072039.968941705.1436971740) 和 [测试网络](http://lifehacker.com/know-your-network-the-complete-guide-5833254) 是否有漏洞都很有趣，但如果你想在路上表演，你需要一个方便携带的装备。输入 [卡莉 Linux](http://www.kali.org/) 和 [树莓派](https://www.raspberrypi.org/) 。

Watch

*这篇文章是我们 Lifehacker 的* [*邪恶周*](https://lifehacker.com/welcome-to-lifehackers-sixth-annual-evil-week-1738276927) *系列的一部分，在这里我们看到了做事的阴暗面。有时邪恶是正当的，而其他时候，知道邪恶意味着知道如何打败它。想要更多吗？查看我们的* [*恶周标签页*](http://lifehacker.com/tag/evil-week#_ga=1.105669515.968941705.1436971740) *。*

Kali Linux 是 [为网络渗透测试](https://lifehacker.com/linux-security-distros-compared-tails-vs-kali-vs-qub-1658139404) 而打造的操作系统。你可以在你的笔记本电脑上运行它来破解附近的 Wi-Fi 密码，欺骗网络，测试蓝牙漏洞，以及许多其他事情。记住，利用这些知识侵入受保护的网络可能会让你被捕并被控重罪——可能是违反计算机安全法的联邦指控。你应该把这些知识用于好的方面，用于你自己的学习，并且只玩你控制的网络。在使用 之前，我们已经非常广泛地讨论了使用 [Kali Linux，所以我们不会在这里详细讨论，但是请查看我们的](http://lifehacker.com/behind-the-app-the-story-of-kali-linux-1666168491#_ga=1.261824013.1055861349.1441835238) [指南，了解您可以使用它做的一切](https://lifehacker.com/how-to-hack-your-own-network-and-beef-up-its-security-w-1649785071) 。所有这些都适用于我们将在这里构建的 Raspberry Pi 版本。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled How to Build a Portable Hacking Station with a Raspberry Pi and Kali Linux](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-to-hack-your-own-network-and-beef-up-its-security-w-1649785071) [###### 如何利用 Kali Linux 入侵您自己的网络并增强其安全性](https://lifehacker.com/how-to-hack-your-own-network-and-beef-up-its-security-w-1649785071) 

Kali Linux 是一个注重安全性的操作系统，您可以在任何地方从 CD 或 USB 驱动器上运行。…

[Read more](https://lifehacker.com/how-to-hack-your-own-network-and-beef-up-its-security-w-1649785071)</aside>

Raspberry Pi 是一款小型的信用卡大小的电脑，使用起来不需要太多电力。当你把 Raspberry Pi 和 Kali Linux 结合在一起时，你就得到一台超级便携的网络测试机，你可以把它带到任何地方。在本指南中，我们将向您展示如何让 Kali 通过触摸屏在 Raspberry Pi 上运行。这样，您永远不需要在您的主计算机上安装 Kali Linux。

### 你需要什么

*   树莓派( [型号 B/B+](http://www.amazon.com/Raspberry-Pi-Model-512MB-Computer/dp/B00LPESRUK/ref=sr_1_4?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&ie=UTF8&keywords=raspberry pi b+&qid=1446050008&s=pc&sr=1-4&tag=kinjalifehackerlink-20) 或 [2](http://www.amazon.com/Raspberry-Pi-Model-Project-Board/dp/B00T2U7R7I/ref=sr_1_4?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&ie=UTF8&keywords=raspberry pi 2&qid=1446050021&s=pc&sr=1-4&tag=kinjalifehackerlink-20) )，然而，树莓派 2 需要一些额外的安装步骤，所以如果你不想经历这些，就坚持使用型号 B+
*   一个电池组( [任何这些为智能手机打造的带 USB 端口的外部 5V 电池](http://lifehacker.com/five-best-external-battery-packs-509802431) 都应该工作， [不过如果你感兴趣还有更优雅的解决方案](https://learn.adafruit.com/touch-pi-portable-raspberry-pi) )
*   一张 [Wi-Fi 卡](http://www.amazon.com/Edimax-EW-7811Un-150Mbps-Raspberry-Supports/dp/B003MTTJOY/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&ie=UTF8&keywords=raspberry pi wi-fi card&qid=1446054043&sr=8-2&tag=kinjalifehackerlink-20)
*   一张 [8 GB SD 卡](http://www.amazon.com/SanDisk-Memory-Adapter--SDSDQUAN-008G-G4A-Version/dp/B00M55C0VU/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&ie=UTF8&keywords=8gb micro sd&qid=1446054060&sr=8-1&tag=kinjalifehackerlink-20)
*   [一个 PiTFT 触摸屏](https://www.adafruit.com/products/2423) ( **更新:**这篇文章的一个旧版本 [指向了这个屏幕](http://www.amazon.com/Adafruit-83-15684-PiTFT-Mini-LCD/dp/B00JFJJTM2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&tag=kinjalifehackerlink-20) ，它仍然工作，但不适合与树莓 Pi 2 或 Pi 的其他新版本齐平)
*   一个盒子(可选，但如果你随身带着树莓派，它会很有用。 [这个来自 Adafruit 的案例是为了打包放入 PiTFT](https://www.adafruit.com/products/1892) 而 Model B 是一个很好的选择，如果那是你正在使用的模型的话。)
*   键盘(我喜欢使用带触摸板的小无线键盘 [，就像这个](http://www.amazon.com/gp/product/B00556NMMW/ref=oh_aui_detailpage_o04_s00?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-portable-hacking-station-with-a-raspberr-1739297918&asc_source=&ie=UTF8&psc=1&rawdata=[r|https://www.google.com/[t|link[p|1658839211[a|B00556NMMW[au|5716493564230329059&tag=kinjalifehackerlink-20) ，这样它就能装进一个小包里。)
*   台式计算机(用于执行初始安装)

### 第一步:在树莓派上安装 Kali

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-aTQjuDfEGWc&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-aTQjuDfEGWc&start=0) 

在我们做任何事情之前，您需要下载并安装用于 Raspberry Pi 的 Kali Linux 映像的触摸屏构建。这就像安装任何其他的 Raspberry Pi 操作系统一样，我们已经详细地走过了 [这里](https://lifehacker.com/a-beginners-guide-to-diying-with-the-raspberry-pi-5976912) ，但这里是简短的版本:

**如何在 Windows 下将 Kali 安装到您的 SD 卡上**

1.  [为你的硬件下载 Kali Linux Raspberry Pi](https://www.offensive-security.com/kali-linux-arm-images/) 镜像(型号 B/B+用户应该抓取 TFT 版本，Raspberry Pi 2 应该抓取 Pi 2 版本)并解压。img 文件在里面。注意:如果你没有使用触摸屏显示器，下载树莓派 的 [普通版 Kali Linux。](https://www.offensive-security.com/kali-linux-vmware-arm-image-download/) 
2.  [下载 win32 diski manager](https://launchpad.net/win32-image-writer/+download)并解压应用程序(。exe 文件)中。
3.  使用读卡器将 SD 卡插入 Windows PC。
4.  双击打开您刚刚下载的应用程序 Win32DiskImager.exe。如果你运行的是 Windows 7 或 8，右击它，选择“以管理员身份运行”。
5.  如果应用程序没有自动检测到您的 SD 卡，请单击右上方的下拉菜单(标有“设备”)并从列表中选择它。
6.  在应用程序的图像文件部分，单击小文件夹图标并选择 Raspbian。您刚刚下载的 img 文件。
7.  单击 Write 按钮，等待 Win32DiskImager 完成它的工作。完成后，您可以安全地弹出您的 SD 卡，并将其插入您的 Raspberry Pi。

**如何在 OS X 将 Kali 安装到您的 SD 卡上**

1.  [为你的硬件下载 Kali Linux Raspberry Pi](https://www.offensive-security.com/kali-linux-arm-images/) 镜像(型号 B/B+用户应该抓取 TFT 版本，Raspberry Pi 2 应该抓取 Pi 2 版本)并解压。img 文件在里面。注意:如果你没有使用触摸屏显示器，下载树莓派 的 [普通版 Kali Linux。](https://www.offensive-security.com/kali-linux-vmware-arm-image-download/) 
2.  [下载 RPi-sd 卡构建器](http://alltheware.wordpress.com/2012/12/11/easiest-way-sd-card-setup) (一定要为你安装的 OS X 版本选择合适的版本)并解压应用程序。
3.  使用读卡器将 SD 卡插入 Mac。
4.  打开 RPi-sd 卡生成器。你会立即被要求选择一个拉斯比图像。选择。您之前下载的 img 文件。
5.  系统会询问您是否连接了 SD 卡。因为我们之前插入了它，所以它是，所以继续并单击 Continue。您将看到 SD 卡选项。如果您只插入了一个，您将不会在列表中看到任何其他内容，它将被检查。如果没有，只需检查您想要使用的卡，然后单击确定。
6.  输入您的管理员密码，然后单击确定。
7.  您将被询问 SD 卡是否被弹出。这是应该发生的，因为应用程序需要卸载它，以便它可以执行直接拷贝。仔细检查您的 SD 卡在 Finder 中是否不再可用。不要将其从 USB 端口上移除。确定后，点按“继续”。
8.  RPi-sd 卡生成器完成准备您的 sd 卡，安全弹出它并将其插入您的 Raspberry Pi 单元。

### 第二步:连接显示器

Raspberry Pi 有一个 GPIO(通用输入/输出),触摸屏可以插入其中。在你的 Raspberry Pi 上，它是角落里的一组大头针——它是如何组合在一起的应该很明显。继续点击你的显示器进入树莓 Pi。

### 第三步:插上所有的电源并开机

显示器装好后，是时候把其他东西都插上了。将 Wi-Fi 适配器和键盘插入 USB 端口。然后，将 Pi 插入电池组。

这里的启动过程可能会有点慢和笨拙，所以不要担心它会花一点时间。首先，在启动过程开始之前，您会看到一段时间的白屏。最终，你会看到一个登录界面。

如果你用的是 Raspberry Pi 2，你需要在这里做一些设置来让屏幕工作。如果您使用的是 B+，请跳到下一步。

Raspberry Pi 2 目前需要一些额外的步骤来让屏幕工作。当你第一次启动它时，迎接你的是一个悲伤的白色屏幕。谢天谢地，让屏幕工作起来并不太麻烦。不幸的是，你需要一个 HDMI 监视器来连接 Pi，或者你需要通过 SSH 登录 [来通过这个部分](https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md) 。继续连接其中任何一个并启动 Pi。

1.  您将在 Raspberry Pi 的命令行上看到用户名和密码提示。输入用户名`root`和密码`toor`。

2.  从安装引导分区开始。输入`mount /dev/mmcblk0p1 /boot`并按回车键。

3.  接下来，您将下载并安装 Adafruit 的安装软件。输入`wget http://adafruit-download.s3.amazonaws.com/adafruit_pitft_kernel_1.20150420-1.tar.gz` 并按回车键。

4.  键入`tar xf adafruit_pitft_kernel_1.20150420-1.tar.gz`并按回车键提取文件。

5.  输入`cd adafruit_pitft_kernel_1.20150420-1`并按回车键。

6.  输入`./install.sh`并按回车键。这需要一段时间。完成后，它会要求你重新启动。说是，并等待重新启动。

7.  输入`git clone https://github.com/adafruit/Adafruit-PiTFT-Helper.git`，回车下载 Adafruit 的屏幕软件。

8.  好了，现在你需要再次安装启动盘。输入`mount /dev/mmcblk0p1 /boot`并按回车键。

9.  输入`cd Adafruit-PiTFT-Helper`并按回车键。

10.  输入 `./adafruit-pitft-helper -u /root/ -t 28r`并按回车键。这将配置您的显示器。

11.  现在你需要解决一些开机屏幕只显示闪烁光标的问题。输入`sudo apt-get install xserver-xorg-video-fbdev`并按回车键。

12.  一旦完成，输入`cd /usr/share/X11/xorg.conf.d/`并按回车键。

13.  最后，键入`nano 99-fbdev.conf`并按回车键。这将打开一个文本文件。您需要将以下代码复制到文件中:

```
Section “Device”
Identifier “myfb”
Driver “fbdev”
Option “fbdev” “/dev/fb1”
EndSection
```

完成后，按 Ctrl+X 保存并退出。

应该可以了。继续键入 reboot，然后按 Enter 键，用一个工作屏幕重新启动您的 Pi。

### 第四步:登录并启用你的无线网卡

现在是登录并启用 Wi-Fi 卡的时候了，这样您就可以实际使用 Kali Linux 中的工具了。Raspberry Pi 会自动识别你的 Wi-Fi 卡，但你仍然需要登录到你的网络。首先，我们需要启动 Kali Linux 图形用户界面，并确保一切正常:

1.  您将在 Raspberry Pi 的命令行上看到用户名和密码提示。输入用户名`root`和密码`toor`(我们稍后会更改)。
2.  输入`startx` 并按回车键启动 Kali 的图形界面。这可能需要一点时间加载到 Pi 上。
3.  现在，您可以使用触摸屏和键盘浏览您的 Pi。点击底部 dock 上的小终端图标打开命令行。
4.  要设置您的 Wi-Fi 卡，请在命令行中键入`nano /etc/network/interfaces`,然后按 Enter 键加载您的 Wi-Fi 设置的配置文件。
5.  将以下几行添加到刚刚打开的文本文件中，替换您在中的网络信息:

```
auto wlan0
iface wlan0 inet dhcp
wpa-ssid “your network name”
wpa-psk “the network password”
```

完成后，按 Ctrl+X 保存并退出。您的 Wi-Fi 卡现在应该可以工作了(尽管您可能需要先重启)。

### 第五步:更改您的密码

在你做任何事情之前，你应该*真的*更改你的设备的根密码(以免其他具有类似黑客技能的人获得对它的控制)。谢天谢地，这很容易。

1.  当你还在命令行的时候(如果你不在，就点击 Kali 中的终端图标重新打开它)，输入`passwd`并按回车键。
2.  输入两次新密码。
3.  现在重新配置 OpenSSH 服务器也很好，这样它就不会被设置为默认服务器。输入`dpkg-reconfigure openssh-server`并按回车键。

现在，您的小型便携式系统已经设置好并安全了。

### 你能用这个设备做什么

从这里开始，你用你的便携式黑客站做什么由你决定。您可以使用 Pi 上的触摸屏进行基本导航，并运行您想要的 Kali Linux 中的任何程序。如果你不知道从哪里开始，这里有一些想法:

*   [设置 SSH 远程连接 Pi](https://www.raspberrypi.org/documentation/remote-access/ssh/)
*   [学习命令行的基础知识](http://lifehacker.com/a-command-line-primer-for-beginners-5633909)
*   [破解 Wi-Fi 密码，创建假网络，或者窥探另一台设备的流量](http://lifehacker.com/how-to-hack-your-own-network-and-beef-up-its-security-w-1649785071#_ga=1.261824013.1055861349.1441835238)

*   [监控网络上发生的一切](http://lifehacker.com/how-to-tap-your-network-and-see-everything-that-happens-1649292940)
*   [更多卡莉 Linux 指南](http://www.kalitutorials.net/2013/08/kali-linux.html)

世界是你的。各位负责任地黑吧。

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=5953047,5833254,1649292940&title=Get Off My LAN)