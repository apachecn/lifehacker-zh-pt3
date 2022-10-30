# 构建 Hackintosh 的最新指南(macOS Sierra)

> 原文:[https://life hacker . com/the-always-update-guide-to-building-a-hackintosh-o-5841604](https://lifehacker.com/the-always-up-to-date-guide-to-building-a-hackintosh-o-5841604)

构建一台 hackintosh——即在非苹果硬件上安装 macOS 过去需要极其有限的硬件选择和相当多的专业知识。现在您的选择范围很广，安装过程也相当简单。考虑到这一点，这里是我们构建 hackintosh 的最新指南，它将引导您购买兼容的部件，构建您的机器，并自行安装 macOS。

Watch

**目前最新版本:macOS 10.12 (UniBeast 方法)**

本指南是关于在你的 hackintosh 上安装 macOS Sierra 的。如果你正在寻找安装一个旧版本，检查我们的存档 [OS X 10.7 狮子](http://lifehacker.com/how-to-install-os-x-10-7-4-on-your-hackintosh-30779545) ， [OS X 10.8 山狮](http://lifehacker.com/how-to-install-os-x-10-8-5-on-your-hackintosh-1454156452) ， [OS X 10.9 小牛](http://lifehacker.com/how-to-install-os-x-10-9-5-on-your-hackintosh-1648600653#_ga=1.160109373.1055861349.1441835238) ，和 [OS X 10.10 约塞米蒂](http://lifehacker.com/how-to-install-os-x-10-10-yosemite-on-your-hackintosh-1743070950) 指南。

### 首先:到底什么是 Hackintosh？

一台 hackintosh 简单来说就是任何非苹果的硬件，被制造出来或者被“黑”出来运行 macOS。这适用于任何硬件，无论是制造商制造的还是个人制造的电脑。出于本指南的目的，我们只讨论一个可靠的方法来构建你*构建的黑客工具。*

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled The Always Up-to-Date Guide to Building a Hackintosh (macOS Sierra)](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/can-i-hackintosh-my-laptop-5869731) [###### 我能黑进我的笔记本电脑吗？](https://lifehacker.com/can-i-hackintosh-my-laptop-5869731) 

亲爱的生活黑客，我有一个 Sorny Inspiron book mate 2564300 ip00。我能做 Hackintosh 吗？但是说真的，

[Read more](https://lifehacker.com/can-i-hackintosh-my-laptop-5869731)</aside>

这意味着你需要习惯于 [建造自己的机器](http://lifehacker.com/how-to-build-a-computer-lesson-3-building-the-compute-5827491) 并在遇到问题时提供自己的技术支持。如果您是构建 hackintosh 的新手，这种前景可能有点可怕，但它也将为您节省大量资金，同时仍然为您提供一台功能强大、完全可定制的机器。我们还会为您提供一些资源，帮助您了解构建计算机所需的一切知识，让您在第一次完成整个计算机构建过程时充满信心。这不是一个初学者的项目，但它是任何人都可以学会做的事情。

### 本指南是如何工作的？

拥有一个总是最新的构建 hackintosh 的指南似乎很奇怪，因为这个过程会根据您所做的硬件选择而变化。虽然这是真的，但并没有改变那么多。我们将在广泛的层面上讨论构建 hackintosh 的过程，因为它适用于大多数硬件。因此，这份指南并不总是能告诉你确切的选项和选择，但是它会教你如何自己去发现。在整个过程中，我们会尽可能地紧紧握住你的手，但有些决定你必须自己做出。有时候会有点吓人，但这也是乐趣的一部分。

总之，这本总是最新的指南将解释如何为优秀的 hackintosh 选择正确的硬件，并引导您完成标准的安装过程，但它也要求您勤奋并了解您的特定构建中的变量。

### 如何选择最适合您需求的硬件

挑选硬件和组装电脑通常是这个过程中最令人望而生畏的部分。谢天谢地，我们在这里为你做了很多工作！虽然您当然可以 [自己研究](https://lifehacker.com/how-do-i-choose-the-right-hardware-when-building-a-hack-5837615) 并挑选兼容的部件，但我们已经创建了一个 [大型预配置系统选择](http://www.customac.com/) 以及一个兼容部件列表，供您构建自己的系统。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled The Always Up-to-Date Guide to Building a Hackintosh (macOS Sierra)](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-do-i-choose-the-right-hardware-when-building-a-hack-5837615) [###### 构建 Hackintosh 时，我如何选择合适的硬件？](https://lifehacker.com/how-do-i-choose-the-right-hardware-when-building-a-hack-5837615) 

亲爱的 Lifehacker，我已经阅读了你关于如何构建一个普通黑客电脑和一个迷你黑客电脑的指南，但是

[Read more](https://lifehacker.com/how-do-i-choose-the-right-hardware-when-building-a-hack-5837615)</aside>

我们的 [构建列表](http://www.customac.com/) 包括以下类型的机器:

*   CustoMac Mini:一个装在鞋盒大小的盒子里的苹果迷你克隆体。
*   CustoMac Mini Deluxe :一台更大但仍低于平均尺寸的计算机，拥有强大的动力。
*   **CustoMac mATX** :一款中等大小的产品，配有四核 CPU、最大容量的 RAM 和大量的可扩展性。
*   CustoMac Budget ATX :一款功能强大的台式机，采用经济型部件，没有显卡。
*   **CustoMac Pro** :全尺寸构建，配有四核 CPU、最大 RAM 和大量可扩展性。

或者，您可以查看我们的单个组件列表，并构建您自己的定制系统。我们数据库中列出的组件并不是唯一可用的组件，但根据我们的研究，它们是最简单、最受支持的选项。使用我们的买家指南作为购物清单或进一步定制的起点。

一旦你有了硬件，你就需要把它组装成一台可以工作的计算机。我们有一个关于计算机构建 的 [整个夜校课程，但是](https://lifehacker.com/how-to-build-a-computer-the-complete-guide-5828747) [这个特定的课程将带你经历如何构建你的第一台计算机](http://lifehacker.com/how-to-build-a-computer-lesson-3-building-the-compute-5827491?tag=nightschool) 。努力遵循它，*仔细阅读您的主板和机箱手册*，您应该很快就会拥有一台功能正常的机器。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled The Always Up-to-Date Guide to Building a Hackintosh (macOS Sierra)](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-to-build-a-computer-the-complete-guide-5828747) [###### 如何建造一台计算机:完全指南](https://lifehacker.com/how-to-build-a-computer-the-complete-guide-5828747) 

从零开始构建一台计算机会为您提供满足您需求的完美机器，但它可能…

[Read more](https://lifehacker.com/how-to-build-a-computer-the-complete-guide-5828747)</aside>

### 如何在你的 Hackintosh 上安装 macOS

在 hackintosh 硬件上安装 macOS 不仅仅是放入一张 DVD，选择一个引导卷，然后点击一个按钮。你也必须采取这些步骤，但是要经过相当多的准备工作。让我们开始吧。

对于大多数 Mac 用户来说，完整的操作系统是免费下载的，所以你需要一台真正的 Mac 来获得它(如果你没有，就借用朋友的)。在任何运行 macOS 10.6.8 或更高版本的 Mac 或功能性电脑上，使用您的 Apple ID 从 Mac App Store 下载应用程序。

#### 第一步:配置 BIOS

开始之前，您需要调整计算机 BIOS 中的一些设置。你可以在我们的计算机构建指南 中阅读更多关于 BIOS 的内容，但这里是基本步骤。

如果您在推荐的带有 AMI UEFI BIOS 的 CustoMac 桌面上安装，选项很简单。对于其他系统，请确保将 BIOS 设置为优化默认值，并将硬盘设置为 AHCI 模式。下面是标准的 AMI UEFI BIOS 设置为 [技嘉 AMI UEFI BIOS](http://www.tonymacx86.com/bios-uefi/130920-recommended-bios-uefi-settings-beginners.html) 、 [技嘉奖 BIOS](http://tonymacx86.blogspot.com/2010/04/iboot-multibeast-install-mac-os-x-on.html) 、 [华硕 AMI UEFI BIOS](http://www.tonymacx86.com/user-builds/136796-tonymacx86s-asus-test-build-z97-i3-4340-hd4600-thunderbolt-ex-ii.html) 、 [微星 AMI UEFI BIOS](http://www.tonymacx86.com/bios-uefi/143167-msi-9-series-motherboards-os-x-setup-configuration.html) 。

1.  要访问 BIOS/UEFI 设置，请在系统启动时按住 USB 键盘上的**Delete**

2.  加载**优化默认值**

3.  如果你的 CPU 支持 **VT-d** ，禁用它

4.  如果你的系统有 **CFG 锁**，禁用它

5.  如果你的系统有**安全引导模式**，禁用它

6.  将操作系统类型设置为**其他操作系统**

7.  如果你的系统有 **IO 串口**，禁用它

8.  将 XHCI 切换设置为**启用**

9.  如果您的 6 系列或 x58 系统带有 AWARD BIOS，请禁用 **USB 3.0**

10.  保存并退出。

#### 步骤 2:安装 macOS Sierra

现在是时候真正安装 macOS 了。我们将使用 UniBeast，它是一个工具，可以为你的 hackintosh 从你下载的 macOS 版本中创建一个可引导的安装程序。

我们推荐的 bootloader 叫 Clover。三叶草是一个新的和令人兴奋的开源 EFI 引导加载程序。由 Slice 领导的 OS X 项目的一组开发人员在过去两年中开发的 Clover 旨在解决现有 macOS 安装方法和遗留引导程序中的固有问题。

请记住，在这个过程的第一步，你需要一台真正的 Mac 电脑，所以如果你没有自己的电脑，可以向朋友借一台。如果你完全没有办法借用一台工作的 Mac，你可以用实际的 DVDT3[从头开始安装雪豹。](http://tonymacx86.blogspot.com/2010/04/iboot-multibeast-install-mac-os-x-on.html)

为此，您还需要:

*   从 Mac App Store 下载一份[**Mac OS Sierra**](https://itunes.apple.com/us/app/macos-sierra/id1127487414?mt=12)。(确保你有最新版本！)
*   一个 **16GB 的拇指驱动器**(或更大)。
*   [**UniBeast**](http://www.tonymacx86.com/downloads.php?do=cat&id=3) ，可从 tonymacx86.com 的下载页面获得。
*   [](http://www.tonymacx86.com/downloads.php?do=cat&id=3)**，也可从 tonymacx86.com 的下载页面下载。**

**一旦你有了一切，你需要创建你的安装闪存驱动器。为此，请按照下列步骤操作:**

1.  **在借来的 Mac 上打开 Mac App Store，下载 macOS Sierra。请确定它出现在/Applications 中。**
2.  **插入 8GB+ USB 驱动器，打开/应用程序/实用工具/磁盘工具。**
3.  **突出显示左栏中的 USB 驱动器，并单击分区选项卡。点按“当前”并选择“1 个分区”。**
4.  **在 Clover 启动屏幕上，选择 USB 并按回车键。如果你无法找到安装程序，请查看本页 中的 [步骤 4 了解更多信息。](http://www.tonymacx86.com/445-unibeast-install-os-x-yosemite-any-supported-intel-based-pc.html)**
5.  **在“格式”下选择“Mac OS 扩展(日志式)”。**
6.  **完成后，关闭“磁盘工具”并运行 UniBeast。**
7.  **按照屏幕上的向导，在提示时选择您的 USB 驱动器，并在询问您正在安装什么版本的 macOS/OS X 时选择 Sierra。**
8.  **完成向导，创建您的 USB 驱动器。这大约需要 10-15 分钟。**
9.  **将 MultiBeast 拖到您的新闪存驱动器上，以便以后使用。**
10.  **将新的安装程序闪存驱动器插入您即将开始的 hackintosh。启动系统并按热键选择一个引导设备(通常是 F12 或 F8)。出现提示时，选择您的闪存驱动器。**
11.  **在 Clover 启动屏幕上，选择 USB 并按回车键。如果你无法找到安装程序，请查看本页 中的 [步骤 4 了解更多信息。](http://www.tonymacx86.com/445-unibeast-install-os-x-yosemite-any-supported-intel-based-pc.html)**
12.  **在欢迎屏幕上选取您的语言，然后前往“实用工具”>“磁盘工具”。**
13.  **在左栏中高亮显示您想要用于 macOS 的硬盘，点按“分区”标签，然后在下拉菜单中选取“1 分区”。**
14.  **单击选项按钮，选择“GUID 分区方法”。**
15.  **给驱动器命名，从“格式”下拉列表中选取“Mac OS 扩展(日志式)”，然后点按“应用并分区”。完成该过程后，请关闭“磁盘工具”。**
16.  **完成安装向导的其余部分以完成该过程。**

**这是安装过程的一个压缩版本，应该可以让你完成你需要的一切。要获得完整的逐步截图和额外的故障排除信息(以防您遇到问题)，请参见 [我在 tonymacx86.com](http://www.tonymacx86.com/el-capitan-desktop-guides/172672-unibeast-install-os-x-el-capitan-any-supported-intel-based-pc.html)的完整指南。**

#### **第三步:安装你的驱动程序**

**现在您已经安装了 Sierra，是时候让所有硬件正常工作了。MultiBeast 是一个一体化的安装后工具，旨在实现从硬盘启动，并安装对音频、网络和图形的支持。它还包括修复权限的系统实用程序以及驱动程序和配置文件的集合。**

**从 USB 驱动器启动 MultiBeast，并按照以下步骤操作:**

1.  **如果这是全新安装，请单击快速启动。如果您有基于 UEFI 的较新系统，请选择 UEFI 引导模式。对于使用基于 BIOS 的系统的旧台式机，建议使用传统引导模式。**
2.  **接下来，从驱动程序选项卡中选择驱动程序。这取决于你的版本，但是你可能需要音频驱动。找出主板上的芯片组，并为其选择相关的驱动程序。您可能还需要以太网驱动程序。大多数其他事情将取决于您是否选择了其他本机兼容的硬件，如您的 GPU。有些 GPU 需要特殊的驱动程序，有些则默认工作。**
3.  **如果您有英特尔集成 HD 3000 显卡或较旧的 AMD 或 NVIDIA 显卡，请单击自定义并选择相关的显卡选项。**
4.  **单击打印或保存备份您的配置。**
5.  **单击构建，然后单击安装。让多播做它自己的事。**
6.  **重新启动计算机以完成安装。**

**MultiBeast 旨在用作 UniBeast 的安装后方法，因此是一种简单的启动和运行方法。**

#### **备选 NVIDIA 显卡驱动程序**

**NVIDIA 在网上为每个 macOS 版本单独发布替代图形驱动程序。这些不同于 Apple 作为标准提供的驱动程序，应该被视为实验性的。过去，这些驱动程序已经解决了某些应用程序的 OpenCL 问题，并为某些设备提供了更好的本机 GPU 电源管理。它们还将使最新的“Maxwell”卡能够完全加速工作，包括 NVIDIA GeForce GTX 750、750 Ti、950、960、970、980、980 Ti 和 TITAN X。你可以 [阅读有关这些驱动程序的更多信息，并在这里](https://www.tonymacx86.com/threads/nvidia-releases-alternate-graphics-drivers-for-macos-sierra-10-12-0-367-15-10-05.200843/) 下载它们。**

#### **第四步:更新你的黑客工具**

**在过去的版本中，更新通常需要您重新安装在第三步中安装的任何带有 MultiBeast 的图形、网络和音频驱动程序。请继续关注[tonymacx86.com 首页](http://www.tonymacx86.com/) 的更新帖子，我们在那里概述了苹果扔给我们的每个软件更新都需要哪些变通办法(如果有的话)。(例如， [以下是你为 OS X 10.11.6](https://www.tonymacx86.com/threads/os-x-10-11-6-update.195102/) 所做的)。**

### **如何解决你的黑客问题**

**黑客攻击并不完美——任何原因都可能导致事情出错。你不太可能创建一个而不陷入，至少是一个小困境。不幸的是，许多故障排除都涉及到反复试验，你只能不断地修改，直到问题得到解决。如果你遇到一些问题，你可能会在上找到支持。**

**最后，一旦你开始工作，你应该 [克隆你的硬盘](http://www.tonymacx86.com/173-backup-solutions-your-mac-customac.html) ，这样你就有了一个可启动的拷贝，以防出错。通过这种方式，您可以恢复到该副本，或者至少比较自从它正常工作以来发生变化的内容。不管你怎么想，总有一天你会把事情搞砸。保留备份。你不会后悔的。**

**如需更多故障排除技巧，请查看 Lifehacker 的 [hackintosh 故障排除指南](https://lifehacker.com/how-to-troubleshoot-a-hackintosh-5845186) 和 tonymacx86.com 多播指南 [底部的故障排除链接。](https://www.tonymacx86.com/threads/unibeast-install-macos-sierra-on-any-supported-intel-based-pc.200564/)**

* * *

**[<small>*tonymacx86*</small>](https://twitter.com/tonymacx86)<small>*创始人是*</small>[<small>*【tonymacx86.com】*</small>](http://tonymacx86.com/)<small></small>*[<small>*CustoMac 买家指南*</small>](http://www.tonymacx86.com/section/295-customac.html) <small>*、iBoot、MultiBeast、uni*</small>***