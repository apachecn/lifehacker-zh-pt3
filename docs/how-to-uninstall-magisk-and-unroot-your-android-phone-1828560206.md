# 如何卸载 Magisk 和 Unroot 你的 Android 手机

> 原文：<https://lifehacker.com/how-to-uninstall-magisk-and-unroot-your-android-phone-1828560206>

在你的 Android 智能手机上运行 [Magisk Manager](https://magiskmanager.com/) 的一个好处是 Magisk 可以隐藏特定应用程序的 root 访问权限，如果某个应用程序因为检测到你篡改了你的设备而无法启动，这很有帮助。然而，一些应用程序— [像口袋妖怪 GO](https://forum.xda-developers.com/apps/magisk/magisk-hide-pokemon-t3813961)—现在在运行时会专门检查 Magisk，这破坏了该软件的一个最佳功能。

Watch

由于 Magisk 没有太多的替代品，并且没有一个能够执行与 Magisk 相同的功能，所以捕捉动物的唯一真正选择是从您的设备中删除 Magisk(和 root 访问)。谢天谢地，你有一些方法可以选择:

### 轻松卸载 Magisk

从 Android 设备上卸载 Magisk 的第一个也是最简单的方法是从 Magisk manager 应用程序中卸载它。

确定您已接入互联网，然后从应用程序屏幕打开 Magisk 管理器。点击主屏幕底部的“卸载”按钮。

您将看到“恢复库存”、“完全卸载”或取消该过程的选项。若要移除 Magisk 和所有模块，请点击“完全卸载”

之后，Magisk Manager 将下载并运行必要的脚本，从您的手机中删除 Magisk，并恢复您的设备的原始固件。等待该过程完成，您就完成了！

### 另一种选择: Magisk TWRP 卸载实用程序

类似地，XDA 开发者论坛 上有一个 [Magisk 卸载程序实用程序，它将执行与上述相同的任务。对于那些因为任何原因无法通过自己的设备访问互联网的人来说，这也是一个很好的选择。](https://forum.xda-developers.com/apps/magisk/official-magisk-v7-universal-systemless-t3473445)

要运行该实用程序，您首先需要将软件直接下载到您的手机上，或者下载到另一台设备上，如您的台式机或笔记本电脑，然后手动将文件传输到您的手机上。然后，启动手机自定义恢复，如 TWRP，并打开卸载压缩文件。整个过程可能会变得相当复杂，但 Magisk 官方网站有关于如何在 TWRP 安装和运行卸载的 [详细说明。](https://magiskroot.net/uninstall-magisk-module-twrp/)

### 如何摆脱你的设备的根

Magisk 卸载后，下一步是撤销根本身。好消息是有很多方法可以做到这一点，而且都出奇的简单。

#### 手动删除根文件

使用具有 root 权限的文件管理器(如 [MiXplorer](https://labs.xda-developers.com/store/app/com.mixplorer) 或 [ES 文件浏览器](https://play.google.com/store/apps/details?id=com.estrongs.android.pop&hl=en_US) )，可以手动删除根文件。

我们首先要找到并删除标有**、【busybox】、**、【苏】、**的文件，这两个文件都保存在你手机的主驱动器中。它们将位于以下两个目录之一:**

**《统》>《宾》。**

或者

**【系统】>【xbin】**

一旦找到“ **busybox** ”和“ **su** ”，就删除它们。

我们需要删除的最后一个文件在**“系统”>app 中**打开那个文件夹，删除**“超级用户. apk”。**

关闭文件资源管理器，并重新启动设备。完成重新启动后，您就成功地从设备中移除了根目录，它应该会恢复正常。

#### 尝试使用 SuperSU

另一种方法是使用 [SuperSU app](http://www.supersu.com/) 。如果你不喜欢摆弄手机的系统文件，这可能是恢复手机的最好方法。

要以这种方式移除根，请打开应用程序。在“设置”标签中，轻按“完全取消根”之后，只需在必要时遵循屏幕上的提示，其余的将由应用程序和您的手机处理。最后，你的手机将被成功解锁。

#### 恢复库存固件

你可以使用的最后一种方法来摆脱你的根是安装最新的官方系统更新或重新安装你的设备的股票固件。

下载并安装智能手机操作系统的最新更新通常会从你的设备中删除根文件，这是一个相当简单的过程。但是，它需要您手动查找并下载更新文件。

同样，你可以通过重新安装手机的固件来简单地撤销根。这种方法将因人而异，因为每部手机都有不同的固件，需要定制步骤来完成安装过程。然而，像“[手机型号]固件恢复”这样的互联网搜索可能会给你指出正确的方向。