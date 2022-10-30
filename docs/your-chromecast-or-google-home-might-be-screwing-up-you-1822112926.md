# 你的 Chromecast 或 Google Home 可能会干扰你的无线网络[更新]

> 原文：<https://gizmodo.com/your-chromecast-or-google-home-might-be-screwing-up-you-1822112926>

据报道，谷歌主页和 Chromecast 设备正在扼杀人们的无线网络。这个问题， [首先由 Android Police](http://www.androidpolice.com/2018/01/14/google-home-max-appears-killing-wifi-networks/) 报告，最初似乎局限于 [Google Home Max](https://gizmodo.com/the-google-home-max-almost-made-my-house-go-boom-1821464329) 扬声器和廉价但通常很优秀的 TP-Link Archer C7 路由器的用户。然而，自从 Android Police 首次报告这个问题以来，它似乎已经蔓延到其他谷歌设备和 TP-Link 路由器。



TP-Link 很快就修复了最初的问题，如果你拥有 Archer C7 路由器，你应该用这个 [beta 固件](http://www.tp-link.com/us/faq-2050.html) 更新它。然后更多的投诉，与 Archer C7 路由器无关，甚至具体到 Google Home Max 音箱，开始在 [Google 产品论坛](https://productforums.google.com/forum/#!msg/googlehome/MmnsVnSxdQc/qBJF2KJ1AQAJ) 上弹出。

这是因为，虽然 Archer C7 特别容易受到影响，但这个问题似乎是整个谷歌 Cast 产品系列的通病。在 TP-Link 网站的博客中，一位 TP-Link 工程师解释了这个问题。

> 这个问题源于这些设备的“Cast”功能，它发送 MDNS 多播发现数据包，以便发现并保持与 Google Home 等 Google 产品的实时连接。这些数据包通常每隔 20 秒发送一次。然而，我们发现设备有时会在很短的时间内以非常高的速度广播大量的这些数据包。当设备从“睡眠”状态中被唤醒时会发生这种情况，并且可能超过 100，000 个数据包。您的设备处于“睡眠”状态的时间越长，该数据包突发就越大。这个问题可能最终导致路由器的一些主要功能关闭，包括无线连接。

本质上，谷歌设备正在从睡眠中醒来，然后一次向路由器发送太多的数据，导致它们崩溃。

谷歌已经 [告诉 9to 5 谷歌](https://9to5google.com/2018/01/15/google-chromecast-home-wifi-outage/) 它正在“快速工作以分享解决方案”然而，如果你在与家人互动或唤醒 Chromecast 时发现网络中断，你可以做一些事情。

最明显的一个方法是向您的路由器制造商咨询任何固件或 beta 固件更新并应用它们。你也可以重启路由器来清空内存，并在数据围攻后重新设置。此外，如果你想要一个非常简单的解决方案，你可以拔掉谷歌的违规设备，至少在路由器制造商和谷歌推出官方修复之前。

我们已经联系了谷歌，一旦得到长期解决方案的反馈，我们会及时更新。

* * *

**更新 1/17/18 11:52 东部**

谷歌 [针对该问题发布了一个新的支持页面](https://support.google.com/chromecast/answer/7634752) ，暗示该问题仅限于 Android 设备用户。

> “在同一个 Wi-Fi 网络上使用 Android 手机和 Chromecast 内置设备(如 Chromecast 或 Google Home 设备)的人可能会遇到这个问题。”

在同一页面上，谷歌表示将从明天 1 月 18 日开始对 Play Store 进行修复。它还建议“同时，尝试重启你的 Android 手机，并检查你的 Wi-Fi 路由器是否运行最新的固件版本。”

[ [安卓警察](http://www.androidpolice.com/2018/01/14/google-home-max-appears-killing-wifi-networks/) ，[9 to 5 谷歌](https://9to5google.com/2018/01/15/google-chromecast-home-wifi-outage/) ]