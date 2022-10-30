# 下面是 Android N 中自由形式窗口的样子，以及如何自己尝试

> 原文：<https://lifehacker.com/heres-what-freeform-windows-in-android-n-look-like-and-1766353465>

当 [谷歌宣布 Android N](http://lifehacker.com/all-the-new-features-coming-in-android-n-1763790001) 时，他们展示了分屏多任务处理，可以让你在同一个屏幕上同时使用多个应用。这看起来很不错，但是隐藏在表面之下的是更酷的东西:自由形式的窗口。下面是它的实际效果，以及如何亲自尝试。



### **自由形式的窗口将改变 Android 的工作方式**

谷歌长期以来一直致力于 Android 中的多任务处理。去年，当谷歌发布 Android M 开发者预览版 时，有一个隐藏的分屏功能 被埋在里面 [，它从未完整地最终发布。然后 Android N 预览版一出](http://lifehacker.com/enable-the-hidden-experimental-multi-window-feature-in-1737116053) 就变成了官方 [。现在，玩 Android N 预览版的开发者和修补者已经发现了隐藏在其中的多任务处理的下一次进化:它被称为自由形式窗口。](http://lifehacker.com/all-the-new-features-coming-in-android-n-1763790001)

要在自由模式下启动应用程序，请按 square Recents 按钮。这将打开你通常的，名片夹风格的多任务菜单。在每个应用程序的标题栏中，有一个小正方形图标，图标内有另一个正方形。当你点击它时，它会在自由工作空间中打开应用程序。

自由工作空间是一个专用的桌面，您可以在其中打开任意数量的应用程序并调整其大小。你可以拖动窗口的边缘或角落，将它们调整到任意大小，就像你习惯的所有桌面操作系统一样。只是不要完全覆盖另一个 app。自由形式模式缺少任何形式的任务栏或应用程序切换，因此很容易丢失窗口。

只要你处于自由模式，你启动的任何应用程序都将作为窗口应用程序弹出。然而，这有点难做到，因为在自由模式下没有应用程序启动器。如果您从另一个应用程序中打开一个应用程序(例如，您可以从通知阴影中打开设置)，它将以窗口模式启动。然而，如果你按下 Home 键并从常规启动器打开一个应用程序，它将以正常的全屏模式打开。

当您离开自由形式模式时，工作区和其中的所有窗口都以其最后的状态保存，直到您返回。例如，你可以点击 Home 按钮，打开另一个应用程序并像正常一样在全屏模式下使用它，然后点击 Recents 按钮返回自由模式。

这种方法乍一看似乎有点奇怪。目前还不清楚这项功能的完成情况，甚至不知道它将于何时发布。根据 [谷歌的开发者文档](http://developer.android.com/preview/features/multi-window.html#overview) ，Android N 设备的制造商可以选择是否启用自由形式支持。这可能意味着 Android N 设备将推出自由形式支持，但鉴于这一功能尚未完成，这似乎不太可能很快实现。话说回来，离 Google I/O 还有几个月，也许我们会感到惊讶。

### **如何亲自尝试**

在这一点上，你可能想自己尝试一下，我不能责怪你。Android 上的自由形式窗口已经很棒了。在一个合适的大屏幕设备上，它们可以改变你使用 Android 的方式。不过现在，它们是一个尚未发布的操作系统的未完成开发者预览版中的一个隐藏的实验性功能。尝试这种方法并不容易，也不安全，而且很可能已经坏了一半。如果你还和我在一起，以下是你自己尝试自由模式的方法。

#### **选项#1:在模拟器中尝试一下**

到目前为止，最简单的选择是使用 Android Studio 内置的模拟器。如果你还没有安装 Android Studio，请查看我们的指南 [作为 Android 开发人员的入门指南](http://lifehacker.com/i-want-to-write-android-apps-where-do-i-start-1643818268) 。你还需要确保你已经下载了[Android N SDK 组件](http://developer.android.com/sdk/index.html) 。如果这些听起来太吓人，你可能不应该尝试这个。

一旦你有了所有这些部分，你将需要 [创建一个运行 Android N 开发者预览版的 Android 虚拟设备](http://developer.android.com/tools/devices/index.html) 。以下是创建您需要的 AVD 的方法:

1.  在 Android Studio 中，打开 AVD 管理器。
2.  单击创建虚拟设备。
3.  选择一个与 Android N 兼容的预设配置文件。我用的是 Nexus 9，因为它为调整窗口大小提供了最大的自由空间。单击下一步。
4.  在系统映像屏幕上，单击“显示可下载的系统映像”
5.  选择 ABI 下标有“x86”的 N 版本。这可能需要一段时间来下载。完成后，选择该系统映像并单击 Next。
6.  选择方向旁边的“横向”。这在技术上是不必要的，但是我发现当你使用 windows 时，默认情况下进入横向模式更容易。其余的默认选项应该没问题。
7.  单击完成创建您的 AVD。

一旦完成，启动你的 AVD。然后，您需要做一些调整，以获得在模拟器中自由工作。为此，你就需要使用 [和](http://lifehacker.com/the-most-useful-things-you-can-do-with-adb-and-fastboot-1590337225) 。打开命令提示符，按照下列步骤操作:

1.  输入`adb shell`
2.  输入`su`
3.  输入`setenforce 0`
4.  输入`settings put global enable_freeform_support 1`
5.  输入`cd /data/local/tmp`
6.  输入`mkdir permissions`
7.  输入`cd permissions`
8.  输入`cp -a /system/etc/permissions/* ./`
9.  输入`sed -e “s/live_wallpaper/freeform_window_management/” android.software.live_wallpaper.xml >freeform.xml`
10.  输入`mount --bind . /system/etc/permissions`
11.  等待几秒钟
12.  输入`stop`
13.  再等几秒钟
14.  输入`start`

之后，您的模拟器将重新启动，您可以开始玩自由形式的窗口。

#### **选项 2:在 Nexus 设备上启用自由格式**

在手机或平板电脑上尝试自由模式可能比使用模拟器更冒险。如果你注册了 [安卓测试计划](http://lifehacker.com/how-to-install-the-android-n-developer-preview-on-your-1763813851) ，它很可能会搞砸谷歌未来推出的任何 OTA 更新。你可能不会把你的设备做成砖块，但是仅仅为了重新注册测试版而把它重新放回库存会很痛苦。最起码，的[后备装置伤不了](http://lifehacker.com/how-to-set-up-a-fully-automated-app-and-settings-backup-5784857)的。如果你真的想尝试一下，那就继续。

首先，你需要 [安装一个自定义的恢复像 TWRP](http://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) 。完成后，请遵循以下步骤:

1.  启动到您的自定义恢复。
2.  以读写方式挂载系统。
3.  打开一个亚行外壳。
4.  输入`cd /system/etc/permissions`
5.  输入`sed -e “s/live_wallpaper/freeform_window_management/” android.software.live_wallpaper.xml >freeform.xml`
6.  重启进入 Android，打开另一个 ADB 外壳。
7.  输入`settings put global enable_freeform_support 1`
8.  重新启动您的设备。

你可以在安卓警察这里找到更多关于这些指令 [的信息。**如果这里有你不明白的命令，一定要先研究一下**。如果你不确定从哪里开始，](http://www.androidpolice.com/2016/03/21/android-n-feature-spotlight-freeform-window-mode-offers-true-windowed-multitasking-but-its-disabled-by-default/)[XDA 论坛](http://www.xda-developers.com/) 是一个极好的资源。

* * *

到目前为止，Freeform 还存在很多问题，但是它展示了很多希望，以及 Android 的美好未来。到目前为止，谷歌进入笔记本电脑世界的唯一入口是 Chrome OS，与 Android 相比，它相对有限。如果 Freeform 允许开发人员将他们的 Android 应用程序发布到传统的窗口操作系统中，我们可能会看到 Android 发展成为一个桌面操作系统，有一天你可能会在笔记本电脑和手机上看到它。就目前而言，它只是在玩谷歌未来将发布的玩具。