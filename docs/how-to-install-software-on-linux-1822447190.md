# 如何在 Linux 上安装软件

> 原文：<https://lifehacker.com/how-to-install-software-on-linux-1822447190>

所以你已经切换到 Linux 了。或者你在考虑掉包。但是你的问题可能会阻止你完全投入进去。大多数新用户最关心的一个问题是，“有什么软件可用，我如何安装它？”



这是个合理的问题。为什么？在很长一段时间里，Linux 饱受应用程序稀缺的耻辱，可用的选项很少，安装起来很困难。我记得，在早期，不得不从源码包编译软件——这将导致一个看似无止境的缺失依赖循环。这令人沮丧，但可行。然而，这种挫败感让很多人远离了 Linux。

幸运的是，那些日子已经过去很久了，在 Linux 上安装任何可用的软件(有很多)不再是一件令人头痛的事情。

在我们开始在 Linux 上实际安装软件之前，有一个非常重要的概念需要理解:

### **包管理器**

这是一个让大多数新 Linux 用户感到困惑的话题。软件包管理器是 Linux 上的一个子系统，如标题所示，它管理您计算机上的软件包(软件)。它是 Linux 的一个重要组成部分，因为它跟踪安装的所有东西；下载软件包；确保所有软件包都安装在一个公共位置；帮助升级软件包；解析依赖关系；并使用户不必从源代码安装。

最大的困惑是有许多可用的包管理器，但是一个发行版上只能使用一个。事实上，发行版的区别主要在于它们选择了哪个包管理器。比如:[Debian](http://www.debian.org)[Ubuntu](http://www.ubuntu.com)(及其衍生)使用 apt [红帽企业版 Linux](https://www.redhat.com) 、 [CentOS](https://www.centos.org/) 、 [Fedora](https://getfedora.org/) 用百胜； [SUSE](http://www.suse.com) 和 [openSUSE](https://www.opensuse.org/) 使用 zypper 而 [Arch Linux](https://www.archlinux.org/) 用的是 pacman。现在有更多的包管理器，但是这是一个很好的起点。

每个包管理器使用不同的文件类型。例如，apt 与。deb 文件和 yum 和 zypper 一起工作。rpm 文件。apt 包管理器无法安装。rpm 文件，yum 或 zypper 都无法安装。黛比档案。让事情更加混乱的是，Ubuntu(及其衍生工具)使用 *dpkg* 命令来安装 local。deb 文件，而 Red Hat(及其衍生产品)使用 *rpm* 命令来安装本地。rpm 文件。

困惑了吗？别担心，实际上比这简单多了。

大多数包管理器都有 GUI 前端。这些前端类似于苹果应用商店。有许多这样的 GUI 前端可用是不足为奇的。这里的好消息是大部分都是类似的标题(比如 GNOME 软件，Ubuntu 软件，Elementary AppCenter)。这些应用程序商店允许你轻松地搜索一个软件名称，然后点击一个按钮就可以安装它(稍后会有更多相关内容)。

包管理器还有一个问题:存储库。存储库是包管理器的一个关键方面，但是对于新用户来说，这个概念可能会增加我们不希望的另一个层次的混乱。然而，为了快速概述，请考虑这一点:开箱即用，您只有特定的软件标题可供选择。该选择由配置的存储库决定。有许多第三方存储库可以添加到系统中。添加后，您可以安装与这些第三方存储库相关联的任何软件标题。可以从 GUI 工具或命令行添加软件存储库。

在任何情况下，存储库都是另外一个问题，对于本文中讨论的软件下载类型来说没有必要理解。

### **安装下载的文件**

我知道，我知道……我说过现代 Linux 操作系统的一个好处是，你不需要*从下载的文件安装。也就是说，我想从这里开始。为什么？有时，您可能会发现某个软件在发行版的“应用商店”中不可用出现这种情况时，您需要知道如何手动安装该应用程序。我要说的是，在日常生活中，一般情况下，你很少需要这样做。即使您从未使用这种方法安装，至少您会对它的工作原理有一个非常基本的了解。*

在这里，我们将使用最新发布的 [Ubuntu Linux](https://www.ubuntu.com/) (在撰写本文时，17.10)进行演示。大多数软件包管理器以相似的方式安装(使用的命令略有不同)。假设你想在 Ubuntu 上安装谷歌 Chrome 浏览器。你不会在 Ubuntu 软件工具中找到这个特定的浏览器。要从命令行安装它，您必须下载正确的文件。如前所述，Ubuntu 的正确文件应该是. deb 文件。所以把你的浏览器指向 [Chrome 下载页面](https://www.google.com/chrome/) ，点击下载 Chrome 按钮。这里的好消息是，你的浏览器将被检测到，Chrome 下载页面将知道你需要哪个文件。点击 ACCEPT AND INSTALL 按钮，一个新窗口将会出现，给你两个选项(**见下面的**)。

您可以将文件保存到硬盘上(然后通过命令行安装)，或者使用软件安装程序打开文件。重要的是要明白，不是每个发行版都包括后者。如果你没有得到打开选项，那么你必须从命令行安装。

让我们首先使用 Open with 选项。确保选择了软件安装(默认),然后单击确定。文件将会下载，然后 Ubuntu 软件将会打开，让您选择安装(**见下面的**)。

单击安装，系统会提示您输入用户密码。安装将完成，Chrome 可以使用了。你可以关闭 Ubuntu 软件工具，从 Dash 打开 Chrome。

但是，如果您没有选择使用 GUI 工具安装，该怎么办呢？然后，您必须选择保存文件，并从命令行运行安装。别担心，没那么难。以下是在 Ubuntu Linux 上从命令行安装最新版 Chrome 的步骤:

1.  点击桌面底部的正方形圆点
2.  当仪表板打开时，键入*终端*
3.  使用命令 *cd ~/Downloads* 进入下载目录
4.  用命令 *sudo dpkg -i google-chrome*安装 Chrome。债务*
5.  当出现提示时(**见下面的**)，键入您的用户密码并按键盘上的 Enter 键
6.  允许安装完成

### **从 GUI 安装**

这是事情变得非常容易的地方。要从您的发行版的 GUI 安装，您只需要打开工具，搜索您想要的软件，然后单击 install。比方说，你想安装 GIMP 图像编辑器。为此，打开 Ubuntu 软件，在搜索栏中输入 gimp。当结果出现时，点击 GIMP 条目，点击安装按钮(**见下面的**)，并(当提示时)输入你的用户密码。等待安装完成，您的新软件就可以打开使用了。

### **底线:这比看起来容易多了**

在 Linux 上安装软件远没有你想象的那么难。是的，当你需要从命令行安装某些东西时，可能会有*或*的罕见情况，但即使这样也不是什么大挑战。此外，很有可能你永远也不需要在 GUI 前端之外安装软件。

请记住，如果你使用 Ubuntu 以外的发行版(或者它的衍生版本)，你需要快速地搜索一下，以确保你理解 apt 软件包管理器和你桌面上使用的软件包管理器之间的区别。