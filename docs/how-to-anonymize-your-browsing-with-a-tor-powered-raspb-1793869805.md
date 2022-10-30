# 如何使用 Tor 驱动的 Raspberry Pi 热点匿名浏览

> 原文：<https://lifehacker.com/how-to-anonymize-your-browsing-with-a-tor-powered-raspb-1793869805>

如果你一直在考虑尝试 Tor 来匿名化你所有的网络浏览，你可以 [下载一个浏览器](https://www.torproject.org/projects/torbrowser.html.en') 并尝试一下，但是制作你自己的高度便携的代理更有趣，你可以随时随地轻松连接到它。进入树莓 Pi。

Watch

Tor 是匿名浏览互联网最简单的方式之一 ，尽管它确实以速度为代价。事实上，它的速度慢得离谱，基本的互联网浏览都很难使用。但这并不意味着它对其他事情没有用处，因为你可能不想一直使用它，所以在 Tor 和常规互联网之间快速切换是很方便的。

树莓派可以帮上忙。首先，你需要把一个 Raspberry Pi 变成一个接入点，很像一个 Wi-Fi 热点，然后你在上面安装 Tor，这样所有通过接入点的流量都是匿名的。

当你想使用 Tor 时，你只需连接树莓 Pi 的 Wi-Fi 网络。当你没有的时候，你可以使用你通常使用的任何网络。Tor 浏览器 也是一个选择，但是你可能不想在你所有的设备上安装软件。如果你是常驻的“技术人员”,这也是很好的选择，因为它可以非常简单地向某人展示，如果他们真的决定使用 Tor 进行浏览，生活会是什么样子(这将是很慢的)。

### 你需要什么

制作 Tor 驱动的 Pi 代理并不需要什么特别的东西，但是在开始之前，您需要收集一些材料:

*   [树莓派 3](https://www.amazon.com/Raspberry-Pi-RASPBERRYPI3-MODB-1GB-Model-Motherboard/dp/B01CD5VC92?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-anonymize-your-browsing-with-a-tor-powered-raspb-1793869805&asc_source=&tag=kinjalifehackerlink-20)
*   [微型 USB 电源](https://www.amazon.com/CanaKit-Raspberry-Supply-Adapter-Charger/dp/B00MARDJZ4/ref=sr_1_3?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-anonymize-your-browsing-with-a-tor-powered-raspb-1793869805&asc_source=&ie=UTF8&keywords=pi 3 charger&qid=1490907232&s=electronics&sr=1-3&tag=kinjalifehackerlink-20)
*   以太网电缆
*   [8GB MicroSD 卡](https://www.amazon.com/SanDisk-Memory-Frustration-Free-Packaging-SDSDQ-008G-AFFP/dp/B007KFXICK/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-anonymize-your-browsing-with-a-tor-powered-raspb-1793869805&asc_source=&ie=UTF8&keywords=micro sd card&qid=1490907252&refinements=p_n_feature_two_browse-bin:6518302011&s=pc&sr=1-2&tag=kinjalifehackerlink-20)
*   访问您的家庭路由器
*   用于初始设置过程的鼠标/键盘/台式计算机

您需要继续使用 Raspbian 设置您的 SD 卡，并设置 SSH。您可以使用 Raspbian 的标准版本，也可以使用 Lite 版本，因为在本指南中您将只使用命令行。 [按照我们的指导在这里设置 Raspbian](https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054) (确保在此过程中更改您的默认密码)和 [本指南启用 SSH](https://www.raspberrypi.org/documentation/remote-access/ssh/) 如果您想从您家庭网络上的任何一台计算机与您的 Raspberry Pi 对话。

一旦你把所有东西都收集到一起，确保你的 Raspberry Pi 通过以太网电缆直接连接到你的路由器，然后插上电源。

### 第一步:安装必要的软件

我们需要做的第一件事是让树莓 Pi 3 的 Wi-Fi 能够像接入点一样工作。这将它变成一个热点，这样你就可以从你的主电脑连接到它，就像你可以连接任何无线网络一样。我们将从 Raspberry Pi 的命令行完成所有这些工作:

1.  输入`sudo apt-get update`并按回车键。
2.  输入`sudo apt-get install iptables-persistent git`
3.  选择`Yes`并按两次提示键。

现在所有的东西都已经下载并安装好了，是时候进行设置了。

### 第二步:把你的树莓皮变成一个接入点

将树莓派转变为接入点的过程有点复杂，但谢天谢地 GitHub 用户 [harryallerston](https://github.com/harryallerston) 创建了一个脚本来自动化整个过程。

1.  输入`git clone https://github.com/unixabg/RPI-Wireless-Hotspot.git`并按回车键。
2.  输入`cd RPI-Wireless-Hotspot`并按回车键。
3.  输入`sudo ./install`并按回车键。这将启动安装过程。
4.  按`Y`同意条款，`Y`使用预配置的 DNS 服务器，`N`使用 Unblock-Us 服务器，`Y`使用 OpenDNS，然后`N`使用 Wi-Fi 默认设置。
5.  默认问题后出现提示时，输入新密码。这是连接到 Pi 供电网络的密码。
6.  出现提示时，输入新的 SSID，这是您的网络名称。
7.  输入频道号。很好，除非你知道你需要别的东西。
8.  输入`N`回答其余问题。

一旦完成，你的 Raspberry Pi 将重新启动，现在应该作为一个接入点。你可以通过使用另一台电脑或手机，从 Wi-Fi 网络列表中选择你的 Raspberry Pi，并查看互联网是否可用来测试这一点。如果由于某种原因，它没有运行， [Adafruit 有一个向导](https://learn.adafruit.com/setting-up-a-raspberry-pi-as-a-wifi-access-point/overview) 来手动完成这一切。否则，继续并安装 Tor 代理软件。

### 第三步:安装 TOR

Tor 有一个非常简单的设置过程，但是你仍然需要调整一些东西来让它工作。

1.  输入`sudo apt-get install tor`并按回车键。
2.  输入`sudo nano /etc/tor/torrc`并按回车键。一直滚动到文档的底部，并将下面的文本输入到文本文件中。完成后，按 Ctrl+X 保存并继续:

```
Log notice file /var/log/tor/notices.log
VirtualAddrNetwork 10.192.0.0/10
AutomapHostsSuffixes .onion,.exit
AutomapHostsOnResolve 1
TransPort 9040
TransListenAddress 192.168.42.1
DNSPort 53
DNSListenAddress 192.168.42.1
```

接下来，你需要告诉 Wi-Fi 接口通过 Tor 软件发送互联网流量。这是通过几个命令实现的:

1.  输入`sudo iptables -F`并按回车键。
2.  输入`sudo iptables -t nat -F`并按回车键。
3.  输入`sudo iptables -t nat -A PREROUTING -i wlan0 -p tcp --dport 22 -j REDIRECT --to-ports 22`并按回车键。

4.  输入`sudo iptables -t nat -A PREROUTING -i wlan0 -p udp --dport 53 -j REDIRECT --to-ports 53`并按回车键。

5.  输入`sudo iptables -t nat -A PREROUTING -i wlan0 -p tcp --syn -j REDIRECT --to-ports 9040`并按回车键。

6.  输入`sudo sh -c iptables-save > /etc/iptables/rules.v4`并按回车键。

现在，是时候最终开始 Tor 了。输入`sudo service tor start`并按回车键。然后，键入`sudo service tor status`以确保它正常工作。如果你没有看到任何错误代码，它的工作。你可以设置它在启动时自动启动，方法是输入`sudo update-rc.d tor enable`，然后按回车键。

完成后，继续重新启动一次。输入`sudo reboot`并按回车键。你的 Raspberry Pi 现在应该在启动时自动启动所有东西。

### 第四步:连接并浏览你的新 TOR 代理

现在，你需要做的就是将任何你想匿名浏览的设备连接到你新的 Raspberry Pi 无线网络。您的常规家庭 Wi-Fi 和这个都将存在，所以像选择任何 Wi-Fi 网络一样选择它。当你连接上时，前往https://check.torproject.org/以验证你在 Tor 网络上。享受你的缓慢，但匿名的互联网！