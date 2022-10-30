# 如何在 Android 上启用 Snapchat 的新 Alpha UI

> 原文：<https://lifehacker.com/how-to-enable-snapchats-new-alpha-ui-on-android-1828472654>

自 2017 年该公司首次进行重大更新以来，Android Snapchat 用户一直在等待这款流行的社交媒体应用程序的更快、更稳定的版本。新版本终于接近全面发布，由于 XDA 开发者米沙·拉赫曼的一些出色工作，一些 Android 用户现在可以试用新版 Snapchat 的 Alpha 版本。如果你对 Snapchat 这个速度更快的新版本感到好奇，并且不想等待，下面是如何在手机上安装它的方法:

### 支持你的安卓手机

在我们开始之前，有几个小警告。首先，这个版本的 Snapchat 是一个 alpha 版本，这意味着它是不完整的，可能有一些缺失的功能、错误或稳定性问题。

Watch

第二个警告更严重:启用 Snapchat Alpha 将需要 root 用户权限才能访问手机的内部文件。这可能是一个有风险的过程，如果你不确定该做什么或摸索一个重要的步骤，它可能会导致一些相当大的问题。这些潜在的风险包括:性能不稳定，应用程序故障，甚至智能手机死机。此外，拔掉手机可能会使你的保修失效——就像，如果出了问题，你将无法打电话给制造商寻求帮助。

扎根于你的设备的结果是，你将拥有对手机内部存储的完全访问权，你将能够安装应用程序和工具，让你以独特的方式操作你的文件和设备的设置。关于什么是寻根，以及如何/为什么这么做的完整解释，请查看我们的[Android 手机](https://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397#_ga=2.191717294.581236602.1534771213-3846207152.1521480874) 寻根初级指南，其中也包括特定设备的寻根资源。

如果出于任何原因，你决定不 root 你的手机，一旦新版本的 Snapchat Android UI 正式推出，你仍然可以使用它(尽管我们不知道确切的时间)。此方法仅适用于访问未发布的 alpha 版本。

### 所需材料

随着这些警告的消失，让我们开始运行闪亮的新 Snapchat 界面。这是你需要的:

*   启用了 root 访问和开发者模式的 Android 手机
*   Snapchat 应用程序的最新版本
*   安装了最新 ADB 二进制文件的计算机
*   连接您的手机和 PC 的 USB 电缆

### 更新您的 Snapchat 应用程序

自然，为了启用最新的功能，我们需要最新版本的 Snapchat 应用程序。为了访问 alpha 版本，您需要运行 10.39 或 10.39.1 beta。

打开 [Snapchat 的谷歌 Play 商店](https://play.google.com/store/apps/details?id=com.snapchat.android&hl=en_US) 页面，看看是否需要更新。如果你没有运行 10.39 或 10.39.1 测试版，但 Play Store 没有显示你已经准备好更新，你可以从 APKMirror 下载最新的 Snapchat APK并将其下载到你的设备上。

### 调整 Snapchat 以启用 alpha 访问

安装了正确的版本后，事情会变得稍微复杂一些。我们将在您手机的 Snapchat 目录中编辑一个文件，这需要一些精确的步骤。首先，如果你还没有 root 你的手机，现在是时候了。如上所述，请参考 [我们的手机寻根指南](https://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397#_ga=2.158274878.581236602.1534771213-3846207152.1521480874) 了解如何进行深入指导。

一旦你的手机被 root，你需要下载一个支持 root 的文件浏览器软件，它将允许你编辑文件。

有多个支持根的文件浏览器，比如 [MiExplorer、](https://labs.xda-developers.com/store/app/com.mixplorer) [FX 文件浏览器](https://play.google.com/store/apps/details?id=nextapp.fx&hl=en_US) 等等，尽管这里我们将使用 MiXplorer。

安装 MiXplorer 后，打开应用程序。在左侧工具栏中，有一个“**根目录**的选项。点击这个，应用程序会要求您进行 root 访问。授予它访问权限，从这里，您可以访问手机上的所有文件，包括系统和应用程序关键文件。

打开名为**数据**的文件夹，然后再次滚动到**数据**。在这个文件夹中，找到 **com.shapchat.android** ，再找到 **shared_prefs** 。

接下来，打开标记为“**dynamicapconfic . XML**的文件在文档中搜索短语**“app family”**，找到我们需要编辑的字符串。完整字符串应读作: **<字符串名称“【应用家族】>snapchat</字符串>** 。在此字符串中，将单词“snapchat”替换为“mushroom”该字符串现在应该读作: **<字符串名称“【app family】>蘑菇</字符串>** 。

保存文件，然后退出 MiExplorer。

在应用抽屉中找到您的 Snapchat 应用，按住图标，直到您可以访问应用信息页面。在那里，选择“强制关闭 Snapchat”

### 启用开发人员模式和 USB 调试

由于下一步将要求您将手机连接到计算机进行更改，您需要启用 USB 调试。

为了做到这一点，你需要进入开发者模式。在你设备的**系统设置**，进入**设置**、**关于手机**，然后**软件信息**。向下滚动并反复点击**内部版本号**，直到你得到开发者模式已开启的通知。

返回到**设置**菜单，然后选择**开发者选项**。滚动直到找到调试部分，然后打开 **USB 调试**。

这些是最初的电话步骤。接下来，我们需要将手机连接到您的 PC 以完成该过程。

### 在你的电脑上

通过 USB 将您的手机连接到 PC，开始这一部分的过程。

如果你还没有，你需要下载最新的亚行二进制文件( [你可以在这里找到我们的指南](https://lifehacker.com/google-finally-lets-you-download-adb-and-fastboot-as-st-1790840830) )。

从“开始”菜单打开计算机上的命令提示符或 Windows PowerShell，或者按下 **Window+X** 键。如果找不到，也可以使用搜索栏。在 Linux 上，按 **Ctrl+Alt+T，**，macOS 用户可以在**应用>实用程序**中打开终端应用。

在命令提示符窗口中，输入保存 ADB 二进制文件的目录。

一旦到了那里，下一步就是打开 ADB 的外壳。在 Windows 命令提示符下，键入命令 **adb shell** 并按 enter 键访问 adb shell。如果你碰巧用的是 Windows PowerShell，用:**。\adb shell** 。macOS 和 Linux 用户将使用**。/亚行外壳**。

一旦访问了 ADB shell，输入命令: **su** 并按 enter 键，接受授予 root 访问权限的请求。

之后，逐个输入这些命令:

*   **pm 启用 com.snapchat.android/com.snap.mushroom.MushroomMainActivity**T2】
*   **pm 启用 com.snapchat.android/com.snap.mushroom.MainActivity**T2】
*   **pm 禁用 com.snapchat.android/.LandingPageActivity**

一旦命令完成，关闭命令提示窗口，并安全地断开您的电话从您的电脑。

如果您完成了这些步骤，您现在已经启用了新的 Snapchat UI 重新设计。还不算太糟，是吧？

*<small>**更新(8/21):** 我们给</small>*[*<small>【XDA】添加了一个归属地——开发者</small>*](https://www.xda-developers.com/enable-snapchat-alpha-faster/) *<small>，这个我们在本文的原始版本中省略了。</small>*