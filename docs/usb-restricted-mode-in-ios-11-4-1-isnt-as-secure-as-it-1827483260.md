# iOS 11.4.1 中的 USB 限制模式并不像看起来那么安全

> 原文:[https://life hacker . com/USB-restricted-mode-in-IOs-11-4-1-isn-as-secure-as-it-1827483260](https://lifehacker.com/usb-restricted-mode-in-ios-11-4-1-isnt-as-secure-as-it-1827483260)

“啊哈！”你心里想。“苹果终于让警察看不到我被没收的 iPhone 上有什么了。”

Watch

不完全是。

苹果今天发布了 iOS 11.4.1，你绝对应该去安装它，但有一个大警告，如果你还没有升级的话，iOS 11.4 可能会导致你的设备出现一些意想不到的电池问题 。这一相对较小的更新中的大变化是加入了苹果新的 USB 限制模式，据称这使得某人更难通过暴力手段进入你的设备，或利用任何其他巧妙的利用，通过 iPhone 或 iPad 的 Lightning 端口部署，来通过你的设备的密码。

一旦你安装了 iOS 11.4.1，USB 限制模式就会默认启用，尽管苹果把措辞弄得有点棘手。如果你打开设置应用程序，点击触控 ID 或(Face ID) &密码，验证，向下滚动，找到“ [USB 附件](https://support.apple.com/en-us/HT208857) ”选项，它就被禁用了。不过，这是你想要的。这意味着，在您的设备被锁定一个小时后，您的 iPhone 或 iPad 将不允许 USB 设备连接。

打开它，你就关闭了 USB 限制模式——任何物理连接的 USB 设备都可以访问你的手机。因此，当你被警察拦下并逮捕时，他们将能够使用 [他们奇特的工具](https://9to5mac.com/2018/03/15/this-is-the-graykey-box-used-by-law-enforcement-to-unlock-iphones-gallery/) 闯入你的设备。或者，更确切地说，正如苹果公司所说，USB 限制模式可以让你更安全地抵御黑客之类的攻击，因为这是该功能创建的原因。*嗯嗯*。

苹果的 [支持页面](https://support.apple.com/en-us/HT208857) 指出，你可能需要解锁你的 iPhone 或 iPad，以便连接的 USB 附件能够工作。这包括支持 iPhone 或 iPad 的配件:

> *从 iOS 11.4.1 开始，如果您在 iPhone、iPad 或 iPod touch 上使用 USB 配件，或者如果您将设备连接到 Mac 或 PC，您可能需要解锁设备，以便它识别和使用配件。然后，即使您的设备随后被锁定，您的配件仍保持连接。*
> 
> *如果您没有首先解锁受密码保护的 iOS 设备，或者在过去一小时内没有解锁并将其连接到 USB 配件，您的 iOS 设备将不会与配件或电脑通信，在某些情况下，它可能无法充电。您还可能会看到一个提示，要求您解锁设备以使用配件。*

苹果没有提到的是——我们想知道是否很快会有 iOS 11.4.2 来纠正这一点——显然在某些情况下绕过 USB 限制模式并不是那么困难。如果它在设备上启用，并且超过了一个小时的时间限制，第三方将无法连接一些神奇的设备并闯入你的 iPhone 或 iPad。然而，如果有人没收你的设备并插入正确的 USB 配件，他们实际上可以阻止这一个小时的倒计时发生。

正如 Elcomsoft 的 Oleg Afonin [对](https://blog.elcomsoft.com/2018/07/this-9-device-can-defeat-ios-usb-restricted-mode/) 的描述:

> 我们发现，即使有人将 iPhone 连接到一个不可信的 USB 配件，一个以前从未与 iPhone 配对过的配件(事实上配件根本不需要配对)，iOS 也会重置 USB 限制模式倒计时定时器。换句话说，一旦警察没收了 iPhone，他或她需要立即将该 iPhone 连接到兼容的 USB 附件，以防止一个小时后 USB 限制模式锁定。重要的是，这只有在 iPhone 仍未进入 USB 限制模式时才有帮助。

我们的建议？如果你不怀好意，而且马上就要被抓住，试着想出一个更有创意的方法来隐藏你智能手机的内容。或者，更好的是， [不要用你全新的 iPhone X](https://www.youtube.com/watch?v=OWV3k_d_y1k) 来经营你的犯罪集团。