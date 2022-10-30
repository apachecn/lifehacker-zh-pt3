# 如何在任何运行 Android Marshmallow 或更高版本的手机上安装谷歌助手

> 原文:[https://life hacker . com/how-to-get-Google-assistant-on-any-phone-running-androi-1787706402](https://lifehacker.com/how-to-get-google-assistant-on-any-phone-running-androi-1787706402)

谷歌助手 [新的智能、对话式虚拟助手](https://lifehacker.com/all-the-things-you-can-do-with-google-assistant-that-yo-1787444497) ，遗憾的是只对 [他们的新 Pixel 手机](http://lifehacker.com/everything-google-announced-at-its-made-by-google-eve-1787404179) 正式可用。然而，只要稍加调整，你就可以在任何运行 Android Marshmallow 或更高版本的手机上获得它，以及 Assistant 的所有强大的搜索和聊天功能。以下是方法。

Watch

谷歌助手，一旦你尝试了，是非常有用的。每天早上你都可以得到一份每日简报，告诉你所在地区的天气、上下班路上的交通状况以及你当天的日程安排。你也可以用手机进行复杂的对话。例如，当你问正在上映什么电影时，你可以通过询问放映时间、评论等等来跟进。你所有的 [旧的最喜欢的语音命令](http://lifehacker.com/everything-you-didnt-know-you-could-do-with-google-voi-512727229#_ga=1.33219710.1347662518.1465819317) 仍然存在，但整个体验更好。如果你喜欢调整你的手机，那就值得一试。

### **你需要什么**

令人惊讶的是，在手机上安装谷歌助手比你想象的要容易。为了简化起见，我们将在你的手机上调整一个名为 *build.prop* 的文件，其中包含了很多关于你手机的信息。我们将改变它，这样当一个程序问“你是什么手机？”它回答“我是像素 XL！”而不是你有的任何一部手机。这是一个风险最小的简单调整。

有几种方法可以做到这一点。**方法#1** 涉及直接编辑 build.prop 文件，需要 root，而**方法#2** 会 flash 一个. zip，可以为你应用 tweak，不需要 root。这是两种方法都需要的东西:

*   安卓牛轧糖:这个调整只适用于运行最新版本安卓系统的手机。这包括 Nexus 6P、5X 6 和 5。你可以在这里 看到这个调整被 [确认的设备更新列表。](http://forum.xda-developers.com/android/software/guide-how-to-enable-google-assistant-t3477879)
*   **Root 访问权限(*方法#1* ):** 如果你想手动更新你的 build.prop 文件，你需要在你的手机上有 Root 访问权限。如果你还没有这样做的话，看看我们的指南 [如何给你的手机](http://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) 。
*   **一个根文件浏览器(*方法#1* ):** 任何允许你编辑根文件的文件编辑器都可以工作，所以你可以选择。我们将重点关注 [我们最喜欢的文件管理器固体资源管理器](http://lifehacker.com/the-best-file-management-app-for-android-5825578) 。
*   **可闪。zip 文件(*方法#2* ):** XDA 用户 [FaserF](http://forum.xda-developers.com/member.php?u=6105718) 已共享 [flashable。这里有压缩文件](https://www.androidfilehost.com/?w=files&flid=121914) ，你可以用它来编辑你的 build.prop，而不用启动你的手机。在继续之前下载它们。
*   **解锁引导加载程序(*方法#2* ):** 为了刷新。zip 文件，你需要解锁你的手机的引导程序。注意，这不同于给你的手机找根，但它仍然需要一点技术知识。我们的生根指南 [解释了区别和如何开始](http://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) 。
*   **定制恢复或快速启动(*方法 2* ):** 你需要一种方法来刷新你的。压缩文件。如果您的手机上已经有自定义恢复功能，您可以使用它。如果您不想麻烦自定义恢复，您可以使用快速启动来刷新文件。我们将重点关注使用自定义恢复，但是你可以在这里阅读更多关于 [如何使用 adb 和 fast boot](http://lifehacker.com/the-most-useful-things-you-can-do-with-adb-and-fastboot-1590337225)。

虽然启用 Google Assistant 很容易，但在继续操作之前，您仍然可以轻松地使用命令行、将文件刷新到手机以及修改系统设置。

此外，请记住，谷歌可以在任何时候修补这一点，所以它可能今天工作，但不一定明天。最后，如果你是 Android Beta 计划 的 [部分，未来的更新(如本月晚些时候即将到来的](http://lifehacker.com/skip-the-line-and-upgrade-your-nexus-to-android-nougat-1785653449) [Android 7.1 开发者预览版](http://lifehacker.com/android-7-1-developer-preview-will-roll-out-to-android-1787672852) )可能会扰乱你的 root 访问权限，并最终让你头疼。只要你愿意冒险，就继续吧！

**更新:**在我们完成本指南后不久，Xposed 模块 Android N-ify 进行了更新，为 Marshmallow 上的设备添加了 Google Assistant 的兼容性。你可以在 [这里了解更多](http://lifehacker.com/android-n-ify-update-brings-google-assistant-to-marshma-1787742400) 。如果你在棉花糖上，想要助手，你需要 [root 你的手机](http://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) ， [安装 Xposed](http://lifehacker.com/how-to-create-your-own-customized-version-of-android-wi-1440101209) ，然后 [安装 Android N-ify](https://ci.paphonb.xyz/jenkins/job/AndroidN-ify/) 。然后，您可以像往常一样继续本指南，尽管我们推荐方法#1，因为您已经拥有了 root 访问权限。

### **方法#1:手动编辑 Build.prop 文件(需要 Root)**

如果你已经在手机上有根权限，这个调整很容易。一旦你有了上面列出的所有项目，请遵循以下步骤:

1.  打开 Solid Explorer。(您首选的根文件资源管理器应用程序的步骤可能略有不同)。
2.  如果您尚未启用根存储，请滑出左侧面板并点击设置齿轮图标。滚动到底部并启用“显示根存储”退出设置。
3.  滑出左侧导航面板并点击 Root。
4.  向下滚动并点击系统。
5.  向下滚动并点击“build.prop”
6.  使用 SE 文本编辑器打开文件。
7.  找到显示 ro . product . model =[您的设备]的行，并将其替换为以下内容:ro.product.model=Pixel XL
8.  在单独的行中添加以下内容:ro.opa.eligible_device=true
9.  保存并退出文件。
10.  重启你的设备。

重新启动后，导航到设置应用程序的应用程序部分，找到谷歌应用程序，清除其数据和缓存。应用程序重启后，你应该可以通过长按 home 键来激活谷歌助手。恭喜你！手机还没上市，你就有了像素专属功能。

### 方法二:闪光。Zip 文件

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-hjt4karDZNM&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-hjt4karDZNM&start=0) 

XDA 用户 [FaserF](http://forum.xda-developers.com/member.php?u=6105718) 创造了一些方便的 flashable。如果你不想 root 你的手机可以使用的 zip 文件。如果你想通过 [安卓测试程序](http://lifehacker.com/skip-the-line-and-upgrade-your-nexus-to-android-nougat-1785653449) 获得早期更新，避开 root 可能会很方便。您可以使用自定义恢复来刷新。zip 文件，或 [使用 fastboot 从您的计算机](http://lifehacker.com/the-easiest-way-to-install-androids-adb-and-fastboot-to-1586992378) 中这样做。我们将向您展示如何使用自定义恢复来实现这一点，但是您使用的方法取决于您自己。

1.  XDA 用户 [mjp93](http://forum.xda-developers.com/member.php?u=4739170) 建议在继续此方法之前完全卸载谷歌应用。
2.  下载 [三。从这个链接](https://www.androidfilehost.com/?w=files&flid=121914) 压缩文件，并复制到你的手机的内部存储。
3.  重启你的手机进入恢复模式。
4.  点击或导航以在您的自定义恢复中安装。对于流行的 TWRP 恢复，安装将是一个大的灰色按钮在第一个屏幕上你看到的恢复。
5.  安装 GoogleAssistantVelvet.zip
6.  安装 GoogleAssistantBuildProp.zip
7.  重启你的手机。

一旦你的手机重新启动，你需要手动授予它使用麦克风等东西的权限，方法是转到设置应用程序的应用程序部分。从那里，找到谷歌，然后点击权限，并启用必要的权限。再次长按 home 键调出助手。