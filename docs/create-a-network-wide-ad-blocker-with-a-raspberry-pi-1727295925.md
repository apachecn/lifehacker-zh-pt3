# 用树莓派创建一个网络广告拦截器

> 原文：<https://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925>

你有在电脑上屏蔽广告的软件，但如果你想屏蔽所有设备上的广告——从智能手机到平板电脑——你需要更强大的软件。进入 Pi-Hole，这是一个树莓 Pi 图像，可以在路由器级别阻止各种广告。

Watch

有些广告是令人讨厌的，但请记住:广告是我们这样的网站赚足够的钱来运营的方式，所以除非你想看到所有你喜欢的网站倒闭，否则我们谦恭地提醒你把你喜欢的网站列入白名单。

一旦你设置了这个漏洞，广告甚至在到达你的电脑、智能手机或家庭网络上的任何其他设备之前就被屏蔽了。除了将你的浏览器从运行另一个扩展中解放出来，这应该会加快你的浏览速度，减少加载时间(它甚至应该会删除像 iOS 和 Android 中那些烦人的游戏内广告之类的东西)。只有当设备连接到您的家庭网络时，这才会起作用，因此如果您离开房子，屏蔽将不再起作用，但如果您不喜欢广告，它仍然有用。幸运的是，开发人员 [雅各布·萨尔梅拉](http://jacobsalmela.com/) 有一个预先配置好的 Pi 镜像，很容易安装和设置。有了它，您的 Pi 会自动设置，您只需更改设备上的一些设置。

### 你需要什么

*   (任何型号)
*   [SD 卡](http://www.amazon.com/Sandisk-MicroSDHC-Memory-Adapter-Packaging/dp/B000SMVQK8/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925&asc_source=&ie=UTF8&keywords=microsd card 4gb&qid=1440791474&s=pc&sr=1-1&tag=kinjalifehackerlink-20) 和读卡器
*   [电源](http://www.amazon.com/NorthPada-Supply-Charger-2000mA-Raspberry/dp/B00OY7HR1U/ref=pd_sim_147_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925&asc_source=&ie=UTF8&refRID=11Z60FPZHT91KZS90MNS&tag=kinjalifehackerlink-20)
*   [以太网线](http://www.amazon.com/Mediabridge-Cat5e-Ethernet-Patch-Cable/dp/B00EUHRLF6/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925&asc_source=&ie=UTF8&keywords=ethernet cable&qid=1440791456&s=pc&sr=1-1&tag=kinjalifehackerlink-20)
*   [键盘](http://www.amazon.com/Inland-USB-standard-Keyboard-70010/dp/B0075W8C1K/ref=sr_1_11?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925&asc_source=&ie=UTF8&keywords=usb keyboard&qid=1440791519&refinements=p_85:2470955011&s=pc&sr=1-11&tag=kinjalifehackerlink-20) (用于初始设置)

### 第一步:下载并刻录 Pi-Hole 映像

您需要做的第一件事是下载并刻录 Pi-Hole 映像。图像是一个名为 [**Diet Pi**](https://www.raspberrypi.org/forums/viewtopic.php?f=63&t=100976) 的 Raspbian 操作系统版本，它从 Raspbian 中削减了大量垃圾，并打包了运行广告拦截器所需的所有软件。你可以按照我们的指南在这里制作一个图像，这里是简短的版本。

#### **窗户**

1.  [下载预先配置好的 Pi-Hole 镜像](https://dl.dropboxusercontent.com/u/16366947/Pi-hole/Pi-hole-DietPi-Fork-2015-08.zip) 并解压。img 文件在里面。
2.  [下载 win32 diski manager](https://launchpad.net/win32-image-writer/+download)并解压应用程序(。exe 文件)中。
3.  将读卡器连接到 Windows PC 并插入 SD 卡。
4.  双击打开您刚刚下载的应用程序“Win32DiskImager.exe”。如果你运行的是 Windows 7、8 或 10，右击它，选择“以管理员身份运行”。
5.  如果应用程序没有自动检测到您的 SD 卡，请单击右上方的下拉菜单(标有“设备”)并从列表中选择它。
6.  在应用程序的图像文件部分，单击小文件夹图标并选择 Pi-Hole。您刚刚下载的 img 文件。
7.  单击 Write 按钮，等待 Win32DiskImager 完成它的工作。完成后，您可以安全地弹出您的 SD 卡，并将其插入您的 Raspberry Pi。

#### **OS X**

1.  [从这里下载预先配置好的 Pi-Hole 镜像](https://dl.dropboxusercontent.com/u/16366947/Pi-hole/Pi-hole-DietPi-Fork-2015-08.zip) 并解压。img 文件在里面。
2.  [下载 RPi-sd 卡构建器](http://alltheware.wordpress.com/2012/12/11/easiest-way-sd-card-setup) (一定要为你安装的 OS X 版本选择合适的版本)并解压应用程序。
3.  将读卡器连接到 Mac(如有必要)并插入 SD 卡。
4.  打开 RPi-sd 卡生成器。您将立即被要求选择一个 Pi-Hole 图像。选择。您之前下载的 img 文件。
5.  系统会询问您是否连接了 SD 卡。因为我们之前插入了它，所以它是，所以继续并单击 Continue。您将看到 SD 卡选项。如果您只插入了一个，您将不会在列表中看到任何其他内容，它将被检查。如果没有，只需检查您想要使用的卡，然后单击确定。
6.  输入您的管理员密码，然后单击确定。
7.  您将被询问 SD 卡是否被弹出。这是应该发生的，因为应用程序需要卸载它来执行直接拷贝。仔细检查您的 SD 卡在 Finder 中是否不再可用。不要将其从 USB 端口或读卡器上移除。确定后，点按“继续”。
8.  RPi-sd 卡生成器将完成准备您的 sd 卡。安全弹出它，并将其插入到您的树莓派。

### 第二步:启动并配置您的树莓派

将您的 SD 卡插入您的 Raspberry Pi 并连接键盘。将以太网电缆连接到 Wi-Fi 路由器，然后插入 Raspberry Pi，等待它启动。

当你第一次启动你的树莓派，它会启动和重启几次。这很正常，就顺其自然吧。在很大程度上，它在进行基本的设置过程，比如扩展文件系统和配置网络设置。最终，它将引导至登录屏幕。

使用**用户名:** *root* 和**密码:** *dietpi* 登录。一旦你这样做了，你的 Raspberry Pi 将会检查并可能下载一组更新，所以也请耐心等待。完成后，你需要重新启动，然后登录。

### 第三步:为您的 Pi 设置一个静态 IP 地址

在所有这些重启之后，您将最终到达 DietPi 设置屏幕，在这里您可以分配一个静态 IP 地址。这是必要的，这样您的 Pi 将始终可以从您的任何设备的同一地址获得。以下是你需要做的:

1.  在初始设置屏幕中选择确定。
2.  选择更改有线网络设置。
3.  选择更改模式并按 Enter 键将其更改为静态。
4.  选择将当前地址复制到静态。记下顶部列出的 IP 地址，在下一步中会用到。
5.  选择应用以保存更改并重启网络。
6.  完成后，选择退出再次重启设备。

配置网络设置后，您的 Pi 将再次重启。接下来，安装 Pi-Hole 软件(这可能需要一段时间，对我来说大约需要 20-30 分钟)，然后最后一次重启。一旦它重新启动，广告拦截软件将自动运行，所以你需要做的就是设置你的电脑。

### 第四步:将您的设备指向用于 DNS 的树莓 Pi

一旦你的 Raspberry Pi 运行了 Pi-Hole 软件，你仍然需要通过它来路由你的设备流量，这样广告拦截才会起作用。为此，您需要更改设备的 DNS 设置。这样，只要广告都在同一个网络上，你的设备就可以 ping Pi 来阻止广告。这非常简单，但会根据您的设备及其运行的内容而有所不同。

#### **窗户**

1.  右键单击开始按钮并选择网络连接。
2.  选择您的 Wi-Fi 或以太网。
3.  双击 Internet 协议版本 4。
4.  单击使用下列 DNS 服务器地址。
5.  在首选 DNS 服务器下，输入您在第三步中收集的 Raspberry Pi 的 IP 地址。

#### **OS X**

1.  打开“系统偏好设置”。
2.  点击网络。
3.  选择您的 Wi-Fi 或以太网。
4.  点击高级。
5.  单击 DNS 选项卡。
6.  点击加号并输入您在第三步中收集的 Raspberry Pi 的 IP 地址。

#### **安卓**

1.  打开设置。
2.  选择 Wi-Fi。
3.  长按当前网络并选择修改网络。
4.  轻按“显示高级选项”。
5.  将 IP 设置更改为静态。
6.  在 DNS 字段下输入您的 Raspberry Pi 的 IP 地址。

#### **iOS**

1.  打开设置。
2.  选择 Wi-Fi 并点击您的家庭网络。
3.  点击 DNS 并输入您的 Raspberry Pi 的 IP 地址。

你也可以点击`[RaspberryPiIPaddress]/pihole/index.php`来追踪 Pio-Hole 在屏蔽广告方面的表现

在这里，你会看到统计数据和其他信息。

### 白名单网站

默认情况下，Pi-Hole 会阻止很多网站，但是您可以将您最喜欢的网站列入白名单，尽管现在有点复杂。首先，你需要回到你的树莓派。当您启动 Raspberry Pi 并登录时，您将自动进入命令行。在这里，您可以创建并编辑一个文本文件，其中包含您希望**而不是**阻止广告的网站:

1.  在 Raspberry Pi 的命令行中，键入`cd /etc/pihole/`
2.  键入`nano whitelist.txt`打开一个空白文本文件。
3.  键入您不想阻止广告的任何网站的 URL。在每个条目之间按 Enter 键，将每个条目放在一个新行上。使用`www.site.com`和`site.com`访问您不想阻止的网站。
4.  按 CTRL+X 保存并退出。
5.  重新启动 Raspberry Pi，更改将生效。

未来的更新还承诺从上述索引屏幕编辑白名单和黑名单的能力，所以请密切关注。为了更深入地了解如何创建你自己的白名单和黑名单，你 [可以遵循这个指南](http://jacobsalmela.com/block-millions-ads-network-wide-with-a-raspberry-pi-hole-2-0/#blockmalware) 。