# 构建基于 Raspberry Pi 的 Amazon Echo 的最简单方法

> 原文：<https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212>

不久前，我们详细介绍了如何使用树莓派 制作自己的 [亚马逊 Echo 设备，但如果它出现任何问题，你就必须手动重启整个设备。这是一件痛苦的事情。现在，有一种更简单的方法来制作你自己的回声。](https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931) 



这个版本到底有什么不同？首先，最终结果基本相同:你可以通过说出唤醒词“Alexa”来激活你的 DIY Echo，该设备就像真正的 Echo 一样工作 [。](https://lifehacker.com/the-seven-best-things-you-can-do-with-an-amazon-echo-1766989219)

这里的安装过程是不同的。不使用 [亚马逊的官方资源](https://github.com/alexa/alexa-avs-sample-app) ，我们将使用一个名为 [Alexa Pi](https://github.com/alexa-pi/AlexaPi) 的 GitHub 项目。这将把亚马逊在 Echo 上使用的 Alexa 语音服务安装到你的 Raspberry Pi 上。有了这个版本的项目，如果出现问题，当你重启你的 Raspberry Pi 时，Alexa 服务会自动启动。这比之前的项目要好得多，之前的项目需要你通过打开三个不同的终端窗口来手动重启服务。除此之外，该方法还支持其他开发板，如 [Orange Pi](http://www.orangepi.org/) 和 [C.H.I.P](https://lifehacker.com/affordable-electronics-board-showdown-raspberry-pi-zer-1786409766) 。

显然，这并不比像 [Echo Dot](https://www.amazon.com/All-New-Amazon-Echo-Dot-Add-Alexa-To-Any-Room/dp/B01DFKC2SO?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&tag=kinjalifehackerlink-20) 这样的系统便宜，但如果你已经有了材料，它是完全可定制的，也是一个伟大的项目。就这样，让我们开始吧。

### 你需要什么

正如你所料，你需要一个树莓派和一些零件

*   [树莓派 3](https://www.amazon.com/Raspberry-Pi-RASP-PI-3-Model-Motherboard/dp/B01CD5VC92/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&ie=UTF8&keywords=raspberry+pi+3&qid=1476306172&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B01CD5VC92[au|5716493564230329059[b|lifehacker&s=pc&sr=1-2&tag=kinjalifehackerlink-20) (推荐)、 [树莓派 Zero W](https://www.raspberrypi.org/products/pi-zero-w/) 或 [树莓派 2](https://www.amazon.com/Raspberry-Pi-Model-Project-Board/dp/B00T2U7R7I/ref=sr_1_3?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&ie=UTF8&keywords=raspberry+pi+2&qid=1476306182&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B00T2U7R7I[au|5716493564230329059[b|lifehacker&s=pc&sr=1-3&tag=kinjalifehackerlink-20) (型号 2 还需要一个 USB Wi-FI 适配器)安装了 Raspbian 并设置了 Wi-FI。如果你之前没有安装过 Raspbian， [我们的指南涵盖了你需要知道的一切](http://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054) 。虽然我将集中精力在 Raspberry Pi 上安装它，但它也支持许多其他设备。你可以在这里 找到 [的完整列表。出于好奇，我也在 C.H.I.P .上运行了这个安装程序，它运行得很好。](https://github.com/alexa-pi/AlexaPi/wiki/Devices) 
*   一根 [MicroUSB 电源线](https://www.amazon.com/CanaKit-Raspberry-Supply-Adapter-Charger/dp/B00MARDJZ4/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&ie=UTF8&keywords=raspberry+pi+power&qid=1476306223&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B00MARDJZ4[au|5716493564230329059[b|lifehacker&sr=8-2&tag=kinjalifehackerlink-20) 。
*   一张 [8GB 的 MicroSD 卡](https://www.amazon.com/dp/B00IVPU7KE/ref=twister_B00IYOCEG2?_encoding=UTF8&asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&psc=1&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B00IVPU7KE[au|5716493564230329059[b|lifehacker&tag=kinjalifehackerlink-20) 。
*   一个 USB 麦克风(我用的是这个便宜的 6 美元的麦克风 ，但是几乎任何 USB 麦克风都可以用。如果你想稍微升级一下，[【8 美元】Playstation Eye](https://www.amazon.com/PlayStation-Eye-3/dp/B000VTQ3LU/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B000VTQ3LU[au|5716493564230329059[b|lifehacker&tag=kinjalifehackerlink-20) 似乎特别好用)如果你用的是树莓派 Zero W，你还需要一个 [MicroUSB-USB 适配器](https://www.amazon.com/Ksmile-Female-Adapter-SamSung-tablets/dp/B01C6032G0/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&ie=UTF8&keywords=microusb to usb&qid=1491931594&s=electronics&sr=1-2&tag=kinjalifehackerlink-20) 。
*   扬声器(任何有源扬声器都可以工作，我决定使用一个 [UE 迷你吊杆](https://www.amazon.com/MINI-BOOM-Wireless-Bluetooth-Speaker/dp/B01IC263QC/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&ie=UTF8&keywords=ue+mini+boom&qid=1476287163&rawdata=[r|https://www.google.com/[t|link[p|1787726931[a|B01IC263QC[au|5716493564230329059[b|lifehacker&s=electronics&sr=1-2&tag=kinjalifehackerlink-20) ，因为我已经拥有它，即使当它插入 Pi 时，它仍然可以作为蓝牙扬声器工作)。
*   用于设置的键盘和鼠标(或使用 SSH，[)Adafruit 的 Pi Finder](https://lifehacker.com/the-raspberry-pi-finder-easily-locates-your-pis-ip-addr-1702081021) 使这个项目更容易从您的主计算机上完成，因为您可以复制/粘贴较长的命令)。

现在你已经把所有的东西都收集起来，连接好，插上电源，让我们来建造这个吸盘。

### 第一步:注册一个免费的亚马逊开发者账户

在你做任何事情之前，你需要注册一个免费的亚马逊开发者账户，然后为你的 DIY Echo 创建一个档案。如果你已经这样做了，因为你做了以前版本的 DIY Echo，请注意第 10-13 节略有不同，所以你会想改变这些细节。否则，这是非常简单的，尽管需要点击很多次:

1.  登录你的 [亚马逊开发者账号](https://developer.amazon.com/home.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212&asc_source=&rawdata=[r|https://www.google.com/[t|link[p|1787726931[au|5716493564230329059[b|lifehacker&tag=kinjalifehackerlink-20) 。
2.  点击 Alexa 标签。
3.  单击注册产品类型>设备。
4.  命名您的设备类型和显示名称(我任意选择了“Pi2 ”,尽管您可以在这里输入您想要的任何内容),然后单击 Next。
5.  在安全配置文件窗口上，单击“创建新配置文件”
6.  在“常规”选项卡下，在“安全配置文件名称”旁边命名您的配置文件。对描述进行同样的操作。单击下一步。
7.  记下网站为您生成的产品 ID、客户端 ID 和客户端密码。
8.  单击 Web 设置选项卡，然后单击配置文件下拉列表旁边的编辑按钮。
9.  在“允许的来源”旁边，点击“添加另一个”并输入:`http://localhost:5050`。
10.  点击“添加另一个”，然后输入`http://your.raspberrypi.ip.address:5050`，但用你的树莓派的 IP 地址替换为`your.raspberrypi.ip.address`。你可以使用 [Pi 查找工具找到你的 Pi 的 IP 地址，这里详细介绍](https://lifehacker.com/how-to-control-your-raspberry-pi-from-any-computer-usin-1788592777) 。
11.  在允许返回的网址旁边，点击“添加另一个”并输入:`http://localhost:5050/code`
12.  点击“添加另一个”,再次添加`http://your.raspberrypi.ip.address:5050/code`,用您自己的信息替换`your.raspberrypi.ip.address`。完成后，单击下一步。

13.  接下来是设备详细信息选项卡。你在这里输入什么并不重要。选择一个类别，写一个描述，选择一个预期的时间表，并在表格上计划使用多少设备旁边输入 0。单击下一步。
14.  最后，你可以在这里选择添加亚马逊音乐。这在 Pi 驱动的设备上**不**起作用，所以保持选中为“否”。点击保存。

现在您有了一个 Amazon 开发人员帐户，并且为 Pi 驱动的 Echo 创建了一个配置文件。是时候去树莓酒吧让 Alexa 工作了。

### 第二步:安装 Git 和 AlexaPi

接下来，您需要在您的 Raspberry Pi 上启动终端，因为我们将在命令行中完成整个项目。在你开始安装之前，你需要更新和安装一些东西:

1.  键入`sudo apt-get install update`并按 Enter 键以确保您的 Raspbian 版本是最新的。让它在这里做它的事情。
2.  键入 `sudo apt-get install git`并按回车键安装 Git。还是那句话，让它做它该做的。
3.  键入`cd /opt`并按回车键改变目录。
4.  最后，键入`sudo git clone https://github.com/alexa-pi/AlexaPi.git`并按回车键克隆 AlexaPi GitHub 库。再次，给它一秒钟下载和做它的事情。

这就是下载部分，然后是实际安装。

### 第三步:运行 AlexaPi 安装脚本

接下来，您将运行一个安装脚本。这将自动安装让 Echo 启动和运行所需的所有其他东西。

1.  输入`sudo ./AlexaPi/src/scripts/setup.sh`并按回车键。
2.  你会被问一系列问题。如果你使用的是 Raspberry Pi，只需在操作系统和设备提示符下按回车键。最后一个问题问你要不要加入 AirPlay 支持。如果你有一个 iOS 设备，这使得你可以轻松地通过 Airplay 将音乐从你的 iPhone 流式传输到你的 DIY Echo。该脚本将在接下来的 5-10 分钟内下载一系列软件，所以请放松一下。
3.  最后，你会被要求输入你的亚马逊开发者信息。键入您在第一步中创建的设备类型 ID 和安全配置文件描述(我们使用的是 AlexaPi)。接下来，您需要输入所有这些又长又复杂的数字作为您的个人资料 ID、客户 ID 和客户密码。
4.  最后，你需要做的最后一件事是授权你的设备。您只需要这样做一次。回到你的主电脑，打开网页浏览器。然后输入`http://your.raspberrypi.ip.address:5050`，用之前你的 Raspberry Pi 的 IP 地址替换`your.raspberryi.ip.address`。然后你需要登录你的亚马逊账户。之后，您会看到一个授权令牌。

就是这样，Alexa 语音服务现在已经安装在你的树莓 Pi 上了。你只需要启动服务。你可以完全重启你的设备，或者输入`sudo systemctl start AlexaPi.service`并按回车键来启动它。

试试吧，对着麦克风说“Alexa”，它应该会回答“是？”如果它不起作用，你可以输入`sudo systemctl status AlexaPi.service`并按回车键来检查状态。当你重启设备或者由于某种原因断电时，Alexa 会自动启动，所以你不应该再去想它。