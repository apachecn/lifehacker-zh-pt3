# 如何入门苹果的 ARKit 增强现实平台

> 原文：<https://lifehacker.com/how-to-get-started-using-apple-s-arkit-augmented-realit-1797690723>

大多数人认为， [苹果的新智能手机“iPhone 8”，](http://gizmodo.com/apple-iphone-8-rumor-roundup-everything-we-think-we-kn-1797533947) 将于 2017 年 9 月发布。但是我可以自信地说，公司今年最具突破性的发布实际上发生在今年夏天早些时候，在加州圣何塞举行的 [苹果全球开发者大会(WWDC)](http://gizmodo.com/the-coolest-stuff-apple-announced-today-at-wwdc-2017-1795828823) 。



在那场 发布会上，苹果发布了“ [ARKit](https://developer.apple.com/arkit/) ”，这是一套新的免费软件工具，任何人都可以用它在 iPhone 和 iPad 上构建令人印象深刻的新应用和体验。“ARKit”中的“AR”指的是“增强现实”(augmented reality)，这是一种将交互式虚拟对象和效果置于你对现实世界的看法中的技术，将虚拟世界与物理现实融为一体。

今天，这通常是通过应用程序来实现的，这些应用程序使用智能手机(或其他设备)的摄像头向你展示你面前的真实世界，然后在其上放置虚拟物体。例如，现在最受欢迎的一些 AR 功能是 Snapchat 中的“镜头”或面部滤镜——这些效果会将动物的耳朵放在你的头上，或者以奇怪的方式扭曲你的脸。另一个是 Pokémon Go，这款游戏应用让口袋妖怪看起来好像在你的桌子或街道上蹦蹦跳跳。这些应用的共同点是，它们内部的虚拟物体似乎正在居住或改变现实世界的场景——“增强”我们的现实。

但这些应用程序是由专业软件开发商定制的。苹果 ARKit 版本的增强现实如此令人兴奋是因为它不是一个应用程序，而是一个 T2，任何人都可以免费构建新的增强现实应用程序，这些应用程序将能够在过去几年中的许多苹果 iOS 设备上运行。证据就在布丁中:苹果的 ARKit 仅仅公开发布了大约两个月，但已经有 [独立软件开发商](https://motherboard.vice.com/en_us/article/payq7g/developers-are-already-impressed-with-apples-augmented-reality-software) 为 iPhone 创造了一些看起来不可思议的体验——从你可以进入的 [虚拟门户](https://www.youtube.com/watch?v=rIPfpGCxONQ) 到将 [虚拟僵尸放在你的客厅](https://www.youtube.com/watch?v=zT54Xht9Opk) 等等。就连《指环王》的导演彼得·杰克森也拿《T21》这部阿尔吉特短片开了玩笑。

多年来我一直对增强现实感兴趣，所以当苹果宣布 ARKit 时，我激动不已。如果你有同样的感觉或者只是对自己尝试感兴趣，下面是你可以开始的方法。

## **检查以确保您有兼容的 iOS 设备**

ARKit 只运行包含 A9 处理器(或更新版本)的苹果 iOS 设备。根据 [雷德蒙派](http://www.redmondpie.com/ios-11-arkit-compatibility-check-if-your-device-is-compatible-with-apples-new-ar-platform/) 的说法，这限制了它对以下设备的使用:

*   iPhone 6s 和 6s Plus
*   iPhone 7 和 7 Plus
*   国际版
*   iPad Pro (9.7、10.5 或 12.9)
*   iPad (2017 年)

想必新的 iPhone 8 阵容也会支持 ARKit。你还需要确保你的 iOS 设备上的摄像头正在工作，因为 ARKit 依赖于它。您还需要一根电缆来将您的设备连接到 Mac 电脑。

## **在你的 iPhone 或 iPad 上下载 iOS 11**

一旦你手头有了这些兼容的 iOS 设备，你就需要在上面下载 iOS 11。这是苹果移动操作系统的最新版本，目前只有测试版，这意味着它可能包含漏洞，可能会破坏你设备上的一些东西。如果这是一个主要问题，购买或使用其他设备，而不是你的主要设备。或者，等 iOS 11 正式发布，预计也是 2017 年 9 月。

如果不想等，可以下载 iOS 11 测试版开始使用。要做到这一点，你需要注册苹果的测试软件项目。这是免费的，但是需要 20 分钟到几个小时来设置。 [把头伸过来，跟着指令](https://beta.apple.com/sp/betaprogram/) 。

## **检查以确保您有一台兼容的 Mac 电脑**

你还需要一台电脑来编写 ARKit 应用程序。具体来说，一台安装了免费操作系统[Mac OS Sierra 10 . 12 . 4](https://www.apple.com/macos/sierra/)(或更新版本)的 Mac。这意味着以下机器是合格的:

*   MacBook(2009 年末或更高版本)
*   MacBook Pro(2010 年年中或新款机型)
*   MacBook Air(2010 年末或新款机型)
*   MAC mini(2010 年年中或新款机型)
*   iMac(2009 年末或更高版本)
*   MAC Pro(2010 年年中或更高版本)

## **注册苹果开发者账户**

您可以使用免费或付费的开发人员帐户来开始使用 ARKit。如果你在 iPhone/iPad/Mac 上已经有了一个用于购买应用程序等的普通消费者 Apple 帐户，你可以将其升级为免费或付费的开发者帐户。在你的 Mac 电脑上使用网络浏览器，导航 [到苹果开发者账户登录页面](https://developer.apple.com/account/) ，选择适合你的选项。

## **从苹果开发者网站**免费下载适用于 Mac 的 Xcode 9(包含 ARKit)

在你的 Mac 上，登录你的苹果开发者账户，然后点击这里的 [点击右上角的](https://developer.apple.com/arkit/) 获得 Xcode 9，苹果的程序，用于编程(重言式，是的！).警告:您将需要至少 4.9 GB 的可用硬盘空间来下载此内容，然后 Xcode 本身会占用 9.76 GB 的硬盘空间。

## **启动 Xcode 9，用线缆将 iOS 设备连接到电脑**

在 Mac 上，通过连按 Xcode 9 下载来解压缩它，然后将 Xcode 应用程序拖到“应用程序”文件夹中，并连按它来启动它。插上你已经安装了 iOS 11 的 iOS 设备。

## **在 Xcode 中新建一个 AR app 项目模板**

在 Mac 上的 Xcode 中，点按“文件”、“新建”，然后选择“项目”这应该会弹出一个选项网格。点击“增强现实应用”

## **在 Xcode 中填写您的新 AR 应用的信息**

Apple 要求您为新的 AR 应用程序填写以下信息。你可以给它起任何你喜欢的名字，并且一定要选择一个“团队”，即使你是个人(如果你还没有团队，你可以选择创建一个。)保持其他一切检查。

在“语言”选项中，你也可以在苹果新的编程语言 Swift 和它的老语言 Objective-C 之间进行选择。两者都可以让你构建一个 AR 应用。如果你是编程新手，Swift 可能是更好的选择，因为它是苹果未来所有工具的计划。

最后，您可以选择您的“内容技术”，在 SceneKit、SpriteKit 和 Metal 之间进行选择。这些是用于显示图形的不同渲染引擎。这三个都可以让你构建 AR 应用，但提供不同的权衡，其中一些是这里描述的(基本上:SceneKit 用于 3D 图形，SpriteKit 用于 2D，Metal 用于更复杂的场景)。出于演示的目的，我选择了“SceneKit”

您还需要将您的项目放在计算机上的一个文件夹中。选择你想要的任何地方，这没多大关系。

## **选择您连接的 iOS 设备以接收您的新 AR 应用**

在 Mac 上的 Xcode 中，从顶部菜单栏中选择“窗口”，单击“设备和模拟器”，然后双击您的 iOS 设备。确保选中“显示为跑步目的地”复选框

你可能会在你的 iOS 设备上看到一个弹出窗口，上面写着“不受信任的开发者”，并给你一些指示，让你转到你的 iOS 设备的“设置”页面来允许该应用程序。

如果发生这种情况，请继续在您的 iOS 设备上找到您的“设置”应用程序，点击它，向下滚动到“通用”并点击它，然后进一步滚动到“配置文件和设备管理”，您应该可以找到您的苹果开发者电子邮件地址。点击这个，它应该允许你安装你的 ARapp。

## **运行你的第一个演示 AR 应用**

苹果公司提供了一个非常简单的 AR 演示，让你了解一下你可以用 ARKit 做什么。这个演示在你的设备的摄像头前显示一架战斗机在空中。

为了查看它的运行情况，首先确保在 Xcode 左上角的设备选择器下拉菜单中选择了您的 iOS 设备。

然后，在 Xcode 里抬头看顶部菜单栏。找到“产品”，点按它，然后点按“运行”

Xcode 顶部的状态指示器应该会随着活动和信息开始闪烁，然后它应该会在 iOS 设备上启动您的应用程序！

若要停止您的演示应用程序，请返回 Xcode 中的“产品”并向下滚动到“停止”

就这样，你正在使用 ARKit！关于添加你自己的新 3D 模型和创建动画体验的更多信息，我推荐以下指南:

*   [快速开始在 iPhone 或 iPad 上构建增强现实应用(杰森·奥多姆/移动 AR)](https://mobile-ar.reality.news/how-to/arkit-101-get-started-building-augmented-reality-application-iphone-ipad-quickly-0177989/)
*   [ARKit 教程在 Swift 4 for Xcode 9 中使用 SceneKit (Jameson Quave)](http://jamesonquave.com/blog/arkit-tutorial-in-swift-4-for-xcode-9-using-scenekit/)
*   [苹果 ARKit 增强现实 App 教程(Matthew h8/Instructables)](http://www.instructables.com/id/Apple-ArKit-Augmented-Reality-App/)