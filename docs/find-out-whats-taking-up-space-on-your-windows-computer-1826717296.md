# 使用 Wiztree 找出占用 Windows 计算机空间的内容

> 原文：<https://lifehacker.com/find-out-whats-taking-up-space-on-your-windows-computer-1826717296>

Windows:大多数电脑爱好者都知道 [WinDirStat](https://lifehacker.com/windows-app-of-the-week-windirstat-1825098404) ，这是一个非常有用的工具，可以显示哪些文件夹和文件占用了你的硬盘空间。这是一个必须拥有的应用程序，因为你会惊讶——见鬼，*我已经*惊讶过——多少次你可能会在你的桌面上发现一些随机的、三重掩埋的文件夹，它们占用了不适当的空间。



问题？WinDirStat 需要一段时间才能发挥作用。在我的主要 500GB 固态硬盘上，目前有大约 252GB 的可用空间(只有我的 Windows 操作系统和我的应用程序)，WinDirStat 花了 42 秒完成一次分析。虽然这比你最喜欢的播客上的蓝色围裙广告时间少，但仍然不是很快。

我最近看到一些关于应用程序 [Wiztree](http://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive/) 的聊天，它基本上像 WinDirStat 一样扫描你的驱动器。我下载了它的便携式版本并把它调出来，选择了和以前完全一样的驱动器进行分析。Wiztree 只用了 1.44 秒就完成了与 WinDirStat 相同的结果，仅减少了 96.6%。

巫师树的魔法是如何运作的？正如该应用程序所描述的:

> *“扫描 NTFS 格式的硬盘时(大多数现代硬盘都使用这种格式)，WizTree 直接从磁盘读取硬盘的主文件表(MFT)。MFT 是一种特殊的隐藏文件，NTFS 文件系统使用它来跟踪硬盘上的所有文件和文件夹。以这种方式扫描文件完全绕过了操作系统(Windows ),大大提高了性能。”*

虽然这两个应用程序在细节上有所不同——它们找到了多少特定类型的确切文件，或者某个文件夹占用的确切百分比——但我会将这一点写在计算(或忽略)不同类型的文件上。两者都对我最大的文件夹和文件进行了正确的排序，这才是最重要的。你不会很在意那个有 50MB 随机内容的文件夹，但你会很在意识别出那个有几部你偶然复制的 4K 电影的文件夹。如果一个程序与另一个程序相差几 MB，那也没什么。生活还要继续。

我还喜欢 Wiztree 如何使用标签来组织其更通用的树视图，以了解哪些文件夹在搜索中占用了太多空间，以及它的文件视图，这使得它非常容易看到您可能想要删除哪些大文件。右键单击任何文件以弹出通常的 Windows 上下文菜单，然后您可以使用该菜单在文件的确切位置加载文件资源管理器的实例。你觉得合适就删掉。

* * *

你有一个你绝对喜欢的 Windows 应用程序(付费或免费)吗？跟我们说说:[](mailto:david.murphy@lifehacker.com?subject=Windows%20App%20of%20the%20Week)**。**