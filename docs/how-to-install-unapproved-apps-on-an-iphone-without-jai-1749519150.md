# 如何在不越狱的情况下在 iPhone 上安装未经批准的应用

> 原文：<https://lifehacker.com/how-to-install-unapproved-apps-on-an-iphone-without-jai-1749519150>

众所周知，苹果对商店中允许的应用程序非常挑剔，这意味着许多优秀的应用程序被拒之门外。 [越狱一直是获得未批准应用](http://lifehacker.com/how-to-jailbreak-your-iphone-the-always-up-to-date-gui-5771943) 的常用方法，但越狱可能是一件麻烦事。如果你只是想获得一两个非苹果批准的应用程序——像 [Kodi](http://kodi.wiki/view/IOS) ，视频游戏模拟器，甚至是[f . lux](https://justgetflux.com/)——像 [Gamma Thingy](https://github.com/thomasfinch/GammaThingy) ，侧面加载是一种方式。这个过程是免费的，很简单，只需要几分钟。



### 你需要什么

你不需要太多:

*   苹果电脑
*   [Xcode 7](https://itunes.apple.com/us/app/xcode/id497799835?mt=12) (免费)
*   [一个苹果 ID](https://appleid.apple.com/)T3】
*   iOS 设备

没有办法绕过 Mac 的要求，因为 Xcode 只适用于 OS X，不能在 Windows 上运行。

一旦你做好了所有准备，是时候决定你要安装哪个应用程序了。有两种不同的方法可以将应用程序下载到 iOS 上。第一种方法是获取一个为越狱手机制作的应用程序，将其转储到 Xcode 中，然后为你的手机重新构建它。第二种是从一个应用程序中获取源代码(通常是从类似 [GitHub](http://github.com) 的地方)，然后从头开始构建应用程序。在这里，我们将带你了解这两种方法，从一个为越狱手机开发的应用开始。如果您想使用源代码，直接跳到方法二。具体使用哪一种取决于你要构建的应用。如果你下载了一个 DEB 文件，这意味着它是为越狱手机制作的，所以用第一种方法。如果它是一个内部包含 XCODEPROJ 文件的 ZIP 文件，那么它就是源代码，所以使用方法二。

### 方法一:使用专为越狱手机设计的应用

我们将介绍的第一种方法是，将一个为越狱手机制作的应用程序加载到 Xcode 中，然后输出一个可以在非越狱设备上运行的文件。在这个例子中，我们将使用媒体中心应用程序 [Kodi](http://kodi.wiki/view/IOS) ，但是这个过程应该适用于其他应用程序。这是一种不支持的安装方法，使用未经验证的软件，因此您的里程会有所不同。所以，举例来说，Kodi 可以正常工作，但是像 [Winterboard](http://cydia.saurik.com/package/winterboard/) 就不行了。

#### 第一步:安装 Xcode

在您执行任何操作之前，您需要安装一份 Xcode 并使用您的 Apple ID 注册它。如果你想创建应用程序，你过去需要一个 99 美元的开发者账户，但如果你不打算在应用商店出售你的应用程序，那就不再需要了。

1.  [下载安装](https://itunes.apple.com/us/app/xcode/id497799835?mt=12) Xcode 7。
2.  打开 Xcode，点按“Xcode”>“偏好设置”,然后点按“帐户”面板中的+按钮。
3.  输入您的 Apple ID 详细信息。这将使您的 Apple ID 成为免费的开发者帐户。

现在 Xcode 已经设置好了，您可以继续了。

#### 第二步:建立你的项目文件

现在，您需要设置 Xcode 项目文件，以便可以将 Kodi 应用程序导入其中。

1.  下载 [Kodi DEB 文件](http://mirrors.kodi.tv/apt/ios/deb/) 。
2.  打开 Xcode 并选择“创建新 Xcode 项目”选项。然后选择单视图应用程序，并单击下一步。
3.  在“产品名称”下，在第一个框中键入应用程序的名称。
4.  在 organization identifier 下键入一个唯一的名称(使用类似 com.yourname.kodi 的名称)。
5.  确保为该语言设置了 Swift，并且在“开发目标”下设置了您的 iOS 版本
6.  一旦完成，您将看到一个感叹号和一个抱怨预置描述文件的注释。单击“修复问题”按钮。
7.  如有必要，请使用您的 Apple ID 登录。
8.  从下拉菜单中，选择您的开发团队(这通常只是您的名字)。

这部分到此为止。

#### 第三步:签署你的代码

对于像 Kodi 这样的应用程序，将它安装到你的设备上的最简单的方法是获取应用程序的越狱版本并“重新签名”。这需要额外的软件，但这是一个非常简单的过程。

1.  [下载 App 签名者](http://dantheman827.github.io/ios-app-signer/) 。这是一款开源软件，可以将 DEB 文件转换成 IPA 文件，这样 Xcode 就可以安装它了。它还会使用你用 Apple ID 创建的新开发团队来签名，这样你就可以在你的设备上使用它了。
2.  解压文件并打开应用签名。
3.  点击“浏览”按钮，选择你在第二步中下载的 DEB 文件。
4.  在签名证书选项下，单击下拉菜单并选择您的帐户。
5.  在 provisioning profile 下，单击下拉菜单并选择您的应用程序(在我们的示例中为 com.yourname.kodi)。
6.  单击开始按钮，选择一个输出文件名，然后等待 App Signer 完成它的工作。

您现在已经创建了一个签名的 IPA 文件，可以通过 Xcode 安装到您的设备上。

#### 第四步:安装你的应用程序

1.  返回 Xcode 并点按“窗口”>“设备”。
2.  在打开的窗口中，从左侧边栏中选择您的 iOS 设备，然后点按“已安装的应用程序”下的“+”按钮
3.  选择您在第四步中创建的文件，然后单击打开。

现在，应用程序将被发送到您的 iOS 设备。这可能需要一点时间，所以让它做它的事情。

#### 第五步:在你的 iOS 设备上认可自己

最后，第一次这样做时，你需要批准自己成为 iOS 设备上的开发人员(你只需要第一次这样做)。

1.  进入设置>通用>配置文件和设备管理。
2.  找到您的 Apple ID 帐户并选择“信任”。

就是这样！现在，您可以在 iOS 设备上打开您“创建”的所有应用程序。

### 方法 2:从源代码安装应用程序

将应用程序下载到 iOS 设备的第二种方法是从项目中获取源代码，在 Xcode 中打开，然后安装到您的设备上。你通常会在人们可以轻松托管自己代码的网站上找到这些项目，比如 [GitHub](http://github.com) 。对于这个例子，我们将使用 [Gamma Thingy](https://github.com/thomasfinch/GammaThingy) ，以及再现流行的屏幕调光软件效果的 app[f . lux](https://justgetflux.com/)。

#### 第一步:安装 Xcode

在您执行任何操作之前，您需要安装一份 Xcode 并使用您的 Apple ID 注册它。如果你想创建应用程序，你过去需要一个 99 美元的开发者账户，但如果你不打算在应用商店出售你的应用程序，那就不再需要了。

1.  [下载安装](https://itunes.apple.com/us/app/xcode/id497799835?mt=12) Xcode 7。
2.  打开 Xcode，点按“Xcode”>“偏好设置”,然后点按“帐户”面板中的+按钮。
3.  输入您的 Apple ID 详细信息。这将使您的 Apple ID 成为免费的开发者帐户。

现在 Xcode 已经设置好了，您可以继续了。

#### 第二步:找到你的源代码并创建一个项目

根据你想安装的应用程序，这个过程会略有不同，但在 Gamma Thingy 的情况下，它是托管在 GitHub 上的，所以下载它只需点击一下。

1.  前往 [Gamma Thingy 的 GitHub 页面](https://github.com/thomasfinch/GammaThingy) ，点击“下载 ZIP”按钮下载源代码。
2.  解压缩生成的归档文件，并在其中找到扩展名为 XCODEPROJ 的文件。
3.  双击以在 Xcode 中打开它。

Xcode 应该会打开，并载入正确的项目，准备好进行签名。

#### 第三步:签署你的代码

现在您需要构建项目并签署代码。这要求您对上一步中加载的项目文件进行一些更改。

1.  将您的 iOS 设备插入电脑并打开 Xcode。
2.  单击产品>目的位置>您的 iOS 设备。
3.  回到 Xcode 主屏幕，找到 Bundle Identifier 框，输入一个唯一的名称(比如 com.yourname.gammathingy)。
4.  从团队下拉菜单中选择您的 Apple ID。
5.  点按“修复问题”按钮，并使用您的 Apple ID 登录(如果需要)。
6.  将弹出一个窗口询问您的团队名称，从下拉菜单中选择您的开发团队(这通常只是您的名称)。

现在你只需要安装应用程序。

#### 第四步:安装应用程序

点按 Xcode 左上角的播放按钮，等待它编译并安装应用程序。如果没有任何错误，您基本上就完成了。**注:**就 Gamma Thingy 而言，我在 iPad 上编译时遇到了问题，但在 iPhone 上没有遇到。大多数人不会有这个问题，但如果你有， [这篇 Reddit 帖子详细介绍了如何修复它](https://www.reddit.com/r/jailbreak/comments/3sl58j/request_im_having_problem_with_gammathingy/cwybei0) 。

#### 第五步:在你的 iOS 设备上认可自己

最后，第一次这样做时，你需要批准自己成为 iOS 设备上的开发人员(你只需要第一次这样做)。

1.  进入设置>通用>配置文件和设备管理。
2.  找到您的 Apple ID 帐户并选择“信任”。

就这样，你现在可以打开你在 iOS 设备上创建的所有应用了。

<small>*插图由 fruit kujari 制成。*T3</small>

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=1737927710,5771943,1672952936&title=Climb%20Over%20the%20Walled%20Garden)