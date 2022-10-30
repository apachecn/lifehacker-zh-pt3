# 如何使用支持 IFTTT 的路由器实现家居自动化

> 原文:[https://life hacker . com/how-to-automated-your-if TTT-supported-rou-1825956276](https://lifehacker.com/how-to-automate-your-home-with-your-ifttt-supported-rou-1825956276)

我热爱自动化；我知道。我只是觉得走进我的房子，让我的智能灯立即拉出一些丰富多彩的场景，这是有史以来最有趣的事情——更不用说当某些事情发生时，我可以创建所有荒谬的配置来改变它们的颜色和亮度，从“我收到了一条推特”到“都午夜了，你为什么还醒着去睡觉。”

Watch

在 Lifehacker 之前，我花了数年时间研究无线路由器，但直到最近我才有机会了解将一个路由器连接到 IFTTT 是什么感觉。而且现在有了，我想我也不想用一个*不能*的了。

### 虽然这不是有史以来最全面的服务，但它确实很有趣

如果你没有听说过 [IFTTT](https://ifttt.com/) (如果这个，那么那个)，这里有一个快速入门。在线工具允许您将不同的应用程序和服务相互连接。因此，如果其中一个发生了什么——例如，有人在推文中提到你——那么你可以触发另一个发生什么，比如打开连接到附近灯的智能开关。这是一个愚蠢的例子，但是 IFTTT 给了你很多触发和动作的可能性。

您可以使用设备的定位服务来触发硬件和服务，以便在您到达或离开家时执行操作，例如，当您到家时打开吊扇。我发现在连接或断开无线网络时触发这些操作更方便。

这是我的设置:我房间里有一堆飞利浦色调灯，我喜欢在回家时让它们切换到昏暗的设置，因为我懒得点击附近的色调水龙头(或者拿出手机手动触发一个场景)。虽然 Hue 的 iOS 应用程序可以在检测到你到达或离开某个特定的地理围栏时触发场景，但我家周围的虚拟圆圈并没有我想要的那么紧密。

每当我在我的 Hue 应用程序中使用基于位置的触发器时，我经常会发现我离开了我的房子——它会自动关闭我的灯——然后在附近的高速公路上开车经过时意外地触发了“打开”动作。看来，Hue 常常以为我进入了我看不见的“我在家”的泡沫。然后，不管出于什么原因，我的灯会一直亮着——也许当我快速进入和离开地理围栏时，Hue 有点头疼。

不管是什么原因，结果都很烦人:当我不在家的时候，我的灯会亮几个小时，这正是我在设置方便的“当你到达/离开”动作时试图避免的情况。

现在我正在玩一个谷歌 Wifi——它可以连接到 if TTT——我喜欢当某些设备连接或离开我的无线网络时，我可以触发动作。就我而言，现在当我的手机打开或关闭我的 wifi 时，我房间的灯就会打开或关闭。(我甚至在 IFTTT 应用程序中运行了一个小通知，让我知道这种情况何时发生，以保持诚实，并确保如果我不在城里，我的灯不会整个周末都亮着。)

也就是说，我还可以用触发器做更多的事情:发布“我回来了！”twitter 消息，当某些设备连接到我的 Google Wifi 时优先考虑它们，当一个设备连接时在我们的房子巢上设置特定的温度，每当另一个设备连接时播放附近 Android 设备上的歌曲，等等。有很多选项可供选择——其中很多很傻，但探索起来仍然很有趣。

### 你的路由器支持 IFTTT 吗？

我很幸运，因为让谷歌 Wifi 与 IFTTT 一起工作再容易不过了。其他厂商像[TP-Link](https://www.tp-link.com/us/support/ifttt-compatibility/)[华硕](https://www.asus.com/us/support/FAQ/1033394/)[Netgear](https://www.theverge.com/circuitbreaker/2017/11/16/16664824/netgear-disney-circle-routers)([sort-of](https://www.codeproject.com/Articles/1227757/Schedule-Internet-Access-for-Devices-in-Your-Home))都有一些支持 IFTTT 的路由器，但并不是每个路由器都有保障。不仅仅是怀疑你三年前的路由器是否会升级固件来支持这项服务，而且更新的路由器支持 IFTTT 是个例外，而不是常规。

这是一种耻辱。虽然这项服务并不完美——我仍然无法在每次进门时触发谷歌 Wifi 从我的谷歌主页上播放最后的倒计时——但它在家庭自动化的某些方面仍然很棒。虽然我有其他更强大的路由器，我*可以*设置来代替谷歌 Wifi(我对 AC1200 摇头)，但它们不支持 IFTTT，而且它太方便了，比定位更方便制定无线接入规则。

在一个完美的世界里，路由器制造商将允许你将每一个硬件产品与一个在线账户绑定，然后你可以使用这个在线账户和其他连接的服务，以新的令人兴奋的方式扩展你家的功能。

我们还没有到那一步——我希望我们有一天能达到那一步，尤其是随着网状网络越来越受欢迎。(从复杂的基于网络的路由器用户界面到易于使用的设置应用程序，感觉要花很长时间。)我就是想让我家每次回家都做傻事。这个要求很过分吗？