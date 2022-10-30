# 如何从任何使用 VNC 的电脑上控制你的树莓派

> 原文：<https://lifehacker.com/how-to-control-your-raspberry-pi-from-any-computer-usin-1788592777>



售价 35 美元的 Raspberry Pi 是一台非常棒的小电脑，但是如果加上显示器、鼠标和键盘的成本，价格就有点贵了。还好你并不真的需要它们。有了 VNC，您可以从笔记本电脑或台式电脑访问您的 Pi，只需使用您一直使用的鼠标、键盘和显示器，无需重新布线。



### 第一步:在你的 Windows 或 Mac 电脑上下载 VNC 浏览器

你有很多不同的 VNC 软件选项，但我们发现 VNC 浏览器是最容易使用的，与树莓派配合使用。从你的 PC 或 Mac 电脑(以及 [、iPhone](https://itunes.apple.com/us/app/vnc-viewer/id352019548?mt=8) 或[Android](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=en))[上 RealVNC 的 VNC 浏览器](https://www.realvnc.com/download/viewer/) ，点击你的操作系统的下载按钮，然后下载免费应用程序。

### 第二步:使用 SSH 或终端启动 VNC 服务器

VNC 服务器包含在 Raspbian 的最新版本 [、PIXEL](https://lifehacker.com/the-new-raspberry-pi-os-is-here-and-it-looks-great-1787194540) 中，所以我们在这里需要做的就是启动一个服务器。如果你使用的是旧版本的 Raspbian 或者完全不同的操作系统， [这个由 Raspberry Pi 基金会提供的指南](https://www.raspberrypi.org/documentation/remote-access/vnc/) 会告诉你如何下载和安装它。

我们假设您想要设置 VNC，因为您没有额外的显示器、鼠标和键盘。因此，最好的方法是使用安全外壳(SSH)。SSH 允许您在任何计算机上使用命令行来控制您的 Raspberry Pi。第一次启动 VNC 服务器时，您需要这样做。

1.  给你的 Raspberry Pi 加电，用以太网电缆把它插到路由器上。
2.  为你的操作系统下载并安装 [Adafruit 的圆周率查找器](https://github.com/adafruit/Adafruit-Pi-Finder) 。下载完成后，启动应用程序并点击“查找我的 Pi”按钮。
3.  Pi Finder 将在您的网络上搜索树莓 Pi。让它做它的事情。最终，它会显示你的树莓派的 IP 地址。确保用户设置为`pi`，密码设置为`raspberry`(假设您没有更改这些默认值，也就是说，输入您自己的凭证)，然后单击终端按钮。
4.  这将使您登录到 Raspberry Pi 的命令行，在这里您可以启动与您的 Pi 打包在一起的 VNC 服务器。在命令行提示符下，键入:`vncserver`并按 Enter 键。这会运行一个命令，并在 Raspberry Pi 上启动 VNC 服务器。在命令的结尾，你会看到一个类似于上图的注释，写着“新桌面是`raspberrypi:1`”，后面是一个包括 Pi 的 IP 地址的数字，比如(`192.168.0.19:1`)。记下这个号码，你将需要它从你的电脑登录到 VNC 服务器。

现在 VNC 服务器正在运行，您可以从您的另一台计算机登录到它。

### 第三步:从你的电脑登录 VNC 服务器

现在是时候登录 VNC 服务器了:

1.  在 PC 或 Mac 上，双击在第一步中下载的 VNC 查看器应用程序。
2.  在 VNC 服务器框中，键入您在上一步中记下的号码，如`192.168.0.19:1`，然后单击连接。
3.  输入`pi`作为用户名，输入`raspberry`作为密码，然后点击 OK。

在几秒钟内，VNC 浏览器应该会显示您的树莓派的桌面环境。现在，您可以控制您的 Raspberry Pi，就像您正坐在它面前，使用键盘、鼠标和显示器连接到实际的 Pi 一样。

### 第四步:设置 VNC 自动启动

除非你想在每次使用 Raspberry Pi 时都经历第二步中概述的过程，否则你会希望将 VNC 服务器设置为在启动时自动运行。这很容易做到:

1.  在 Raspberry Pi 的桌面环境中，单击终端图标打开命令行。
2.  输入`sudo raspi-config`并按回车键。
3.  使用箭头键向下滚动到高级选项，然后按 Enter 键。
4.  向下滚动到 VNC 服务器，然后按回车键。
5.  选择是并按回车键。

就这样，现在 VNC 服务器应该会自动启动。一旦设置好 VNC，你就可以像使用第二台电脑一样使用你的树莓派，不管它插在哪里。当你只有一台笔记本电脑，不想为了使用 35 美元的树莓派而购买一整套配件时，或者如果你只需要在项目的短暂时间内访问用户界面，不想一直经历设置一切的繁琐时，VNC 非常有用。