# 在 Mac 上运行 Windows:VirtualBox vs VMware Fusion vs Parallels

> 原文：<https://lifehacker.com/run-windows-on-your-mac-virtualbox-vs-vmware-fusion-vs-1750474360>

如果你需要在 OS X 内部运行 Windows，你有三个选择:VirtualBox、VMware 和 Parallels。每一种都有自己的优点和缺点，以及一种比另一种更好的不同用例。让我们来分解一下每一个什么时候是最好的，为了什么。



### 竞争者

虚拟机可以让你在 OS X 运行像 Windows 这样的操作系统，同时运行普通的 Mac 设置。一旦你设置了一个虚拟机，你就可以安装你想要的操作系统，你可以直接从你的 Mac 桌面上使用它，不需要重启。为此，有三种流行的选择:

*   [**VirtualBox**](https://www.virtualbox.org/wiki/Downloads)(免费):VirtualBox 轻松成为 [我们在这里比较的三个选项中最乏味的](https://lifehacker.com/the-beginners-guide-to-creating-virtual-machines-with-v-5204434) 。它为您的虚拟机提供了各种定制选项，但没有任何像 Parallels 和 VMware 那样的花哨集成功能。本质上，VirtualBox 允许你创建一个运行 Windows 的虚拟机，仅此而已。
*   [](http://www.vmware.com/products/fusion/)
*   **[**Parallels**](http://www.parallels.com/products/desktop/)**(一台 Mac 79.99 美元):VMware Fusion 和 Parallels 非常相似，但 Parallels 更紧密地指导您完成安装过程。它还专注于家庭用户，他们只需要一种简单的方式在 Mac 上使用 Windows，而无需重启或购买另一台电脑。****

****在这里，我们不能不提到 Boot Camp ，它在你硬盘的一个独立分区上运行 Windows。与虚拟机不同，Boot Camp 需要重启电脑，你不能同时使用两个操作系统。这有点不太方便，但这意味着您的 Windows 安装可以充分利用 Mac 的硬件，为您提供更好的性能。我们不会将它包括在今天的摊牌中，这是专门关于不同的虚拟化选项，但作为在 Mac 上运行 Windows 的一个选项，它值得一提。****

****现在，让我们深入了解一下每种方法的一些细节。****

### ****易于设置****

****虚拟机不像其他应用程序。安装不仅仅是安装应用程序，因此过程的简单性非常重要。****

****让我们从 VirtualBox 开始，因为它是最实用的。首先创建一个虚拟机，并选择计划运行的操作系统(Windows、Linux 等)。然后，您需要调整一系列系统设置，包括虚拟机获得多少处理器内核，它从系统中安装的总内存中获得多少内存和视频内存。谢天谢地，我们有一个 [向导来帮你完成](http://lifehacker.com/the-power-users-guide-to-better-virtual-machines-in-vir-1569943402) 的整个过程。一旦您完成了所有的配置，您就可以像在任何计算机上一样安装操作系统了。这意味着您需要安装光盘、USB 驱动器或 ISO 文件来进行安装。****

****VMware 和 Parallels 都有设置向导， [会引导您完成整个过程。](https://lifehacker.com/how-do-i-install-windows-8-in-a-virtual-machine-5841065) 除了简单地安装一个虚拟机，两者都允许你导入你的 Boot Camp 分区(如果你有的话)，或者将一台旧的 Windows PC 迁移到你的 Mac 上。Parallels(如上图)会引导您完成更多安装过程，您可以选择自动优化 Parallels 以提高工作效率或玩游戏。当然，如果你愿意，你也可以跳过这个屏幕，从头开始安装 Windows。****

****它们都很简单，尽管 Parallels 对新用户来说有一点优势，因为它在整个过程中都握着你的手。就用户友好性而言，Parallels 一直是我们测试的三款产品中最强的。这使得它成为对设置不感兴趣的人的一个很好的解决方案。****



### ****与众不同的附加功能****

****虽然这三个程序做的基本上是相同的事情，但是一些小的特性使它们彼此不同。****

****这三款应用都支持某种窗口模式(见上图)。这允许你在你的 Mac 桌面上运行一个单独的 Windows 应用程序，所以感觉更像一个本地的 Mac 应用程序。VMware 称此为 [Unity](https://blogs.vmware.com/teamfusion/2011/11/viewing-your-windows-programs-without-seeing-windows.html) ，Parallels 称此为 [Coherence](http://kb.parallels.com/en/4670) ，VirtualBox 称之为 [无缝模式](http://lifehacker.com/how-to-seamlessly-run-that-one-windows-app-you-need-on-5521308) 。当应用程序处于窗口模式时，您可以在 Windows 和 Mac 应用程序之间拷贝和粘贴信息，移动和调整它们的大小，以及在不关闭 Windows 的情况下关闭应用程序。****

****Parallels 和 VMware 都允许您直接从 Dock 打开单个 Windows 程序，这使得整个过程非常简单。VirtualBox 不支持这一功能，而是要求你打开整个虚拟机来选择你的应用程序。****

****相似之处不止于此。如果你运行的是 Windows 10，Parallels 和 VMware 都会给你 [访问 Cortana 的权限来发出语音命令](https://lifehacker.com/everything-you-can-ask-cortana-to-do-in-windows-10-1721725525) ，即使 Windows 不在焦点上。它们都支持 DirectX 10，这意味着它们可以运行大多数游戏，尽管不能保证良好的性能(下一节将详细介绍)。VirtualBox 不支持任何像这样很酷的小技巧。相反，它只是执行作为一个整体运行 Windows 的简单任务。****

****Parallels 和 VMware 之间的功能差异非常微妙。例如，Parallels 支持 OS X 在 Windows 中的快速查看功能，而 VMware 不支持。相反，如果你碰巧有一台漂亮的新 iMac，VMware 原生支持 5K 显示器。大部分的东西都很小，但是，老实说，如果你剥去标志，我很难说出两者之间的区别。****

****如果你想对 VMware Fusion 和 Parallels 中的*一切*进行全面比较， [维基百科有一个方便的图表](https://en.wikipedia.org/wiki/Comparison_of_VMware_Fusion_and_Parallels_Desktop) 值得一看，尽管它不是完全最新的。****

### ****性能和基准****

****由于虚拟机必须与主机操作系统共享资源，因此性能非常重要。谢天谢地， [TekRevue 已经为各种任务对所有三个程序](http://www.tekrevue.com/2015-vm-benchmarks-parallels-11-vs-fusion-8/) 进行了基准测试。当前版本的 VMware 几乎在每个领域都优于其他产品，而 VirtualBox 则远远落后于其竞争对手。当然，不仅仅如此。****

****在 18 项不同的测试中，VMware 在 11 项测试中获得了最高荣誉，尤其是在图形性能指标评测中。性能差距通常非常接近，总体而言，Parallels 在 CPU 相关测试中表现最好，而 VMware 在图形相关测试中表现最好。****

****CPU 对显卡的总体趋势贯穿了他们的测试。Parallels 往往比 VMware 启动更快，传输文件更快，电池寿命比 VMware 更长。反过来，VMware 对 3D 图形和游戏的基准测试要高得多，尤其是 OpenGL。VirtualBox 在 CPU 和 3D 性能方面一直落后。****

### ****结论是:VirtualBox 提供了一个免费的、基本的体验。VMware 或 Parallels 提供易于使用、集成程度更高的解决方案****

****如果你只需要 Windows 来运行一个不需要大量 3D 渲染或其他复杂处理的旧应用程序，VirtualBox 就是你想要的。除此之外，就功能而言，这两种付费选项非常相似，区别主要是价格和需要安装多少台 MAC。如果你打算在 3D 中运行任何东西，或者想在多台 Mac 上安装 Windows，那么就选择 VMware。如果您对生产力软件和电池寿命更感兴趣，并且不介意一台 Mac 的限制，那么 Parallels 是您的最佳选择。****

****所有这些也每年都在变化。Parallels 和 VMware 都要求您每年购买一份年度许可证，以获得包含性能提升和功能改进的更新。这些年度更新在理论上很棒，但它们并不便宜，而且每年都会更新。这有点烦人，尤其是 [当他们把那些付费升级](http://arstechnica.com/information-technology/2015/08/year-old-parallels-and-vmware-software-wont-be-updated-for-windows-10/) 后面的 Windows 新版本锁在外面的时候。如果你不需要走在最前沿，它们通常是相当渐进的，但是，你可以跳过一两个——只要没有新版本的 Windows 出来。****

****不管怎样，好消息是，虽然 VirtualBox 是免费的，但即使是 VMware Fusion 和 Parallels 也有试用期，因此您可以全部试用。我们绝对建议你在丢钱之前这么做。您不必尝试所有三个选项，但是如果您的需求非常有限，请先从 VirtualBox 开始，然后再考虑 VMware 或 Parallels。****