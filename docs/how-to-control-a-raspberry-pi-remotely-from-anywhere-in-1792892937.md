# 如何从世界任何地方远程控制树莓派

> 原文：<https://lifehacker.com/how-to-control-a-raspberry-pi-remotely-from-anywhere-in-1792892937>

你是否希望在旅途中也能使用你的树莓派？也许你已经安装了一个家庭安全摄像头，你正在运行一个私人的《我的世界》服务器，或者你正在使用你的 Pi 进行一些你自己制造的疯狂的网络设备。无论您原因是什么，远程访问树莓 Pi 都比您想象的要容易。以下是方法。



要从家庭网络之外访问 Raspberry Pi(或任何家用电脑),通常需要通过许多关卡，获得一个 IP 地址，并调整家庭路由器上的一些设置。如果你只需要在你的树莓 Pi 上控制几个简单的东西，那就大材小用了。我们将概述两种跳过所有这些的方法。

你需要做的第一件事就是设置好你的 [树莓派，并连接到你的家庭网络](https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054) 。既然你要把你的树莓派暴露在互联网上，确保你在设置过程中 [更改了你的默认密码](https://www.raspberrypi.org/documentation/linux/usage/users.md) 。一旦完成，回到这里设置其他一切。

### 使用 VNC 连接远程登录您的 Raspberry Pi 的完整操作系统

VNC 一直是远程访问同一网络 上任何 [电脑的最佳方式。最近，](https://lifehacker.com/how-to-control-your-raspberry-pi-from-any-computer-usin-1788592777)[【VNC 连接】问世，使得使用云连接从*任何地方*访问](http://lifehacker.com/you-can-now-easily-connect-to-your-raspberry-pi-from-an-1792438276) 你的树莓派变得简单。设置完成后，您可以使用 [VNC 浏览器应用](https://www.realvnc.com/download/viewer/raspberrypi/) 从任何其他电脑或智能手机访问您的 Raspberry Pi 图形界面。

VNC 连接免费提供最新版本的树莓 Pi 操作系统，。如果你已经有了，你可以跳过这一部分。如果没有，您可以安装它，并通过在您的 Raspberry Pi 上打开终端并键入几个命令来打开它:

1.  输入`sudo apt-get update`并按回车键。
2.  输入`sudo apt-get install realvnc-vnc-server realvnc-vnc-viewer`并按回车键。
3.  一旦完成，输入`sudo raspi-config`并按回车键。向下滚动到 VNC，并将其设置为启用。

下载完成后，您可以设置 VNC 连接:

1.  前往 [RealVNC Raspberry Pi 注册页面](https://www.realvnc.com/raspberrypi/#sign-up) 并在注册框中输入您的电子邮件地址。
2.  按照屏幕上的说明完成设置您的帐户密码。
3.  回到你的 Raspberry Pi，点击屏幕右上角的 VNC 图标打开 VNC。然后单击状态菜单并选择许可。
4.  输入您在第一步中创建的电子邮件地址和密码。
5.  出现提示时，选择“直接和云连接”你的树莓派现在可以在线使用了。
6.  从下载 [VNC 浏览器应用](https://www.realvnc.com/download/viewer/) 到你想要控制树莓派*的电脑上，就像你旅行时会有的笔记本电脑或智能手机。*
7.  打开 VNC 查看器应用程序，并输入您在步骤 1 中创建的凭据。
8.  你的树莓派会自动弹出一个选项。选择它以打开连接。出现提示时，输入您的 Raspberry Pi 的用户名和密码(默认情况下是用户名`pi`和密码`raspberry`)。几秒钟之内它就会连接上。

现在，只要您的 Raspberry Pi 可以访问互联网，您就可以从任何地方登录您的 Raspberry Pi 图形桌面。这意味着你可以控制任何安全软件，检查你建立的任何项目的状态，或者在你的私人服务器 上 [玩《我的世界》。](http://lifehacker.com/learn-all-kind-of-coding-skills-using-a-raspberry-pi-an-1784535192)

### 使用 Dataplicity 访问命令行

如果你不需要访问完整的图形界面，那么你会想要查看。Dataplicity 使得从任何浏览器访问您的 Raspberry Pi 命令行变得非常容易。为此，您需要访问网络浏览器和您的 Raspberry Pi。

1.  进入 [数据政策](https://www.dataplicity.com) ，输入您的电子邮件地址创建一个账户。
2.  单击添加新设备。
3.  Dataplicity 将显示一行代码，如上图所示。复制该行代码，并将其输入到您的 Raspberry Pi 的命令行中。你可以在你的 Raspberry Pi 上这样做，方法是选择打开终端应用程序，或者使用类似于 [Adafruit 的 Pi Finder](https://github.com/adafruit/Adafruit-Pi-Finder) 这样的工具通过 SSH 在你的家庭网络上远程访问它 [。几秒钟后，Dataplicity 将下载并安装软件到您的 Raspberry Pi 上，直接链接到您的帐户。](https://lifehacker.com/how-to-control-your-raspberry-pi-from-any-computer-usin-1788592777)
4.  完成后，进入 [数据策略设备页面](https://www.dataplicity.com/devices/) 。在这里，你会看到你的覆盆子酱。点击它打开一个终端窗口。
5.  现在，你可以重启并重命名你的 Raspberry Pi，仅此而已。如果你只是需要远程重启它，让它保持原样。如果你需要做更多的事情，比如安装软件或者编辑文件，你可以以超级用户的身份登录。为此，在 Dataplicity 命令行中，键入，`su pi`并按 Enter 键。然后，输入您的 Raspberry Pi 的密码，并按回车键。现在你可以完全控制你的树莓派。

就这样，只要连接互联网，您就可以在世界任何地方访问您的树莓派。显然，您的 Raspberry Pi 需要保持通电，但除此之外，您可以从任何浏览器访问它。有了这个小小的功能，你可以开箱即用地做一件*吨*的事情，包括:托管一个 [小网站](https://docs.dataplicity.com/docs/host-a-website-from-your-pi) 、 [共享文件](https://docs.dataplicity.com/docs/share-files-from-your-pi) 、 [甚至流媒体视频](https://docs.dataplicity.com/docs/stream-live-video-from-your-pi) 。