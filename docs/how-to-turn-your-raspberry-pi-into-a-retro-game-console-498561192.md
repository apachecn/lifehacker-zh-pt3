# 如何建立一个树莓派复古游戏机

> 原文：<https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192>



自发布以来，35 美元的 Raspberry Pi 迷你电脑被誉为完美的一体化复古游戏机。现在，这比以往任何时候都容易，而且不需要任何 Linux 知识。以下是如何在 10 分钟内制作自己的复古游戏机。



***更新(2017 年 2 月 9 日)*** *:我们更新了本指南，以反映 RetroPie 最新版本(目前为 4.1)中的变化。这包括设置您的卡、系统和控制器的全新部分。谢天谢地，现在整个过程简单多了！如果您只是想将 RetroPie 的旧版本更新到最新版本，请启动 RetroPie 并进入 RetroPie 菜单>更新，或者按照本* [*指南*](https://github.com/retropie/retropie-setup/wiki/updating-retropie) *获取更多详细说明。*

我们已经带你经历了树莓派 的各种 [DIY 项目，但这一个可能是最简单的。您将在不到 10 分钟的时间内安装并运行复古游戏控制台(配有老式控制器)。你所需要做的就是在 SD 卡上安装操作系统，并从你的电脑上做一些简单的文件共享。](http://lifehacker.com/tag/raspberry-pi)

在我们开始之前，让我们复习一些基础知识。模仿老派电子游戏需要两样东西:游戏光盘和一个玩游戏的模拟器。ROM 是存在于你的设备上的游戏的拷贝。仿真器是可以播放 ROM 应用程序。模拟器伦理的规则是，如果你有 ROM，你应该有一个游戏的物理副本(或者你 [可以从你的旧墨盒创建你自己的](http://www.retrode.org/) )。我们会让你自己想出 rom。就这样，让我们来设置树莓派。

### **你将得到什么**

你的树莓派会自动启动进入 [仿真站](https://github.com/Aloshi/EmulationStation) 。这是一个运行在名为 RetroPie 的自定义 SD 卡上的程序，它允许您使用控制器来选择模拟器和游戏，而无需触摸键盘或鼠标。在一切都设置好之后，你将能够从一个控制器导航和做你需要在 Raspberry Pi 上做的一切。

除了游戏，你还可以获得媒体中心软件的完整版本，(你需要 [进入一些高级设置来下载](https://github.com/RetroPie/RetroPie-Setup/wiki/KODI) Kodi)。这意味着您基本上可以拥有一个运行经典游戏和媒体中心的一体化娱乐中心。这是一个相当杀手的设置。

你能模仿什么系统？他们中的很多人:

*   [3do](https://github.com/retropie/retropie-setup/wiki/3do)T3】
*   [阿米加](https://github.com/retropie/retropie-setup/wiki/Amiga)T3】
*   [Amstrad CPC](https://github.com/retropie/retropie-setup/wiki/Amstrad-CPC)T3】
*   [苹果二代](https://github.com/retropie/retropie-setup/wiki/Apple-II)T3】
*   [雅达利 2600](https://github.com/retropie/retropie-setup/wiki/Atari-2600)
*   [雅达利 5200 和 8 位系列](https://github.com/retropie/retropie-setup/wiki/Atari-800-and-5200)
*   [雅达利 7800](https://github.com/retropie/retropie-setup/wiki/Atari-7800)
*   [雅达利捷豹](https://github.com/retropie/retropie-setup/wiki/Atari-Jaguar)
*   [雅达利猞猁](https://github.com/retropie/retropie-setup/wiki/Atari-Lynx)
*   [雅达利 ST/STE/TT/猎鹰](https://github.com/retropie/retropie-setup/wiki/Atari-ST-STE-TT-Falcon)T3】
*   [田蜜](https://github.com/retropie/retropie-setup/wiki/Coco)T3】

*   [准将 64](https://github.com/retropie/retropie-setup/wiki/Commodore-64)
*   达芙妮
*   [【dragon 32】](https://github.com/retropie/retropie-setup/wiki/Dragon)
*   [梦幻组合](https://github.com/retropie/retropie-setup/wiki/Dreamcast)
*   [最终燃烧阿尔法](https://github.com/retropie/retropie-setup/wiki/FinalBurn-Alpha)
*   [GameCube](https://github.com/retropie/retropie-setup/wiki/GameCube)
*   [游戏&观看](https://github.com/retropie/retropie-setup/wiki/Game-&-Watch)
*   [游戏装备](https://github.com/retropie/retropie-setup/wiki/Game-Gear)
*   [游戏少年](https://github.com/retropie/retropie-setup/wiki/Game-Boy)
*   [游戏男孩色](https://github.com/retropie/retropie-setup/wiki/Game-Boy-Color)
*   [游戏少年晋级](https://github.com/retropie/retropie-setup/wiki/Game-Boy-Advance)
*   [智能视觉](https://github.com/retropie/retropie-setup/wiki/Intellivision)
*   [麦金塔](https://github.com/retropie/retropie-setup/wiki/Macintosh)
*   MAME
*   [主控系统](https://github.com/retropie/retropie-setup/wiki/Master-System)
*   [mega drive/创世纪](https://github.com/retropie/retropie-setup/wiki/Genesis-Megadrive)T3】
*   [狼狈](https://github.com/retropie/retropie-setup/wiki/MESS)
*   MSX
*   [任天堂 64](https://github.com/retropie/retropie-setup/wiki/Nintendo-64)
*   [任天堂 DS](https://github.com/retropie/retropie-setup/wiki/Nintendo-DS)
*   [任天堂娱乐系统](https://github.com/retropie/retropie-setup/wiki/Nintendo-Entertainment-System)
*   [近地天体](https://github.com/retropie/retropie-setup/wiki/Neo-Geo)
*   [近地小行星](https://github.com/retropie/retropie-setup/wiki/Neo-Geo-Pocket)
*   [Neo Geo 口袋颜色](https://github.com/retropie/retropie-setup/wiki/Neo-Geo-Pocket-Color)
*   [Oric-1/Atmos](https://github.com/retropie/retropie-setup/wiki/Oric)T3】
*   [PC](https://github.com/retropie/retropie-setup/wiki/PC)
*   [PC 发动机/TurboGrafx-16](https://github.com/retropie/retropie-setup/wiki/PC-Engine)
*   [PC-FX](https://github.com/retropie/retropie-setup/wiki/PC-FX)
*   [PSP](https://github.com/retropie/retropie-setup/wiki/PSP)
*   [PlayStation 1](https://github.com/retropie/retropie-setup/wiki/Playstation-1)
*   [PlayStation 2](https://github.com/retropie/retropie-setup/wiki/Playstation-2)
*   [剩余虚拟机](https://github.com/retropie/retropie-setup/wiki/ResidualVM)
*   [萨姆·库佩](https://github.com/retropie/retropie-setup/wiki/Sam-Coupe)T3】
*   土星

*   [世嘉 32X](https://github.com/retropie/retropie-setup/wiki/Sega-32X)T3】
*   [世嘉 CD](https://github.com/retropie/retropie-setup/wiki/Sega-CD)
*   [世嘉 SG-1000](https://github.com/retropie/retropie-setup/wiki/SG-1000)T3】
*   [超级任天堂娱乐系统](https://github.com/retropie/retropie-setup/wiki/Super-Nintendo-Entertainment-System)
*   [TI-99/4A](https://github.com/retropie/retropie-setup/wiki/TI-99)T3】
*   [TRS-80](https://github.com/retropie/retropie-setup/wiki/TRS-80)
*   [威格斯](https://github.com/retropie/retropie-setup/wiki/Vectrex)
*   [video PAC/odyssey 2](https://github.com/retropie/retropie-setup/wiki/VideoPac-Odyssey-2)T3】
*   [虚拟男孩](https://github.com/retropie/retropie-setup/wiki/Virtual-Boy)
*   [Wii](https://github.com/retropie/retropie-setup/wiki/Wii)
*   [【旺德万】](https://github.com/retropie/retropie-setup/wiki/WonderSwan)
*   [绝色](https://github.com/retropie/retropie-setup/wiki/Wonderswan-Color)
*   [Zmachine](https://github.com/retropie/retropie-setup/wiki/Zmachine)T3】
*   [ZX 谱](https://github.com/retropie/retropie-setup/wiki/ZX-Spectrum)

您还将获得多个针对特定游戏 的 [特殊端口，包括](https://github.com/RetroPie/RetroPie-Setup/wiki/Ports) [【雷神之锤】](https://github.com/RetroPie/RetroPie-Setup/wiki/Quake)[《我的世界》Pi](https://github.com/RetroPie/RetroPie-Setup/wiki/Minecraft)[保德之门](https://github.com/RetroPie/RetroPie-Setup/wiki/GemRB) 等等。

### **你需要什么**

在这里你不需要太多就可以开始:

*   [一个树莓派](http://www.amazon.com/Rasberry-Pi-Model-Mother-board/dp/B01CD5VC92/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192&asc_source=&ie=UTF8&keywords=raspberry pi 3&qid=1460750329&s=pc&sr=1-1&tag=kinjalifehackerlink-20) (我们推荐树莓派 3，因为你可以兼容完整的游戏以及内置的 Wi-Fi 和蓝牙。RetroPie 将在旧版本的 Raspberry Pi 上工作。
*   [微型 USB 电源](https://www.amazon.com/CanaKit-Raspberry-Supply-Adapter-Charger/dp/B00MARDJZ4/ref=sr_1_3?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192&asc_source=&ie=UTF8&keywords=raspberry pi usb power supply&qid=1486567676&sr=8-3&tag=kinjalifehackerlink-20) 。
*   至少一张 [8GB 的 Micro SD 卡](https://www.amazon.com/Samsung-Electronics-Adapter-MB-MP08DA-AM/dp/B00JEVHZPY/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192&asc_source=&ie=UTF8&keywords=samsung evo 8gb&qid=1486567769&sr=8-1&tag=kinjalifehackerlink-20) 。
*   USB 控制器(可选，但使整个事情更有趣。 [我们喜欢](https://lifehacker.com/the-best-controllers-for-retro-gaming-1791090209)[水牛经典 USB](https://www.amazon.com/Buffalo-Classic-USB-Gamepad-PC/dp/B002B9XB0E?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192&asc_source=&rawdata=[r|http://lifehacker.com/word-of-warning-i-got-the-nes30-pro-for-my-retropie-an-1791119934[t|link[p|1791090209[a|B002B9XB0E[au|5716493564230329059[b|lifehacker&tag=kinjalifehackerlink-20) ) RetroPie 也 [原生支持 PS 3/4 和 Xbox 360/One 控制器以及](https://github.com/petrockblog/RetroPie-Setup/wiki/RetroArch-Configuration) 。
*   一个 USB 键盘(仅用于初始设置，并且仅当您想要设置 Wi-Fi 时，之后您将不再需要它。当然，如果你在模拟电脑游戏，你可以用键盘和鼠标来控制它们。
*   电视/显示器，AV/HDMI 线缆(你可以在树莓 Pi 维基 上找到兼容 SD 卡、电源块和其他一切 [)的完整列表。](http://elinux.org/RPi_VerifiedPeripherals)
*   一台 Windows/Mac/Linux 电脑来设置您的 SD 卡并传输您的 rom。

### **第一步:在 SD 卡上下载并安装 retro pie**

因为有了 [RetroPie](https://retropie.org.uk/) 的工作，在你的树莓派上安装所有这些模拟器的过程变得异常简单:

1.  下载 [RetroPie 项目 SD 卡镜像](https://retropie.org.uk/download/) 用于您的树莓派版本(0/B/B+或 2/3)。对于本指南，我们使用的是 3.7 版。不过有一个警告，根据他们的服务器有多忙，这个吸盘可能需要一段时间来下载，所以给自己足够的时间。
2.  下载完成后，将图像解压到 SD 卡上，就像处理普通 Raspbian 图像一样。Windows 用户可以使用[win 32 diski manager](https://sourceforge.net/projects/win32diskimager/)非常轻松地做到这一点，Mac 用户可以使用 [RPI-sd 卡生成器](http://alltheware.wordpress.com/2012/12/11/easiest-way-sd-card-setup) 。Linux 用户必须学会一个非常简单的命令行技巧。无论哪种方式，看看我们的《树莓派狄莺入门指南》 ,并遵循与 Raspbian 相同的说明。
3.  完成后，取出 SD 卡，放入你的树莓派。

至于初始设置，这就是你需要做的。事实上，如果你打算用键盘和鼠标代替控制器，你基本上已经完成了，可以跳到第五步来传输你的 ROM 文件。

如果您喜欢手动安装模拟器，您也可以这样做。RetroPie Github 页面 有这样做的指南，但要注意:手动过程需要大约六到九个小时来下载和安装所有东西。好处是您可以获得最新版本的模拟器，并且可以选择安装什么。对于我们的目的来说，上面的方法非常有效，而且非常简单。

### **第二步:启动你的 Raspberry Pi 并设置仿真站**

接下来我们会启动你的树莓派。将您的一个控制器和键盘插入 Raspberry Pi。插入刚刻录的 SD 卡，打开树莓 Pi。经过几分钟的自动设置(它将扩展文件系统并准备一些其他的东西)，它将直接引导到 EmulationStation，这个接口包装器上有您所有的仿真器。在这里，您将设置您的控制器，并做一些其他调整来设置系统。

第一次启动时，按照屏幕上的提示使用控制器进行设置(向上、向下、向左、向右等)。如果您使用的是蓝牙控制器，请在此步骤中用 USB 电缆连接它。您可以稍后在下一步中设置蓝牙。

完成后，你可以用你的控制器在你的 RetroPie 中导航。这些控件将在模拟器和 RetroPie 本身中工作。除了控制基本动作之外，你还可以使用一些“热键”,这样你就可以在游戏中快速完成某些动作:

*   **选择+开始:**退出游戏
*   **选择+右肩**:保存
*   **选择+左肩**:加载
*   **选择+右键**:输入状态槽增加
*   **选择+左**:输入状态槽减少
*   **选择+X** : RGUI 菜单
*   **选择+B** :复位

并非所有这些快捷方式对每个人都有用，但你至少应该知道如何退出游戏，创建一个保存，并加载一个保存。

另一件值得注意的事情是，虽然 RetroPie 附带了大量的模拟器，**它隐藏了所有没有安装游戏的模拟器**。因此，当您第一次浏览 RetroPie 时，您会注意到没有模拟器可用。放心吧！事情应该是这样的。其他模拟器会在你添加游戏时出现。

### **第三步:设置无线网络**

最新版本的 RetroPie 有一个内置系统，你可以访问所有的 Raspberry Pi 设置，调整你的内存，等等。这些设置中的大部分是为高级用户设置的，但是有一个几乎每个人都想设置的是 Wi-Fi:

1.  向下滚动到配置 WiFi 选项并点击 A 按钮。
2.  选择“连接到 WiFi 网络”并选择您的网络。键入您的密码，然后选择确定。

这就是基本设置。如果你想再修修补补，这里就是你要做的地方。你可以编辑 RetroPie 的主题，设置无线蓝牙控制器(这因品牌而异，但 RetroPie GitHub 页面的有最流行选项的指南)，管理文件，以及这方面的更多内容。不过，在您对基础知识更加熟悉之前，这些东西大部分都不值得玩味。如果你对如何调整这些高级选项感兴趣，请查看我们的回溯指南。

### **第四步(可选):从你的主计算机转移你的 ROMs】**

对于这一步，我们将假设您的主计算机上已经有一堆 rom，您想将它们转移到您的 Raspberry Pi。这个超级容易做:

1.  确定您的 Raspberry Pi 已打开，并已连接到路由器。
2.  RetroPi 文件夹应该自动显示为共享文件夹。如果没有，可以手动加载。从窗口打开文件管理器，在文件夹位置输入`\\retropie`。在 Mac 上，打开 finder 并选择前往>连接到服务器。输入`smb://retropie`并点击连接。

从现在开始，您将能够通过这种方法轻松地将 rom 远程复制到 Raspberry Pi，所以如果您想添加更多内容，请不要担心。一旦文件传输完成，重启 Raspberry Pi。

如果你喜欢使用一个装满 rom 的 USB 驱动器，你也可以这样做。只需将它们转储到 USB 驱动器上名为`retropie`的文件夹中，然后将其插入您的 Pi。

*<small>视频中的音乐由</small>*[*<small>RoccoW</small>*](http://freemusicarchive.org/music/RoccoW/~/Hello_Chiptune_Cover)*<small>组成。</small>T15】*