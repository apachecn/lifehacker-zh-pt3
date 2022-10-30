# 如何用树莓派构建自己的亚马逊 Echo

> 原文:[https://life hacker . com/how-to-build-your-own-Amazon-echo-a-raspberry-pi-1787726931](https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931)

亚马逊的放在家里很有用。它可以播放播客，做提醒和笔记，告诉你通勤的长度，甚至控制你家里的其他电器。但价格从 50 美元到 150 美元不等，如果你不确定是否会使用它，这是一个昂贵的提议。不过好消息是，你可以用树莓派做一个全功能的。

Watch

**更新** : [这个方法稍微简单一点，能让你得到更好的最终产品](https://lifehacker.com/the-simplest-way-to-build-a-raspberry-pi-powered-amazon-1794218212) 。我们保留这个指南，因为它使用亚马逊的官方仓库，但是这个系统工作得更好。

### 你会得到什么

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-4yfK90OJrek&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-4yfK90OJrek&start=0) 

在本指南结束时，你将拥有一个(几乎是) [全功能的亚马逊 Echo](https://lifehacker.com/the-seven-best-things-you-can-do-with-an-amazon-echo-1766989219) 来响应你的语音命令。它唯一不能做的是访问亚马逊 Prime、Spotify 或 Pandora 等音乐服务。否则，它就是亚马逊虚拟助手 Alexa 的所有花哨功能的回声。这意味着它可以进行单位转换，查看体育比分，给你读你的 Kindle 书籍，查看天气，播放播客和广播，等等。一旦完成，你将能够 [使用 Alexa 配套应用](https://www.amazon.com/gp/help/customer/display.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&nodeId=201602060&tag=kinjalifehackerlink-20)[(](https://www.amazon.com/gp/help/customer/display.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&nodeId=201602060&tag=kinjalifehackerlink-20)iOS和 [](https://www.amazon.com/gp/help/customer/display.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&nodeId=201602060&tag=kinjalifehackerlink-20)Android)来改变你的 Alexa 的设置，你将能够在一个真实的 Echo 上安装所有相同的技能。这包括像 [这样的蝙蝠侠选择自己的冒险游戏](http://www.alexaskillstore.com/other/the-wayne-investigation/635) 或者一个 [的猫事实数据库](http://www.alexaskillstore.com/other/cat-facts/257) 。也许在更有用的一端，它包括最近宣布的与第三方待办应用程序的集成，如[【Todoist】](https://blog.todoist.com/2016/10/13/todoist-alexa-integration/)和 [Any.do](http://www.theverge.com/circuitbreaker/2016/10/13/13268142/amazon-echo-alexa-any-do-integration) 。

它还可以与各种联网设备配合工作，如 LIFX 或 [Nest 恒温器](https://nest.com/support/article/Learn-how-to-control-your-Nest-Thermostat-with-Amazon-Alexa-on-Echo-and-Fire-TV) 等智能灯泡，所以你可以用你的声音控制它们。像真实的 Echo 一样，你的 DIY Echo 可以链接到 [如果这样那么](https://ifttt.com/) 到 [添加更多功能](https://ifttt.com/amazon_alexa) ，像添加 [待办事项到 Evernote](https://ifttt.com/recipes/284234-add-your-alexa-to-dos-to-evernote) 或者 [当定时器响起时在你的手机上得到通知](https://ifttt.com/recipes/303974-receive-a-notification-on-your-phone-when-your-echo-timer-goes-off) 。

就价格而言，有一件事我们应该在这里提一下:亚马逊最新的 [Echo Dot](https://www.amazon.com/gp/product/B01DFKC2SO?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&hvadid=138821270547&hvdev=c&hvexid=&hvnetw=g&hvpone=&hvpos=1t1&hvptwo=&hvqmt=e&hvrand=2363571709453072558&ref=ODS_HA_B_surl&ref=pd_sl_1bxrunqc4w_e&tag=kinjalifehackerlink-20) (较小的 Echo，带有一个垃圾扬声器)仅售 50 美元，这使得用 35 美元的树莓皮制作自己的产品变得更加困难。然而，树莓派有一个关键的特点使它物有所值:*它仍然是一个树莓派，而不是一个单位任务设备*。这个项目只是安装了一套程序，使你的树莓 Pi 像回声一样工作。你的树莓 Pi 仍然可以与许多其他项目一起工作，如 [复古游戏站](http://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) (你只需要 [安装桌面环境](https://github.com/retropie/retropie-setup/wiki/Updating-RetroPie) )或 [媒体中心](http://lifehacker.com/turn-a-raspberry-pi-into-an-xbmc-media-center-in-under-5929913) 。这意味着你可以把它变成一台多任务处理机器。

### 你需要什么

正如你所料，你需要一个树莓派和一些零件

*   [树莓 Pi 3](https://www.amazon.com/Raspberry-Pi-RASP-PI-3-Model-Motherboard/dp/B01CD5VC92/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&ie=UTF8&keywords=raspberry pi 3&qid=1476306172&s=pc&sr=1-2&tag=kinjalifehackerlink-20) (推荐)或 [树莓 Pi 2](https://www.amazon.com/Raspberry-Pi-Model-Project-Board/dp/B00T2U7R7I/ref=sr_1_3?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&ie=UTF8&keywords=raspberry pi 2&qid=1476306182&s=pc&sr=1-3&tag=kinjalifehackerlink-20) (型号 2 还需要 USB Wi-FI 适配器)安装了 Raspbian。如果你之前没有安装过 Raspbian， [我们的指南涵盖了你需要知道的一切](https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054) 。
*   一根 [MicroUSB 电源线](https://www.amazon.com/CanaKit-Raspberry-Supply-Adapter-Charger/dp/B00MARDJZ4/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&ie=UTF8&keywords=raspberry pi power&qid=1476306223&sr=8-2&tag=kinjalifehackerlink-20)
*   一张 [8GB 的 MicroSD 卡](https://www.amazon.com/dp/B00IVPU7KE/ref=twister_B00IYOCEG2?_encoding=UTF8&asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&psc=1&tag=kinjalifehackerlink-20)
*   一个 USB 麦克风(我用的是这个便宜的 6 美元的麦克风 ，但是几乎任何 USB 麦克风都可以用。如果你想稍微升级一下，[【8 美元】的 Playstation Eye](https://www.amazon.com/PlayStation-Eye-3/dp/B000VTQ3LU/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&tag=kinjalifehackerlink-20) 似乎特别好用
*   扬声器(任何有源扬声器都可以工作，我决定使用一个 [UE 迷你吊杆](https://www.amazon.com/MINI-BOOM-Wireless-Bluetooth-Speaker/dp/B01IC263QC/ref=sr_1_2?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&ie=UTF8&keywords=ue mini boom&qid=1476287163&s=electronics&sr=1-2&tag=kinjalifehackerlink-20) ，因为我已经拥有它，即使当它插入 Pi 时，它仍然可以作为蓝牙扬声器工作)
*   用于设置的键盘和鼠标(或 [用 VNC](https://www.raspberrypi.org/documentation/remote-access/vnc/) 访问计算机)

理论上可以使用更老的树莓派或 [树莓派零](https://www.adafruit.com/product/2885)[f](https://www.adafruit.com/product/2885)[r](https://www.adafruit.com/product/2885)[t](https://www.adafruit.com/product/2885)h[I](https://www.adafruit.com/product/2885)sp[r](https://www.adafruit.com/product/2885)o[j](https://www.adafruit.com/product/2885)[GitHub 上的这个线程](https://github.com/alexa/alexa-avs-sample-app/issues/2) 可以帮上忙。然而，我们在 Raspberry Pi 2 和 3 上测试了这一点。

你可以通过安装亚马逊 Alexa 技能工具包 到树莓派上来构建你的 DIY Echo。对于本指南，我们将使用亚马逊的官方代码。不过这有一个警告:它要求你每次启动 Pi 时手动启动 Alexa 服务*。这很烦人，但假设你没有经常断电或需要经常重启你的 Pi，这只是有点烦人。*

### 第一步:注册一个亚马逊开发者账户

在你做任何事情之前，你需要注册一个免费的亚马逊开发者账户，然后为你的 DIY Echo 创建一个档案。这很简单:

1.  登录你的 [亚马逊开发者账号](https://developer.amazon.com/home.html?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931&asc_source=&tag=kinjalifehackerlink-20) 。
2.  点击 Alexa 标签。
3.  单击注册产品类型>设备。
4.  命名您的设备类型和显示名称(我们选择“Raspberry Pi”作为两者)。
5.  单击下一步。
6.  在安全配置文件屏幕上，点击“创建新配置文件”
7.  在“常规”选项卡下，在“安全配置文件名称”旁边命名您的配置文件。对描述进行同样的操作。单击下一步。
8.  记下网站为您生成的产品 ID、客户端 ID 和客户端密码。
9.  单击 Web 设置选项卡，然后单击配置文件下拉列表旁边的编辑按钮。
10.  在“允许的来源”旁边，点击“添加另一个”并输入:`https://localhost:3000`。
11.  在允许返回的网址旁边，点击“添加另一个”并输入:`https://localhost:3000/authresponse`完成后点击下一步。
12.  接下来是设备详细信息选项卡。你在这里输入什么并不重要。选择一个类别，写一个描述，选择一个预期的时间表，并在表格上计划使用多少设备旁边输入 0。单击下一步。
13.  最后，你可以在这里选择添加亚马逊音乐。这在 Pi 驱动的设备上**不**起作用，所以保持选中为“否”。点击保存。

现在您有了一个 Amazon 开发人员帐户，并且为 Pi 驱动的 Echo 创建了一个配置文件。是时候去树莓酒吧让 Alexa 工作了。

### 第二步:克隆并安装 Alexa

把所有东西都插入你的 Pi 并启动它。你需要进入图形用户界面( [现在被称为像素](https://lifehacker.com/the-new-raspberry-pi-os-is-here-and-it-looks-great-1787194540) )，因为你最终会使用网络浏览器来验证你的设备。

1.  在 Raspberry Pi 上打开终端应用程序，键入:`cd Desktop`并按回车键。
2.  输入`git clone https://github.com/alexa/alexa-avs-sample-app.git`并按回车键。

3.  一旦完成，输入:`cd ~/Desktop/alexa-avs-sample-app`并按回车键。
4.  输入`nano automated_install.sh`并按回车键。
5.  这将打开您的文本编辑器。在这里，您需要输入您在上一步中记录的 ProductID、ClientID 和 ClientSecret。使用箭头键导航到每个条目。如上图所示，在`=`符号后输入每个细节。完成后，点击 CTRL+X 保存并退出。
6.  您现在回到了命令行。是时候运行安装脚本了。输入 `cd ~/Desktop/alexa-avs-sample-app`并按回车键。
7.  输入`. automated_install.sh`并按回车键。
8.  出现提示时，按 Y 键回答不同的问题，并回答您认为合适的其他问题。这将配置您的 Pi 并安装一些额外的软件。这可能需要 30 分钟，所以让它做它的事情。

一旦完成，就该启动 Alexa 服务了。

### 第三步:运行 Alexa Web 服务

接下来，您将在三个不同的终端窗口中同时运行三组命令。您将为以下每个步骤创建一个新的终端窗口。不要关任何窗户！每次重启 Raspberry Pi 时，您都需要执行第三步(这一步)、第四步和第五步。

你首先要启动的是 Alexa 网络服务:

1.  输入`cd ~/Desktop/alexa-avs-sample-app/samples`并按回车键。
2.  输入`cd companionService && npm start`并按回车键。

这将启动配套服务，并打开一个端口与 Amazon 通信。让这扇窗户开着。

### 第四步:运行示例应用程序并确认您的帐户

打开第二个终端窗口(文件>新窗口)。下一步是运行一个 Java 应用程序，并启动一个 web 浏览器，将您的 Pi 驱动的 Echo 注册到 Alexa web 服务。

1.  在新的终端窗口中输入`cd ~/Desktop/alexa-avs-sample-app/samples`并按回车键。
2.  输入`cd javaclient && mvn exec:exec`并按回车键。
3.  将弹出一个窗口，要求您验证您的设备。单击是。这将打开一个浏览器窗口。Java 应用程序中会出现第二个弹出窗口，要求您单击 Ok。不要**不要**点击这个。
4.  在浏览器中登录您的亚马逊帐户。
5.  您将看到设备的认证屏幕。单击确定。您的浏览器现在将显示“设备令牌就绪”
6.  现在，您可以在 Java 应用程序中单击“确定”弹出窗口。

现在，您的 Raspberry Pi 拥有了与 Amazon 的服务器通信所需的令牌。让这个终端窗口保持打开。

### 第五步:启动你的唤醒词引擎

最后，打开第三个终端窗口(文件>新窗口)。在这里，您将启动唤醒词引擎。这使得你可以说“Alexa ”,让你的树莓派开始听你说话。你有两个唤醒词软件选项，和 [KITT。AI](https://github.com/Kitt-AI/snowboy) 。两者都是免费的，但 Sensory 在 90 天后过期，所以让我们改用 KITT:

1.  输入`cd ~/Desktop/alexa-avs-sample-app/samples`并按回车键。
2.  输入`cd wakeWordAgent/src && ./wakeWordAgent -e kitt_ai`

就这样，你的 DIY Echo 现在运行了。说“Alexa”试试吧。您应该会听到一声哔哔声，表示它正在监听。当你听到哔哔声时，问一个类似“天气如何？”或者“道奇队比赛的比分是多少？”

### 第六步:改进麦克风，确保你的回声能听到你

最后，根据麦克风的质量，您可能会注意到它听不清您的声音。与其声嘶力竭地喊“Alexa”，不如最后一次去命令行。

1.  从命令行输入`alsamixer`并按回车键。
2.  轻按“F6”以选择不同的 USB 设备。使用箭头键选择您的麦克风。
3.  使用箭头键增加采集音量。
4.  当您对音量满意时，轻按 ESC 退出。
5.  输入 `sudo alsactl store`并按下回车键，使设置永久化。

现在，你应该能够像正常人一样对它说话，而不是大喊大叫，从而触发你的 DIY 回声。如果需要，您也可以在这里更改默认音量。

### 额外积分:添加 AirPlay 支持

你的 DIY Echo 在商业版中缺少的一点是作为蓝牙扬声器的功能。可以用 AirPlay 添加 [类似的功能。这样，你的回声也可以作为一个接收器，你可以从你的手机或电脑发送音乐。这很容易添加，您只需要通过终端最后一次访问命令行:](http://lifehacker.com/turn-a-raspberry-pi-into-an-airplay-receiver-for-stream-5978594) 

1.  输入`sudo apt-get install git libao-dev libssl-dev libcrypt-openssl-rsa-perl libio-socket-inet6-perl libwww-perl avahi-utils libmodule-build-perl`并按回车键。这将安装您需要的不同软件。
2.  出现提示时按 Y 键，等待所有内容下载并安装。
3.  输入`git clone https://github.com/njh/perl-net-sdp.git`并按回车键。这是 AirPlay 软件的最新版本所必需的。接下来的几个命令构建并安装这个软件。
4.  输入 `cd perl-net-sdp`并按回车键。
5.  输入`perl Build.PL`并按回车键。
6.  输入`sudo ./Build`并按回车键。
7.  输入`sudo ./Build test`并按回车键。
8.  输入`sudo ./Build install`并按回车键。
9.  输入`CD ..`并按回车键。
10.  现在你会抓住 shairport，DIY 机场软件。输入`git clone https://github.com/hendrikw82/shairport.git`并按回车键。

11.  输入`cd shairport`并按回车键。
12.  输入`make`并按回车键。
13.  输入`./shairport.pl -a AlexaPi`并按回车键。

有了它，你现在可以使用 AirPlay 协议将音乐或其他音频传输到你的 DIY Echo。既然您的 Echo 已经启动并运行，那么就开始使用它吧。