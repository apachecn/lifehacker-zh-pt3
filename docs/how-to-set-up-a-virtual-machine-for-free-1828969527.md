# 如何免费设置虚拟机

> 原文:[https://life hacker . com/how-to-setup-a-virtual-machine-for-free-1828969527](https://lifehacker.com/how-to-set-up-a-virtual-machine-for-free-1828969527)

运行虚拟机有很多原因。第一个，也是最令人信服的，是你想玩:也许你想尝试一些其他的操作系统(*咳咳 Linux 咳咳*)，但是你不想安装另一个硬盘，分割你现有的硬盘，或者以不同的方式设置你的系统。

Watch

虚拟机非常棒，因为它们允许您在现有的操作系统中安装操作系统。你在这个新操作系统中所做的一切——cue*Inception*soundtrack——都来自你的主操作系统。你安装的任何东西，或者搞砸的任何东西，只要点几下鼠标就能删除。(如果你聪明的话，你会在安装后立即保存一个二级操作系统的版本，这样你就可以很快回到一个干净、全新的 Linux、Windows 或其他版本。)

更好的是，你可以免费在你的系统上设置一个虚拟机。以下是开始的方法:

### 您需要的应用程序

你可以付费购买一个虚拟机应用程序，如[VMWare Workstation Pro](https://www.vmware.com/products/workstation-pro.html)、 [VMWare Fusion](https://www.vmware.com/products/fusion.html) 或[Parallels Desktop](https://www.parallels.com/products/desktop/)，但如果你是虚拟机世界的新手，我建议你使用免费的 [VirtualBox](https://www.virtualbox.org/) 应用程序。(如果你使用的是 Windows 10 Pro，你还会得到一个免费的、 [内置虚拟化工具](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/create-virtual-machine) 。)

为了简单起见，本文中我所有的例子都来自于 Windows 版本的 VirtualBox，但是这个应用是跨平台的。(例如，对于 Mac 用户来说，如果你不想将引导至 Windows，VirtualBox 是一个很好的选择。)

如果没有安装操作系统，虚拟机就没有多大用处。为此，你可能要有点创意。对于 Windows，你可以抓取 [Windows media 安装工具](https://www.microsoft.com/en-us/software-download/windows10) ，用它下载一个镜像(。ISO ),然后将它加载到 VirtualBox 中。

你也可以下载微软提供的 的 [个免费虚拟机镜像，90 天后到期。](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)

如果你想在 macOS 上运行虚拟版本的 macOS *，你需要 [通过](https://blog.caffeinesecurity.com/creating-a-macos-high-sierra-vm-for-virtualbox-mac-host-bb67eada27af) 几道关卡。这一过程不像运行任何其他操作系统的虚拟版本那样简单，但这是可能的。如果你想在 Windows 上运行 macOS 尤其是如果你使用的是 VirtualBox——你会陷入一个痛苦的世界。它很复杂，配置起来很麻烦，而且我发现在我升级后的系统上运行起来非常慢。*

如果你走这条路，你可能会想尝试免费的 [VMWare 播放器](https://www.vmware.com/products/workstation-player.html) ，并在 [/r/hackintosh](https://www.reddit.com/r/hackintosh) 或有用的 YouTube 教程( [就像这个](https://youtu.be/szHn5GunojU) )上咨询指南，让 macOS 在你的 Windows 系统上工作。创建一个 Hackintosh 本身就是一个指南，如果我能让它变得不那么糟糕的话，我肯定会在以后的文章中再次讨论它。

### 设置 VirtualBox

要开始使用你的虚拟机——无论是 Windows、Linux 还是 macOS(如果你真的想要的话)——加载 VirtualBox 并点击角落里的大“新建”按钮。你不会错过的。

(如果你下载的是微软的免费虚拟机镜像，而不是 Windows。ISO 文件，您将改为点击文件>导入设备并找到。你解压的 OVA 文件。导入它，您将能够立即启动它——不需要其他配置，尽管您可能想要调整一些设置，正如我们稍后讨论的那样，以获得最佳性能。)

给你的新操作系统起个名字，选择它是什么——Windows、Linux、macOS 等等——然后选择你要安装的任何东西的正确版本。如果你只看到 32 位选项，你可能需要做一点故障排除 [来解锁 64 位版本](http://www.fixedbyvonnie.com/2014/11/virtualbox-showing-32-bit-guest-versions-64-bit-host-os/) 。然而，这可能是值得研究的，因为 64 位版本的虚拟化操作系统可以使用 4GB 以上的内存(如果您计划将这么多内存用于 OS-in-an-OS)。如果你使用的是 32 位处理器，因为你的电脑是老式的，那么你应该坚持使用 32 位版本的虚拟操作系统。

当 VirtualBox 问你你想把多少系统内存分配给你的虚拟操作系统时，我会坚持它的建议——特别是，留在“绿色区域”为了让 Windows 流畅运行，您可能至少需要 2–4GB 的内存。如果能上 8GB，那就更好了。(是的，在 VirtualBox 中，一切都是以 MB 为单位的，所以 2GB 等于 2048MB，4GB 等于 4096MB，等等。)

事后，您可以随时调整分配给虚拟机的内存量。如果您对最初的选择不满意，可以调整一下，看看这会如何影响虚拟机的性能。

接下来，VirtualBox 会要求你设置一个“硬盘”——实际上是一个用作硬盘驱动器的文件——供你的虚拟机使用。点击“创建”后，您将看到三种不同的硬盘文件类型供您选择:

您应该可以坚持使用默认选项:VirtualBox 磁盘映像，或 VDI。然而，在下一个屏幕上，你需要考虑你的选择。您可以选择创建一个动态分配的磁盘，该磁盘仅在您使用实际硬盘驱动器时占用空间(但在您删除虚拟操作系统上的文件时不会缩小)，或者您可以为虚拟操作系统将使用的硬盘驱动器设置一个固定的大小。

固定磁盘比动态分配的磁盘快，但是你必须预先分配所有的空间，而不是让你的虚拟操作系统随着你的填充而使用越来越多的空间。我自己会选择固定磁盘，因为它简化了一切，并为您提供最佳性能，但如果您空间紧张，您可能只能坚持使用动态分配的磁盘。

您将在下一个屏幕上设置磁盘的大小:

一旦 VirtualBox 创建了您的磁盘，您将看到全新的虚拟机，一切就绪！但也不尽然。您还需要查看一些设置，因此选择您的虚拟机并单击大的设置齿轮图标。

有很多方法可以让你的虚拟机发挥出最大的性能，包括调整它获得的内存量，多少处理器用于虚拟操作系统，以及它应该有多少显存。您现在可以通过系统和显示菜单调整这些设置。完成后，您将需要访问存储菜单，以便实际安装操作系统。

在存储器中，您会看到一个 CD(或 DVD)的小图标，旁边有“空”字。选择它，然后点按“光盘驱动器”右侧最右侧“属性”部分中的 CD(或 DVD)图像选择“选择虚拟光盘文件”选项，找到您要安装的操作系统的映像，然后选择它。

如果您已经完成了对虚拟机设置的编辑，并且您确实应该检查 USB，以确保您的主机系统连接的设备也可以由您的虚拟机使用，以及通用>高级，以在您的主机和虚拟操作系统之间共享剪贴板和拖放功能，请单击确定。然后点击绿色的“开始”箭头，启动你的虚拟操作系统。如果幸运的话，它将启动到它的设置过程中，您将准备好安装它，就像您正在设置一个全新的台式机或笔记本电脑。

一旦你启动并运行了你的虚拟机，你会想要充分利用 VirtualBox 的快照功能(在它的“机器”菜单下)。快照允许您随时保存和恢复虚拟机的状态。所以，一旦你安装了新版本的操作系统，拍一张快照。如果你搞乱了你的虚拟机，或者想把它恢复到原始的状态(不需要重新安装操作系统)，你可以恢复你的快照。或者，如果您打算做一些可能会因为任何原因搞乱您的虚拟机的事情，请先拍一张快照——同样的原则。