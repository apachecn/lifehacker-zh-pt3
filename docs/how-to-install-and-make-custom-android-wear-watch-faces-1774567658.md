# 如何安装和定制 Android Wear 手表表盘

> 原文:[https://life hacker . com/how-to-install-and-make-custom-Android-wear-watch-faces-1774567658](https://lifehacker.com/how-to-install-and-make-custom-android-wear-watch-faces-1774567658)

如果说我喜欢可穿戴设备的可能性，那就是换上新的表盘。虽然许多公司要么阻止用户定制手表表面，要么要求一些像样的编码技能，但 Android Wear 有一些变通办法——它们很棒。如果你想打造别人没有的属于你自己的定制表盘，请继续阅读。连 iOS 用户都可以！

Watch

我是一个 iPhone 用户，带着 Android Wear 手表。为什么？因为我认为 Apple Watch 是一种混乱的、毫无意义的技术。虽然谷歌的 Android Wear 平台在 iOS 上做得不太好，但我发现它的重点是让可穿戴体验*更好*，它实际上似乎可以更可靠地与我的手机配对。但不管你喜欢手腕上的什么平台，Android Wear 是唯一一个可以简单选择制作你自己的定制手表表面的平台。 [Gizmodo 详细介绍了几个安卓用户可以轻松使用的](http://gizmodo.com/design-your-own-android-wear-watch-faces-no-coding-req-1748087304) ，但在本帖中，我们将回顾一个甚至 iPhone 用户也可以使用的过程。

### iPhone 的困境

如果你进入 iPhone 上的 Android Wear 应用程序，你会在顶部找到一个手表面孔部分。当您点击“更多”按钮时，您可以在您的设备上选择手表面孔，或者点击屏幕底部的“获取更多手表面孔”来同步其他选项。与你的安卓手机朋友不同，你无法访问你在谷歌 Play 商店能找到的任何手表表盘。谷歌确实提供了一些很酷的选择，但我发现大多数都太局限了。它们看起来不错，但是很少提供有用的信息，也没有一个显示当前的温度。

### 如何将 Watch Faces 侧装到 Android Wear 上

我对我的选择不满意，就像谷歌产品一样，你通常可以找到大多数限制的解决方法。如果你想在你的设备上安装一个定制的手表表面，你可以直接将任何你能拿到的 APK 下载到你的 Android Wear 智能手表上。如果你已经准备好了，你只需要遵循几个步骤(并有一台电脑来完成它们):

1.  [在你的 OS X、Windows 或 Linux PC 上下载并安装 Android 开发者工具](http://developer.android.com/tools/help/adt.html) 。你真的只需要 adb 命令行工具，但这是正确设置一切的最快方法，这样你的电脑和手表就可以通信了。(如果你想这样做，你可以少安装一些， [下载 adb](https://drive.google.com/a/awkwardhuman.com/file/d/0B0MKgCbUM0itVVFWRC02Q0VBQnc/view?usp=sharing) 和 [谷歌 USB 驱动](http://developer.android.com/sdk/win-usb.html) 。你还需要为你的智能手表下载驱动程序。你只能靠自己了。
2.  在你的手表上启用开发者模式，就像你在 Android 手机上一样:打开设置，进入关于部分，然后一直点击内部版本号部分，直到手表告诉你你是一名开发者。
3.  回到设置菜单，进入新的开发者选项部分，启用 ADB 调试。(侧加载将通过 USB 进行，因此如果您愿意，可以禁用蓝牙调试。)
4.  拿起你想侧装的手表面 APK，改变它的文件扩展名。apk 到. zip。
5.  提取这个“压缩”文件，你刚刚作出的，并深入到实际的 APK 文件。您应该可以在/res/raw 中找到它。
6.  如果还没有，请通过 USB 将手表连接到电脑。

这五个步骤带你走了大部分的路，但是随着平台的不同，事情会有一点点的变化。从下面选择您的计算平台，完成侧面加载过程。如果你用的是 Linux，OS X 的指令应该几乎是一样的，所以你可以遵循这些指令，用你喜欢的命令行程序替换“Macintosh HD”和你的引导盘和终端的名称。

#### **在 OS X**

1.  打开终端(在 Macintosh HD →应用程序→实用程序中),通过 USB 将手表连接到电脑。
2.  键入以下命令(但不要按 enter！):`*./adb install*`
3.  在该命令之后，添加您想要侧加载的 APK 的位置(通过手动键入路径或将 APK 文件拖到终端窗口上)。该命令看起来应该是这样的:`*./adb install /Macintosh\ HD/locationofapk/apk.apk*`
4.  当你得到所有正确的，按下回车键，让亚行做它的事情。整个侧装过程大约需要一分钟。如果您没有得到即时反馈，也不要担心。可能需要一段时间才能让你知道发生了什么。

#### **在 Windows 中**

1.  通过在搜索中键入 cmd 打开命令提示符。为了确保一切正常，请键入`*adb devices*`以确保您的电脑可以看到您的手表。如果可以，您很可能会得到一个序列号，旁边有“设备”。
2.  键入以下命令(但不要按 enter！):`*adb install*`
3.  在该命令之后，添加您想要侧加载的 APK 的位置(通过手动键入路径或者只是将 APK 文件拖到命令提示符窗口上)。该命令看起来应该是这样的:`*adb install C:\Users\BestUserEver\locationofapk\apk.apk*`
4.  当你得到所有正确的，按下回车键，让亚行做它的事情。整个侧装过程大约需要一分钟。如果您没有得到即时反馈，也不要担心。可能需要一段时间才能让你知道发生了什么。

这听起来好像要做很多工作，但是一旦你知道你在做什么，这真的很容易。安装了手表表面后，您现在可以直接在手表上选择它(按住手表表面以显示选择屏幕)或在 Android Wear 应用程序中选择它。该应用程序将显示其名称，但不一定是预览图像，所以如果你侧载了很多手表的脸，你可能会有一些困难区分它们。幸运的是，这在你的 Android Wear 设备上不会成为问题。

### 从哪里获得新的表盘，以及如何设计自己的表盘

虽然加载任何一个令人敬畏的第三方手表表面都是令人敬畏的，但更令人敬畏的是从侧面加载你自己制作的手表表面。我想在我的手机上显示天气，但我也想要一些个性，所以我把我和我的男朋友(和他的狗——最后的结果见本文的上图)的一些像素艺术(在有才华的 [肖恩·沃顿](http://seanwarton.com/#/awkward-the-game/) 的帮助下)。现在我有了一个非常棒的个性化手表表面(你可以在上面看到)。如果你也想这样做，你有很多选择:

*   使用你已经安装的 Android 开发工具从头开始写一个。 [这些指令可以帮助](http://developer.android.com/training/wearables/watch-faces/index.html) ，但显然这是你能挑选的最耗时的选项。
*   使用 [WatchFacePro](http://www.watchfacepro.com/) 创建自己的。虽然该工具本身并不出色，而且有很多限制，但这个 webapp 可以免费快速生成一个简单、信息丰富、甚至动画的手表界面。不过，它没有显示天气的选项。
*   如果你有一部 iPhone，那么*不要*使用 Android 应用程序来制作一部， [如 Gizmodo 建议的](http://gizmodo.com/design-your-own-android-wear-watch-faces-no-coding-req-1748087304) 这些伟大的和前面提到的选项。如果你有一部安卓手机，它们会非常好用。如果你有一个 Android 设备来制作人脸，你或许可以让它工作，但将其转移到你的 iPhone 配对手表上会比它更麻烦。

除非你是一个精明的 Android 开发者(在这种情况下，你为什么要向我学习技巧？)，通过侧装第三方选项，您会发现更坚固的表盘。尽管如此，做出自己独特的设计通常会胜过附加功能。两种都试试，找出你喜欢的！不管结果如何，真的很好玩。

* * *

[<small>*亚当·达奇斯*</small>](http://adamdachis.com/) <small>*是洛杉矶的作家和顾问。你会发现他在*</small> [<small>*笨拙的人类*</small>](http://awkwardhuman.com/) <small>*写东西，包括他播客的*</small> [<small>*笨拙的人类生存指南*</small>](http://5by5.tv/awkward) <small>*。*</small>

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=1638552352,1632388855,1727727262&title=Get%20Busy%20With%20Android%20Wear%3A)