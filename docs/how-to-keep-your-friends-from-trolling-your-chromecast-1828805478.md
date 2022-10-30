# 如何防止您的朋友窃取您的 Chromecast

> 原文：<https://lifehacker.com/how-to-keep-your-friends-from-trolling-your-chromecast-1828805478>

如果你拥有一台 Chromecast，并且有令人讨厌的朋友或室友，你可能厌倦了他们通过 [向你的设备](https://www.reddit.com/r/Chromecast/comments/1togo6/prevent_roommates_from_casting_porn_to_my_tv/) 传输愚蠢的视频来打断你的电影观看。Rickrolls 在第一次是有趣的，而不是第 26 次，尤其是当你投资于你最喜欢的节目或电影时。



Chromecast 使流媒体传输到联网电视变得容易，但这种对 T2 使用的便利也是该设备的致命弱点。任何与 Chromecast 连接到同一个无线网络的人都可以向它发送流媒体，不管你是否希望他们这样做。

虽然谷歌可以很容易地解决这个问题，如果它允许最后播放一段内容的人——甚至 Chromecast 的注册所有者——批准所有的流媒体请求，但它 [还没有提供这一功能](https://support.google.com/chromecastbuiltin/answer/6123915?hl=en) 。你可能不想有新的室友——朋友，*也许是*，但不是室友。

与此同时，你有两个主要的技巧可以用来防止别人干扰你的 Chromecast，它们都涉及到管理你的小流媒体 [棒](https://support.google.com/chromecast/answer/3046409?hl=en) 或 [球](https://store.google.com/us/product/chromecast_ultra?hl=en-US) 连接的网络。(这是对 [禁用 Cast media control notifications](https://support.google.com/chromecast/answer/7206638?hl=en)的补充，您应该这样做，这样当您开始流式传输时，其他人就不会试图打扰您了。)

### 为自己设置客人网络

如果你幸运的话，你的路由器可以广播一个“客人网络”给其他人使用。如果是这样，您可以通过两种不同的方式使用访客网络来保护您的 Chromecast。首先，给你的朋友和室友访客网络的密码，他们将无法访问你的有线或无线网络上的设备，除非你通过你的路由器设置明确允许他们访问(如果你可以的话)。

或者你可以把 Chromecast 放在你的访客网络上，永远不要分享访客网络的 wifi 密码。你必须连接到网络才能向 Chromecast 物理连接的任何设备播放媒体，这可能会有点烦人，但至少可以让 Chromecast 与其他 wifi 网络隔离开来。当你这么做的时候，你也可以将你所有的“智能”设备连接到你的访客网络，因为这是一个很好的安全实践来隔离你的家庭网络中不太安全的设备。

### 使用 VLAN 隔离您的设备

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-oo-hejIq3iQ&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-oo-hejIq3iQ&start=0) 

我在 [我的设置网络交换机](https://lifehacker.com/how-to-pick-the-right-network-switch-1828694436) 的指南中稍微提到了这一点，但是你也可以对 VLAN——虚拟局域网——感到有点疯狂，假设你的路由器或管理交换机支持该功能。简而言之，VLANs 允许您创建隔离的网络，并设置数据如何在它们之间传递的规则。

因此，举例来说，如果你运行你家的网络，你总是可以把你室友的以太网连接接到一个单独的 VLAN 上，并使用访问控制来防止他们与你的 VLAN 通话。他们将能够毫无问题地访问互联网，但他们无法干扰您的*VLAN 上的任何设备，包括您通过以太网连接到网络或通过无线接入点连接到网络的 Chromecast。*

与通过管理你的 wifi 来阻止访问你的 Chromecast 相比，VLAN 需要更多的设置 [和专业知识](https://www.megajason.com/2016/03/03/how-to-set-up-vlans-when-you-dont-understand-vlans/) ，但这可能是一个很好的解决方案，取决于你家的网络配置。