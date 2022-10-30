# 如何将 DVD 翻录到电脑上

> 原文：<https://lifehacker.com/how-to-rip-a-dvd-to-your-computer-5809765>

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-F_dw0NTVZiQ&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-F_dw0NTVZiQ&start=0) 

假设你有一部电影的 DVD，但你想在手机、平板电脑或其他地方观看。您可以“翻录”该 DVD，或者将其转换为电脑上的电影文件，以便在任何地方播放。下面是怎么做的。



将电影翻录到硬盘上看起来很复杂，但实际上非常简单。有很多方法可以做到这一点，也有很多不同的程序，但我们最喜欢的方法是使用一个名为 [**手刹**](http://handbrake.fr/) 的程序。它很容易使用，适用于 Windows，Mac 和 Linux，它可以将你的文件转换成任何设备的兼容格式，如 iPad 或 Android 手机。上面的视频应该会引导你完成这个过程，但是你也可以按照这些指示去做。

1.  进入 [手刹主页](http://handbrake.fr/) 下载程序。按照指示将其安装到您的计算机上。
2.  默认情况下，手刹可以翻录未受保护的 DVD，但你从商店购买的大多数 DVD 都有复制保护。要解决这个问题，您需要安装 libdvdcss。在 Windows 上，你可以单独下载这个文件(这里的 [用于 32 位系统](http://download.videolan.org/pub/libdvdcss/1.2.11/win32/libdvdcss-2.dll) 这里的 [用于 64 位系统](http://download.videolan.org/pub/libdvdcss/1.2.11/win64/libdvdcss-2.dll) )，~~重命名为 libdvdcss.dll~~保留文件名为 libdvdcss-2.dll，放入你的手刹程序文件夹(C:\Program Files\Handbrake)。如果你在 Mac 上， [下载这个文件](http://download.videolan.org/pub/libdvdcss/1.2.11/macosx/libdvdcss.pkg) 双击安装。*如果你运行的是 OS X El Capitan，你还需要几个步骤——在做其他事情之前，先看看这篇文章的底部。*
3.  插入您想要翻录的 DVD，并打开手刹。
4.  点按左上角的“源”按钮，并从列表中选取您的 DVD 驱动器。它将开始扫描您的 DVD，这可能需要几分钟时间。
5.  完成后，进入窗口左上角的“标题”下拉菜单。您可以在这里选择要翻录的 DVD 部分。就电影而言，它通常是最长的标题，所以就选那个吧。如果你要翻录一个电视节目的片段，通常是 22 分钟或 44 分钟的片段，你必须分别翻录。
6.  单击窗口右侧的浏览按钮。导航到要保存电影文件的位置，并在框中键入文件名。单击确定。
7.  接下来，前往右边标有“预设”的栏。您可以在这里选择结果文件的格式。如果你只是想在电脑上看的话，“普通”或者“高调”的预设就可以了。但是，如果你想在 iPod 或 iPhone 上观看，请从列表中选择正确的预设。
8.  点击窗口顶部的开始按钮。这需要一段时间，所以你可能会想要喝杯茶。
9.  完成后，你会得到一个弹出通知。从那里，你可以双击你的电影文件观看，或同步到你选择的设备。尽情享受吧！

起初看起来需要很多步骤，但实际上并不难——尤其是在你第一次完成之后。例如，一旦安装了 libdvdcss 文件，以后就可以跳过这一步。

Mac 用户，特别是那些运行 OS X El Capitan 的用户，必须处理 [系统完整性保护](https://en.wikipedia.org/wiki/System_Integrity_Protection) (SIP)，这是一种旨在保护关键系统文件和进程 的安全功能。可惜 [SIP 坏了很多软件](http://lifehacker.com/how-to-see-all-the-software-disabled-by-os-x-el-capitan-1735489877) ，去掉了手刹为了工作需要的 libdvdcss 文件。您可以禁用 SIP，但它很有用，您不应该非禁用不可。除此之外，还有一个更好的办法， [正如 redditor hvyboots 指出的](https://www.reddit.com/r/osx/comments/3n6gz4/el_capitan_apparently_broke_handbrake_ripping/cvmc4pf) :

1.  关闭手刹，并打开一个新的取景器窗口。

2.  键入 *cmd+shift+G* ，粘贴到以下路径:`/Library/SystemMigration/History/`

3.  在这个文件夹中应该有一个名为“迁移-[随机字母和数字]”的文件夹打开那个文件夹，你会发现“隔离根”打开该文件夹，您应该会看到您的 *libdvdcss.2.dylib* 文件。

4.  打开第二个 Finder 窗口。

5.  键入 *cmd+shift+G* ，粘贴到这个路径:`/usr/local/lib`(如果你得到一个错误消息说这个文件夹不存在，转到`/usr/local`，创建一个名为“lib”的新文件夹，打开它。)

6.  将 libdvdcss.2.dylib 文件从第一个窗口拖放到`/usr/local/lib`文件夹中。应该会提示您输入管理员密码。输入并等待复制完成。

确保在完成此操作后重新启动手刹，因为应用程序将扫描 libdvdcss 文件，一旦检测到它，您就不必移动它或再次处理它。然后你就可以像平常一样按照上面的指示去做，然后撕掉！

只需要从 DVD 中挑选合适的章节，然后将其转换成合适的格式。请注意，如果你要翻录很多 DVD，你可以进入工具>选项(或者手闸>偏好设置，如果你在 Mac 上)，点击“默认路径”旁边的“浏览”，为你将来翻录的所有其他电影选择一个位置。你也可以点击“添加到队列”而不是“开始”，一次翻录多个文件，这对翻录电视节目非常有用。

祝你好运，享受你新翻录的 DVD！如果你也想破解蓝光，你只需要做一点额外的工作。查看 [我们的蓝光抓取指南](https://lifehacker.com/the-hassle-free-guide-to-ripping-your-blu-ray-collectio-5559007) 了解更多。

*<small>视频音乐由</small>* [*<small>蓝精灵</small>*](http://freemusicarchive.org/music/Smurd/Mo_Gear/) *<small>组成。</small>T15】*