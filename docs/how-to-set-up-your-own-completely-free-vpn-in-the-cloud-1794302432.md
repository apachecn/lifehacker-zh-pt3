# 如何在云中搭建自己完全免费的 VPN

> 原文：<https://lifehacker.com/how-to-set-up-your-own-completely-free-vpn-in-the-cloud-1794302432>

虚拟专用网络(VPN) [是给你的浏览增加安全](https://lifehacker.com/why-you-should-be-using-a-vpn-and-how-to-choose-one-5940565) 的好方法，同时还能防止窥探( [包括你的互联网服务提供商](http://lifehacker.com/why-is-everyone-talking-about-vpns-1793768312) )，但是 [VPN 提供商是出了名的粗略](https://lifehacker.com/how-do-i-know-if-my-vpn-is-trustworthy-508866499) 。你可以做一些研究来找到一个好的。或者你可以在 10 分钟内自己做。



快速复习一下，VPN 会在数据离开您的设备之前对其进行加密，然后数据在通过您的本地网络和互联网服务提供商(ISP)时保持加密状态，直到最终被 VPN 服务器解密。在这种情况下，您将在 web 服务上安装 VPN 软件。

商业 VPN 更容易建立，虽然这个项目不是非常复杂，但你确实需要在技术上有所倾向。由于设置不佳的 VPN 毫无用处，我建议坚持使用知名公司的商业选项，如[slick VPN](https://www.slickvpn.com/)[nord VPN、](https://nordvpn.com/)[Hideman](https://www.hideman.net/)或 [Tunnelbear](https://www.tunnelbear.com/) (如果你不习惯自己设置的话)。对于其他熟悉命令行用法的人，让我们开始吧。

### 你有什么

也就是说，你会得到一个免费的 VPN。这意味着您的计算机或移动设备与互联网之间的安全、加密连接。如果你对你的 ISP 可以看到你在网上做的一切感到恼火，或者当你在咖啡店 时，你想要一个安全的互联网连接，那么你想使用 VPN。

多年来，我们强调了许多公共 VPN 提供商， [包括最近的](http://gear.lifehacker.com/the-best-vpn-service-is-private-internet-access-1794083573) [私人互联网接入](https://www.privateinternetaccess.com/) ，但是任何提供商都有一个普遍的问题，那就是很难说他们在保护你的私人数据隐私方面有多忠诚。所以，下一个合乎逻辑的步骤是做出你自己的。有几个不同的项目可以这样做，但我选定了 [Algo](https://github.com/trailofbits/algo) 因为它似乎是所有项目中最简单的。它在几个不同的云竞争服务中的一个上安装 VPN 软件，你可以从你的任何一台电脑上连接到它。

还有一个，包括 [【史翠珊】](https://github.com/jlund/streisand) ，它通过集成 Tor 桥和其他一些专注于隐私的功能，将 VPN 的想法向前推进了一步。史翠珊很棒，但对我们大多数人来说太过了。然而，如果你对史翠珊的额外隐私和安全功能更感兴趣，设置过程的第一步几乎与 Algo 相同，因此本指南的第一步将带你度过设置亚马逊 EC2 服务的困惑部分。之后， [按照史翠珊的指令](https://github.com/jlund/streisand) 进行你的操作系统。

最后，在我们开始之前，Algo 不会匿名浏览你的网页，也不会保护你的数据不被法律或政府机构获取。从理论上讲，政府可以向托管服务提供商(在这种情况下是亚马逊)索要你的账单信息。这意味着你的流量可以追溯到你。当然，他们也可以通过任何商业 VPN 提供商做到这一点。但是，至少这其中的 VPN 部分是完全由你自己负责的。它也是相对一次性的，所以一旦你掌握了这个过程，你可以很快地安装或破坏这个吸盘。

无论如何，算法保护和加密你的连接，这对我们大多数人来说已经足够了。如果你不愿意把钱支付给一个匿名的、随机的 VPN 提供商，这是最好的解决方案。



### 第一步:注册一个亚马逊 EC2 账户

可以在 [【数字海洋】](https://www.digitalocean.com/)[亚马逊 EC2](https://aws.amazon.com/ec2/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-set-up-your-own-completely-free-vpn-in-the-cloud-1794302432&asc_source=&tag=kinjalifehackerlink-20)[谷歌计算引擎](https://cloud.google.com/compute/)[微软 Azure](https://azure.microsoft.com/en-us/) 上安装 Algo。如果你是新用户，你可以使用亚马逊的 EC2 免费层一整年，所以我们将在这里详细说明这个过程。

但是这里有一些限制。首先，你每个月有 750 个小时，这对于一台设备来说应该是绰绰有余的，但是如果你有多台设备的话，这可能会增加。第二，你被限制在每月 15GB 的带宽，如果你下载了很多大文件，这可能是不够的。第三，在一年结束后，价格切换到小时费率。尽管如此，大多数人不应该期望每月支付超过 10-11 美元。

如果这种不可预测性令人讨厌，并且你宁愿跳过免费的一年而喜欢价格更可靠的东西，我建议使用数字海洋的 5 美元/月等级 T3。DigitalOcean 的设置也相当容易。使用默认设置创建一个新的 Droplet，然后点按“API”标签并生成一个新令牌。在 Algo 安装过程中，您将需要该号码。之后，你可以直接跳到下面的算法步骤。

但是，我们都喜欢免费，所以让我们继续亚马逊:

1.  前往亚马逊网站创建一个免费账户。如果你愿意，你可以将你当前的亚马逊账户链接到你的网络服务账户。
2.  登录后，点按“服务”>“IAM”。它位于“安全性、身份和合规性”选项卡下。
3.  单击左侧的“用户”选项卡。
4.  单击添加用户。
5.  创建一个用户名，然后单击编程访问旁边的框。然后单击下一步。
6.  单击直接附加现有策略。
7.  键入“admin”搜索政策。找到“AdministratorAccess”并点击旁边的复选框。完成后，单击下一步。
8.  在最后一个屏幕上，单击下载 CSV 按钮。这个文件包括一些数字和访问键，你需要在算法设置过程中使用。点击关闭，一切就绪。

现在，你的免费服务已经在亚马逊上运行了。是时候装 Algo 了。

### 第二步:下载并安装算法

接下来，我们将安装 Algo。您将在家中的 Windows、Mac 或 Linux 计算机上使用命令行来完成此操作。如果你使用的是 Linux 或 Mac，请直接跳到下面的第二部分。如果您使用的是 Windows，请继续。

#### 第一部分:Windows 10 用户(Mac 用户可以跳过这一步)

Windows 用户将需要为 Algo 安装 Windows 子系统 for Linux，该子系统*仅在 Windows 10(周年更新或更高版本)上提供*。你需要做的是:

1.  打开设置。
2.  单击“更新与安全”,然后单击“开发人员”。
3.  将“开发者模式”选项设置为“已启用”。
4.  安装完成后，单击控制面板，然后选择程序。
5.  单击打开或关闭 Windows 功能。
6.  向下滚动，然后滚动 Linux 的 Windows 子系统旁边的框，然后单击确定。Windows 将安装软件，然后重新启动。

现在，您已经安装了 Linux Bash。点击开始菜单，输入“Bash”你还会被问几个问题。回答这些问题，然后 Windows 将安装另一套软件。最后，一旦完成，您将在命令行。键入以下内容，然后按回车键:

```
sudo apt-get update && sudo apt-get install python-pip python-setuptools build-essential libssl-dev libffi-dev python-dev python-virtualenv git -y
```

然后，使用以下命令克隆存储库:

```
git clone https://github.com/trailofbits/algo && cd algo
```

完成后，跳到下面第二部分的第五步。

#### 第二部分:安装算法

在 Mac 上，你可以很容易地安装算法。然而，根据您运行的 Linux 版本，这里会有一组不同的命令。你可以在这里 算出 Linux 需要的 [。](https://github.com/trailofbits/algo)

1.  一台苹果电脑， [下载 Algo](https://github.com/trailofbits/algo/archive/master.zip) 并把文件解压到你机器上任何你想解压的地方。这将创建一个名为`algo-master`的文件夹。
2.  打开终端，然后键入`cd`，后跟“algo-master”目录位置。如果你不确定，输入`cd`，然后将 algo-master 目录拖放到终端。它会自动填充位置，产生类似于`cd /Users/jimbojones/Documents/algo-master`的结果。
3.  输入`python -m ensurepip —user`并按回车键。
4.  输入`python -m pip install —user —upgrade virtualenv`并按回车键。
5.  输入`python -m virtualenv env && source env/bin/activate && python -m pip install -r requirements.txt`并按回车键。如果您以前没有安装 cc 命令行工具，您将得到提示进行安装。去同意吧。
6.  输入`sudo nano config.cfg`并按回车键。这将打开一个文本编辑器。在“用户”下，键入您想要创建的任何用户的名称。这些都是您希望有权访问您的 VPN 的不同的人，所以如果您正在与朋友或在多个设备上共享，请创建其中的几个人。完成后，按 Ctrl+X 保存并退出。
7.  键入`./algo`开始安装过程。安装脚本会询问您一系列问题。
8.  对于提供商，输入亚马逊 EC2 的`2`(除非你选择了不同的提供商)。为您的 VPN 键入任意名称，并选择服务器位置(我建议使用最近的可用服务器)。
9.  接下来，您需要获取 AWS 访问密钥和 AWS 秘密密钥。还记得上一步中从 Amazon 下载的凭证 CSV 文件吗？包括这两个数字。当你被要求的时候，继续从那个文件复制/粘贴每个数字。
10.  接下来，Algo 问你关于 VPN 点播的问题。这两个问题我都回答了。这会使您的 Apple 设备自动连接到 VPN。否则，您每次都必须手动启用它们。我还建议对安全性增强、HTTP 代理和本地 DNS 解析器说是。剩下的选项完全由你决定，你可以对任何事情说不，你的 VPN 仍然可以正常工作。

最后，在所有这些之后，Algo 将进入世界并安装在你的提供商上，然后建立大量不同的服务，最终给你放行它的完成。您的 VPN 现在已启动并运行。您需要将设备连接到它才能使用它。

### 为您的 VPN 配置您的设备

为了连接到您的 VPN，您需要在想要连接到 VPN 的每台设备上安装描述文件或证书。这对于某些操作系统来说比其他操作系统更复杂。不管怎样，你需要的所有文件都在“configs”文件夹下的“algo-master”目录中。

#### 在 Apple 设备上设置 VPN

在“configs”文件夹中，您会找到一个. mobileconfig 文件。在 Mac 上，连按该文件以在 Mac 上安装描述文件。要在 iPhone 或 iPad 上安装描述文件，你可以将相同的文件从 Mac 空投到 iOS 设备，通过电子邮件发送给自己，或者上传到云服务，如 iCloud 或 Dropbox，然后从那里打开它。您将被要求确认描述文件安装，从那时起，您将连接到该 VPN。您可以通过删除配置文件来断开连接。

#### 在 Android 设备上设置 VPN

在 Android 上，需要先安装 [strongSwan VPN 客户端 app](https://play.google.com/store/apps/details?id=org.strongswan.android) 。然后，将 Configs 文件夹中的 P12 文件复制到您的 Android 设备上，并在 strongSwan 中打开它。按照那里的指示进行设置。如果你需要帮助， [本指南](https://github.com/trailofbits/algo/blob/master/docs/client-android.md) 将带你完成每一部分。

#### 在 Windows 上设置 VPN

这个过程在 Windows 上相当复杂，但仍然是可行的。

1.  前往“配置”文件夹，然后将 PEM、P12 和 PS1 文件复制到您的 Windows 机器上。
2.  双击 PEM 文件，将其导入受信任的根证书存储。
3.  打开 Powershell 应用程序，然后导航到您刚才在步骤 1 中复制的文件所在的文件夹。
4.  键入，`Set-ExecutionPolicy Unrestricted -Scope CurrentUser`并按回车键。
5.  键入 Powershell 脚本的名称，然后按 Enter 键。这将类似于`windows_$usernameyoumadeup.ps1`。遵循屏幕上的指示。
6.  最后，当输入完成后，输入`Set-ExecutionPolicy Restricted -Scope CurrentUser`并按回车键。

您的 VPN 现在应该已经设置好了。

一旦你设置好一切， [按照我们的指南](https://lifehacker.com/how-to-see-if-your-vpn-is-leaking-your-ip-address-and-1685180082) 进行测试，以确保你的 VPN 工作正常。