# 如何使用 CloudReady 将旧笔记本电脑变成 Chromebook

> 原文：<https://lifehacker.com/turn-your-old-laptop-into-a-chromebook-with-cloudready-1740556796>

如果你已经有一段时间没有使用 Chromebook 了，那么它们已经走过了的漫长道路。但是你不需要为了运行 Chrome 操作系统而花钱买一台新的笔记本电脑。你可以将它安装在几乎任何装有 CloudReady 应用程序的笔记本电脑上。

Watch

谷歌版本的 Chrome OS 不供用户安装，但其开源基础 Chrome OS——以及来自开发商 [Neverware](http://www.neverware.com/) 的 [CloudReady](http://www.neverware.com/free) ，使其安装在你的笔记本电脑上变得非常简单。不需要摆弄驱动程序或寻找兼容的硬件-只需点击安装。

### **首先:一些免责声明**

CloudReady 将带你完成 Chromium OS 的安装过程，并在幕后处理大部分技术问题。这使得它像安装任何其他操作系统一样容易。但是，您仍然应该记住一些免责声明:

*   这并不适用于所有 T2 的电脑。虽然 CloudReady 应该可以在 2007 年以来生产的大多数 Windows 和 Mac 笔记本电脑和台式机上运行，但不可能保证它可以在所有设备上运行。你可以在这里 查看已测试硬件的列表，以及 [基本系统要求。Chromium OS 通常被设计为在轻型硬件上运行，因此即使你有一台规格单调的旧机器，这也可能为旧硬件注入新的活力。](https://docs.google.com/document/d/1yPxKAmNFaJwk0kwikF5iROFMOxiinmkW_9KeI1u5jVo/pub)
*   这将清除你的系统。目前，没有办法让 CloudReady 的 Chromium 操作系统与另一个操作系统双启动，比如 Windows。请确保您将此安装在可以完全擦除的设备上。不要在你的主机上安装这个。在继续之前，请务必备份您想要保留的任何数据。
*   这不是完美的 Chrome 操作系统。虽然 Chromium 操作系统在 T2 与 Chrome 操作系统基本相同，但还是有一些关键的区别。最重要的是，你不会得到定期、自动更新或任何官方支持。它也没有内置 Flash，但 CloudReady 会在你第一次启动时告诉你如何手动安装。

只要你能处理好这些，你应该是好的。至少，这应该让你对自己能否在运行 Chrome 操作系统的电脑上生活和工作有一个大致的了解。

### **你需要什么**

一旦你找到了一台你愿意尝试的笔记本电脑，你需要收集一些东西。这是你需要的:

*   一个 8GB 或者 16GB 的 u 盘:对，就那两个。根据 CloudReady 的说法，任何大于或小于这个值的大小都会导致问题。该公司没有确切说明*为什么*任何其他尺寸都可能导致问题，但如果你打算使用其他东西，那么风险自担。
*   云准备好了。bin 文件:在开始之前，您(很明显)需要下载 CloudReady。你可以在这里找到的免费应用。点击屏幕顶部的“下载 CloudReady”并将其保存到您的电脑中。
*   **Chromebook 恢复实用程序:**该工具允许您使用 CloudReady 软件创建 USB 安装盘。你可以在这里 [找到](https://chrome.google.com/webstore/detail/chromebook-recovery-utili/jndclpdbaamdhonoechobihbbiimdgai?hl=en) 并安装在任何电脑上。

理想情况下，你应该将 CloudReady 软件和 Chromebook 恢复实用程序下载到第二台电脑上，这样在安装出错时你就有所准备了。然而，从技术上讲，你可以把所有东西直接下载到你想安装 Chromium OS 的电脑上，并在你到达安装步骤时覆盖它。在这个过程中，你只会失去你的操作系统。

### **如何安装 CloudReady**

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-XUlDYxDKgfw&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-XUlDYxDKgfw&start=0) 

一旦你拥有了你需要的一切，并且下载了所有必要的软件，你就可以开始了。首先，您需要创建一个 CloudReady USB 安装盘。这是一个非破坏性的过程，所以你可以在任何可以运行 Chrome 的电脑上这样做。不过，它会清除你的 u 盘，所以要确保 u 盘里没有你需要的东西。

要创建 USB 安装盘，请遵循以下步骤:

1.  启动 Chromebook 恢复实用程序。
2.  打开后，点按应用程序右上角的设置齿轮图标。
3.  选择“使用本地图像”
4.  选择云就绪。你从 Neverware 下载的 bin 文件。
5.  将 u 盘插入电脑。
6.  在 Chrome 恢复实用程序屏幕的左侧选择您的 u 盘。
7.  单击“继续”和“立即创建”来创建您的 USB 安装盘。

一旦这个过程完成，你就有了一个 u 盘，你可以用它在任意多的设备上安装 Chromium OS。您可以用它来启动 CloudReady 安装程序，但也可以在安装之前用它来试用 Chromium OS。如果您只想看一眼，而不想抹掉整个电脑，请按照以下步骤操作:

1.  确保在计算机的 BIOS 中启用了 USB 引导。如果您不确定，请咨询您的硬件制造商。你也可以 [点击](http://lifehacker.com/how-to-boot-from-a-usb-drive-or-cd-on-any-computer-5991848) 查看我们的 USB 引导指南。
2.  插入 CloudReady 安装 u 盘。
3.  如果出现启动菜单，请选择连接到电脑的 u 盘。有些电脑可能要求您按下特殊的启动键，如 F12。

在这一点上，如果你愿意，你可以尝试 Chromium 操作系统。如果您决定要安装，可以从同一个界面进行安装。记住，**安装 CloudReady 会擦除你的电脑**。请不要开始此过程的这一部分，除非您已经备份了计算机上的所有内容，并且您确定不再需要当前状态的计算机。

要安装 CloudReady，请按照以下步骤操作:

1.  点击 CloudReady live 界面右下角的时钟。
2.  在出现的菜单中，点击“安装 CloudReady”。
3.  出现的窗口将询问您是否确定要安装。这将清除你的硬盘。如果你确定，点击“擦除硬盘&安装 CloudReady”
4.  CloudReady 将最后一次问你是否**超级确定**。说真的伙计们。除非你准备好清除硬盘上的数据，否则不要这样做。如果是，点击“清除&安装”
5.  等待安装过程完成。

安装过程完成后，您可以像设置普通 Chromebook 一样设置您的设备。由于这是 Chromium OS 的 CloudReady 版本，您可能会得到一些提示，指导您如何手动安装 Adobe Flash 之类的东西，但除此之外，您应该只剩下一台标准的 Chromium OS 计算机。现在你的 Chromebook 已经准备好了，一定要看看你能用它做的所有很酷的事情:

*   [如何在任何桌面操作系统上运行 Chrome 内部的 Android 应用](http://lifehacker.com/how-to-run-android-apps-inside-chrome-on-any-desktop-op-1637564101)
*   [用你的安卓手机自动解锁你的 chrome book](http://lifehacker.com/automatically-unlock-your-chromebook-with-your-android-1685218009)
*   [在 Chromebook 应用启动器](http://lifehacker.com/perform-calculations-converstions-right-the-chromebook-1679966929) 中执行计算、转换
*   [“系统”告诉你关于你的 Chromebook](http://lifehacker.com/system-tells-you-everything-you-need-to-know-about-y-1590450273) 你需要知道的一切

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=1637564101,1728228132,1714671981&title=Get Even More Out of Your Chromebook)