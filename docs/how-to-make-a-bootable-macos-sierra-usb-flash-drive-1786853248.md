# 如何制作可启动的 macOS Sierra USB 安装驱动器

> 原文：<https://lifehacker.com/how-to-make-a-bootable-macos-sierra-usb-flash-drive-1786853248>

如果你想全新安装 [macOS Sierra](http://lifehacker.com/all-the-new-stuff-in-macos-sierra-1786817117) ，或者你有多台 MAC 要安装它，那么一个可启动的闪存驱动器是你轻松安装的最佳选择。下面是制作一个的方法。



### 简单的选择:磁盘创建器

创建 USB 闪存安装程序最简单的方法是使用免费程序 Disk Creator。

1.  下载 [macOS Sierra 安装程序](http://go.redirectingat.com/?id=33330X911647&site=lifehacker.com&xs=1&isjs=1&url=https%3A%2F%2Fitunes.apple.com%2Fus%2Fapp%2Fmacos-sierra%2Fid1127487414%3Fmt%3D12&xguid=7701797331255e816207580aa8402705&xuuid=786e7c6a79ebda249dae9a45ad684c07&xsessid=b81043f738f8389d189e2386e27ad6bc&xcreo=0&xed=0&sref=http%3A%2F%2Flifehacker.com%2Fall-the-new-stuff-in-macos-sierra-1786817117&pref=http%3A%2F%2Flifehacker.com%2F&xtz=420&abp=1) 和 [磁盘创建器](http://macdaddy.io/install-disk-creator/) 。
2.  插入 8GB(或更大)的闪存驱动器。如果你的闪存盘上还有其他数据，现在就备份，因为安装程序会删除所有数据。
3.  打开光盘制作程序，然后点按“选择 OS X 安装程序”按钮。
4.  找到 Sierra 安装程序文件。这应该位于您的应用程序文件夹中。
5.  从下拉菜单中选择您的闪存驱动器。
6.  点按“创建安装程序”

完成后，将您的 USB 驱动器插入任何 Mac，然后在启动电脑时按住 Option 键启动安装程序。

### DIY 选项:终端

如果您不想下载额外的软件，您可以使用终端制作自己的安装程序 USB 驱动器。

1.  下载 [macOS Sierra 安装程序](http://go.redirectingat.com/?id=33330X911647&site=lifehacker.com&xs=1&isjs=1&url=https%3A%2F%2Fitunes.apple.com%2Fus%2Fapp%2Fmacos-sierra%2Fid1127487414%3Fmt%3D12&xguid=7701797331255e816207580aa8402705&xuuid=786e7c6a79ebda249dae9a45ad684c07&xsessid=b81043f738f8389d189e2386e27ad6bc&xcreo=0&xed=0&sref=http%3A%2F%2Flifehacker.com%2Fall-the-new-stuff-in-macos-sierra-1786817117&pref=http%3A%2F%2Flifehacker.com%2F&xtz=420&abp=1) 。
2.  插入一个 8GB(或更大)的闪存驱动器，并给它一个名称。对于本教程，我们将使用名称`Untitled`。确保驱动器已格式化为 OS X 扩展(日志式)。如果不是，打开磁盘工具，格式化就是这样。在此之前，请备份该驱动器上的所有重要数据。最好断开任何其他外部硬盘或闪存驱动器，这样就不会混淆。
3.  打开终端(应用程序>实用程序)。
4.  在终端中输入(或者复制粘贴)这个命令，用你的驱动器名替换`Untitled`，然后按回车键: `sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ macOS\ Sierra.app --nointeraction &&say Done`
5.  出现提示时键入您的密码，然后按 Enter 键。
6.  让命令行完成它的工作，不要打断它，直到你看到最后一行写着`Done`。这可能需要一段时间，所以请耐心等待。

完成后，将您的 USB 驱动器插入任何 Mac，然后在启动电脑时按住 Option 键启动安装程序。