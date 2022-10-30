# 新的 Raspberry Pi 操作系统在这里，它看起来很棒

> 原文：<https://lifehacker.com/the-new-raspberry-pi-os-is-here-and-it-looks-great-1787194540>

树莓派的主要操作系统 Raspbian 刚刚从 [树莓派基金会](https://www.raspberrypi.org/blog/introducing-pixel/) 获得了全新的外观。它被称为 PIXEL，是 Raspbian 的一个皮肤，使界面现代化，增加了一些新程序，使用起来更加舒适。你甚至可以在你的电脑或者苹果电脑上运行。让我们仔细看看你的 Pi 的新外观。



### 新的闪屏取代了旧的神秘的引导信息

你将看到的第一个大变化是当你启动你的 Raspberry Pi 时缺少了长字符串。取而代之的是一个闪屏，显示操作系统和版本号，就像你在其他现代电脑上看到的一样。否则，整个引导时间和过程保持不变。

### **PIXEL 预装了 RealVNC、Chromium 等等**

PIXEL 还增加了几个值得注意的新默认程序。最大的新 app 是 [铬](https://www.chromium.org/) ，取代了老化的 [顿悟网页浏览器](https://www.raspberrypi.org/blog/web-browser-released/) 。这是 Chromium 的第一个版本，专门为 Pi 构建，使用 Pi 的硬件来加速视频播放。Chromium 安装了几个扩展，包括用于阻止广告的 [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en) ，以及用于提高 Pi 上 YouTube 视频质量的 [h264ify 扩展](https://chrome.google.com/webstore/detail/h264ify/aleakchihdccplidncghkekgioiakgal?hl=en-US) 。Chromium 最适用于 Raspberry Pi 2 和 3，但也适用于 Pi 1 和 Pi Zero。

[RealVNC](http://www.realvnc.com/raspberrypi) 包含在内，因此您可以轻松地从远程桌面使用树莓 Pi，开箱即用。如果你以前从未在你的 Pi 上使用过 RealVNC， [设置非常简单](https://www.realvnc.com/docs/raspberry-pi.html) 。如果您只有一台笔记本电脑，并且不想购买键盘、鼠标和显示器，那么 RealVNC 是访问您的 Pi 的一个好方法。

还有一个新的 [SenseHAT 模拟器](https://www.raspberrypi.org/blog/desktop-sense-hat-emulator/) ，让你可以测试 [SenseHAT 外设](https://www.raspberrypi.org/products/sense-hat/) 的想法。模拟器允许你调整陀螺仪、温度、屏幕等等。

### PIXEL 自带一堆好看的壁纸

这听起来可能不太像，但考虑到 Raspbian 的默认背景一直是空白或树莓 Pi 标志，PIXEL 附带一堆壁纸真的很好。其中包括树莓派开发者之一格雷格·安南代尔的 16 张照片。您可以通过单击 Pi 徽标>首选项>外观设置来访问它们。

当然，你总是可以使用你自己的壁纸，但是当你第一次穿上靴子的时候看到一张照片会更好。

### 像素具有所有新的应用图标，新的温度和电压图标

你可能不经常考虑图标的质量，但是 Rapsbian 中的图标总是有点欠缺。他们是单调的，有时像素化和模糊的，看起来有点泥泞。现在，它们更有活力，更容易一目了然。

[神秘的彩虹显示屏](https://lifehacker.com/what-the-raspberry-pis-rainbow-boot-screen-and-rainbow-1768470271) 也不见了，它会警告您的 Pi 是否欠压或过热。取而代之的是表示电压的闪电和表示温度的温度计，这将使故障排除变得容易得多。

### 每个窗口都有一个干净的圆形标题栏

在 Raspbian 以前的版本中，窗口是块状的正方形，总是让系统看起来过时。现在，它看起来更现代了，有了圆角、新的标题栏和新的关闭/最小化/最大化按钮。这是一个小变化，但总体上看起来好多了。

### 您可以轻松禁用 Wi-Fi 或蓝牙

如果你不需要 Wi-Fi 或蓝牙，打开它们会很快耗尽电量，如果你正在进行一个使用电池组的项目，这是一个问题。PIXEL 为 Wi-Fi 和蓝牙添加了一个新菜单，使关闭它们变得更加容易。只需点击图标，点击关闭按钮，你就一切就绪了。

### 如何更新当前版本的 Raspbian

从现在开始，PIXEL 将成为 Raspberry Pi 基金会的主要操作系统。如果您已经安装并运行了 Raspbian，您可以通过加载命令行并键入以下命令将其更新到此版本:

```
sudo apt-get update 
sudo apt-get dist-upgrade 
sudo apt-get install -y rpi-chromium-mods 
sudo apt-get install -y python-sense-emu python3-sense-emu 
sudo apt-get install -y python-sense-emu-doc realvnc-vnc-viewer

```

如果你喜欢从零开始，刻录一张新的图像，你可以从 [Raspberry Pi 基金会的下载页面](https://www.raspberrypi.org/downloads/) 获得 PIXEL。