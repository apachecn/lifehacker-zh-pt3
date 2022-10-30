# 如何用 Remix OS 把 Android 放到你的桌面上

> 原文：<https://lifehacker.com/how-to-put-android-on-your-desktop-with-remix-os-1752731845>

[Remix OS](http://www.jide.com/en/remixos-for-pc) ， [昨天出来的](http://lifehacker.com/remixos-brings-desktop-style-android-to-intel-based-pcs-1752436333) ，是一个杀手级的安卓变种，给安卓带来了一个圆滑的桌面风格界面。现在，你可以把它安装在 u 盘上，在电脑上试用。

Watch

Android [并不完全是为键盘鼠标](http://gizmodo.com/google-pixel-c-review-androids-not-ready-for-a-tablet-1747368432#_ga=1.97940058.431406394.1415821409) 打造的，但这并没有阻止我们中的一些人尝试。来自开发者 [Jide](http://www.jide.com/en) 的 [RemixOS](http://www.jide.com/en/remixos-for-pc) ，想要通过给 Android 添加桌面、窗口应用等来改变这一点。以下是如何尝试*非常*实验阿尔法。

**免责声明:**根据 Jide 的网站，这个 OS 是“为不介意一两个 bug 的开发者和早期采用者准备的。”在我们的测试中，有两个以上的错误。虽然 RemixOS 是一个很棒的概念，玩起来很有趣，但不要指望它会很快取代你现在的电脑。然而，如果你正处于风口浪尖，摆弄你的电脑，玩实验软件(这可能解释了你为什么阅读 Lifehacker)，无论如何，继续吧。

### **你需要什么**

默认情况下，RemixOS 运行在 u 盘上。你可以在*访客模式*中使用它，每次运行它都会在一个新的桌面上重新开始，或者在*常驻模式*中使用它，它会将你所有的应用程序和文件保存在 u 盘上，这样你以后就可以在任何计算机上继续你的会话。要创建您的 RemixOS 盘，您需要:

*   **RemixOS for PC package:** 你可以从这里 下载 RemixOS [的安装包。这个包只有不到 700MB，所以如果你的网速比较慢，就开始下载，然后吃点零食什么的。](http://www.jide.com/en/remixos-for-pc)
*   **一个 8GB+的 u 盘，写入速度为 20MB/s:**remix OS 需要至少 8GB 的可用存储空间来安装和运行。如果你计划使用常驻模式来保持你的桌面持久，你显然会想要更多。另外，Jide 推荐一个 20MB/s 写入速度的记忆棒(之前推荐的[SanDisk Extreme](http://www.amazon.com/exec/obidos/ASIN/B008AF384W/?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-put-android-on-your-desktop-with-remix-os-1752731845&asc_source=&rawdata=[r|https://www.google.com/[t|mod-title[p|707359862[a|B008AF384W[au|5716509846451982265&tag=kinjalifehackerlink-20)应该很好用)。在我的测试中，我发现一个写速度低于 10MB/s 的记忆棒可以工作，但它会抛出一个错误，并需要一段时间来加载。注意:创建 RemixOS 驱动器将会擦除您的 u 盘，所以请务必备份 u 盘上的所有文件。
*   基于 x86 的计算机: RemixOS 是 Android 的 x86 变体，因此，它只能在采用英特尔和 AMD 处理器的计算机上运行。基于 ARM 的电脑(比如很多 Chromebooks)和老款 MAC 都不行。你还需要一台 Windows 电脑来制作 u 盘。
*   **从 USB 启动已启用:**现在大多数计算机都有从 USB 启动的能力，但请检查您的 BIOS 或型号以确保这一点。你可以在我们的指南 中找到更多关于 [如何从 USB 启动的信息。](http://lifehacker.com/how-to-boot-from-a-usb-drive-or-cd-on-any-computer-5991848)

创建可引导 u 盘比大多数操作系统安装花费的时间要少，但仍然需要一点时间，所以要做好等待的准备。一旦你有了你需要的一切，就该开始了。

### **创建您的 RemixOS 盘**

首先，你需要创建一个可启动的 u 盘，RemixOS 可以在上面运行。一旦下载了 RemixOS 安装文件，请按照以下步骤操作:

1.  插入你的空白 u 盘。
2.  提取电脑 RemixOS 中的文件。zip 文件。
3.  启动 RemixOS USB 工具可执行文件。
4.  在“ISO”旁边，点击浏览按钮并选择混音。iso 文件。
5.  在“u 盘”旁边，选择与您插入的 u 盘相关的驱动器号。
6.  单击确定。

安装程序将立即开始创建您的 RemixOS 盘。这个过程需要几分钟。一旦完成，你就可以把它插到你的电脑上，从 USB 启动。正如我们上面简单提到的，当你第一次启动 RemixOS 时，你有两个选择。它们是这样工作的:

*   客人模式:这允许你预览 RemixOS 是如何工作的。一旦您关闭电脑，您安装的任何应用程序、更改的设置或下载的文件都将被抹掉。
*   **常驻模式:**这会把你的 u 盘当成一台便携电脑。无论您将它插入哪台计算机，您更改的任何设置都会被记住。你安装的应用程序和下载的文件将被写入 u 盘。这意味着你的 u 盘越大，你安装东西的空间就越大。

请记住，尽管 RemixOS 在 Android 上添加了许多软件，使其更加友好地使用鼠标和键盘，但大多数应用程序仍然是为触摸界面设计的。不管 RemixOS 做什么，它们可能都不太好用。Android 应用程序在传统界面上运行得相当好，但你仍然应该预料到路上会有一些颠簸。

### 安装一些应用程序(比如 Google Apps 和 Play Store)

不管宣传材料看起来如何，RemixOS 并没有预装谷歌 Play 商店或任何相关的谷歌应用程序。RemixOS 以前的限量发行版本有，所以不清楚这是不是一个疏忽，或者 Jide 只是没有公开发行 Play Store 的许可证。

幸运的是，你仍然可以自己下载和安装应用程序。APK 镜报 是一个优秀的网站，拥有大量流行应用的最新版本，包括谷歌服务。要获取 RemixOS 应用，请按照以下步骤操作:

1.  搜索 APK 镜报寻找你要安装的应用程序。
2.  如果适用，请确保您拥有正确的版本。作为参考，RemixOS 运行的是 Android 5.1.1。(根据 APK 镜报的说明，要安装 Google Play 服务，你需要以 270、 [结尾的版本。](http://www.apkmirror.com/apk/google-inc/google-play-services/google-play-services-8-4-89-2428711-270-android-apk-download/) )
3.  打开“设置”应用程序，点按“安全”，并启用从“未知来源”安装
4.  启动“下载”应用程序，点按您下载的 APK，然后按照提示进行安装。

在我的测试中，安装了 Google Play 服务，但许多功能仍然无法在访客模式下正常工作。Chrome 等一些应用程序启动了，运行得相对较好，而网飞等其他应用程序根本无法启动。同样，这些应用程序都不是为 RemixOS 设计的，所以如果一个应用程序不工作，不要责怪开发者。

### 那么，情况如何？

在经历了这一切之后，你可能会想，这一切麻烦是否值得。嗯，这里有一个简短的答案:有点？自从昨晚发布以来，我已经用它玩了几个小时，我遇到了足够多的问题，这些问题会让大多数普通用户敬而远之。不过没关系！这是一个面向开发者和爱好者的 alpha 版本。然而，起作用的东西为 Android 在桌面上描绘了一幅美好的前景。

首先，RemixOS 调整了 Android 的基本界面，让用户在桌面上感觉更加舒适。主屏幕底部有一个用于启动应用程序的任务栏，一个用于搜索文件和查找其他已安装应用程序的类似开始的菜单，一个用于 Wi-Fi 连接、日期和时间等内容的系统托盘，以及一个滑出式通知托盘。坦率地说，它看起来更像 Windows 10 的克隆版，而不是 Android。

Android 应用的扩展性也很好。RemixOS 允许你任意调整窗口大小，就像你在 windows 和 OS X 上做的一样。这似乎是一个显而易见的事情，但请记住，Android 应用程序从来不是为这种界面设计的。尽管如此，该功能运行得相当完美。如果你把窗口做得足够小，这个应用程序将默认为一个手机风格的界面。如果可能的话，较大的窗口将使用平板风格的界面。这意味着 Android 上的应用程序体验仍然只有 Android 对平板电脑应用程序的支持好，这是 [好，但不是恒星](https://lifehacker.com/lifehacker-pack-for-android-tablets-our-list-of-the-es-875602288) 。

最终，应用兼容性的问题意味着 RemixOS 不太可能取代任何人的日常驱动程序。然而，鉴于 Android 从未打算成为一个桌面操作系统，RemixOS 做了出色的工作，让我们相信它可以成为。

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=5789397,1637564101,1440101209&title=Keep Customizing That Android)