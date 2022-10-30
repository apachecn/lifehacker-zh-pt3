# 跑步应用追踪你的距离有多准确？

> 原文：<https://lifehacker.com/how-accurately-do-running-apps-track-your-distance-1734172510>

大多数时候，我相信我的跑步应用。如果我开始跑 3 英里，回家时屏幕上只有 2.8 英里，我会绕着街区慢跑来完成这项工作。但即使是智能手机有时也可能是愚蠢的:就像 MapMyRun 在我朋友跑步的河对岸抓取数据点一样。

Watch

这两秒钟的想象游泳最终增加了应用程序对她跑步的估计距离。如此大的误差是罕见的，但是误差有各种形状和大小。如果你依靠一个应用程序来跟踪你的每周里程，或者在跑步或比赛中为你定速度，准确性就变得非常重要。

### 你的手机(或手表)如何知道你去了哪里

无论你是有一只像 Garmin 生产的 [那样的专用手表，还是使用像](http://explore.garmin.com/en-US/forerunner/) [Runkeeper](https://runkeeper.com/home) 或 [Endomondo](https://www.endomondo.com/) 这样的应用程序，位置数据的主要来源通常是被称为全球定位系统 或 GPS 的 [卫星群。](http://electronics.howstuffworks.com/gadgets/travel/gps.htm)

这些卫星随着时间广播它们的位置。如果你的设备可以接收来自四颗卫星的信号，它可以通过 [三边测量](https://en.wikipedia.org/wiki/Trilateration) 计算出你在太空中相对于那些卫星的位置。

然而，像地球大气层这样不方便的东西会改变信号的速度， [会引入一些误差](http://www.cmtinc.com/gpsbook/#chap6) 。但是你的设备能探测到的卫星信号越多，就有越多的数据来计算你的位置。如果有七个或更多，这个设备可以知道你在 10 米范围内的位置。

如果你有一个旧的 GPS 设备，你可能记得当设备是新的时候(或者每年春天从你的壁橱里把它挖出来之后)，你不得不永远站在那里等待一个位置锁。该设备正在下载 [历书](https://en.wikipedia.org/wiki/GPS_signals#Almanac) 的帧，这是卫星轨道和状态的列表。更新、更快的设备跳过历书，使用自己的处理能力来计算卫星的位置。

这是 GPS 背后的基本思想。还有其他卫星星座也有类似的功能，比如俄国的 [、GLONASS 的](http://beebom.com/2015/05/what-is-glonass-and-how-it-is-different-from-gps) ，它们的工作方式大致相同。Garmin 的一名代表告诉我们，他们的一些设备结合了 GPS、GLONASS 和 WAAS，即由额外卫星和地面站组成的 [广域增强系统](https://en.wikipedia.org/wiki/Wide_Area_Augmentation_System) 。

手机可以使用这些系统以及其他一些系统，包括 Wi-Fi 位置数据(如果你的设备可以看到某个星巴克热点，它就知道你在那家星巴克附近)和 [辅助 GPS](https://en.wikipedia.org/wiki/Assisted_GPS) ，它使用手机信号发射塔来跟踪 GPS 数据，这样设备就不必等待太久或努力搜索信号。

### GPS 到底有多精确？

有了所有这些系统，你的手机或手表可以知道你在 5-10 米内的位置。每隔几秒钟，它就会记录下你的位置，并通过连接这些点来计算你走了多远。

由于位置从来都不是完全准确的，所以把你的 GPS 信号想象成一只主要在你身边奔跑的狗可能会有所帮助。他是你的伙伴，所以他从不远离你；如果你知道狗走了多远，那也和你走的距离大致相同。

这是不准确的来源开始蔓延:如果你的狗是来回曲折，他会比你跑更多的总距离。但是每当你在十字路口转弯时，狗可能会抄近路，缩短距离。在发表在 *PLOS 一台*T5】上的一项 [研究中，GPS 设备*低估了*运动员在一条来回路径上跑的距离，而*高估了*他们在 200 米环中跑的距离——在每种情况下，误差各不相同，但都在 2-3%的范围内。另一个真实世界的测试](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0093693) [发表在*力量期刊&条件研究*](http://www.ncbi.nlm.nih.gov/pubmed/22990565) 上，发现误差通常在 6.2%以下——对他们的目的(测量总训练里程)来说很好，但你不能总是依靠它来区分 9 分钟和 10 分钟的一英里。

如果你在比赛中使用一种设备来测量你的速度，你还需要知道另一件事:由于跑道的测量方式，你可能会得到比比赛距离更长的读数。赛会官员测量最短可能不作弊距离，这意味着坚持在弯道内侧，不躲避其他参赛者——然后他们会额外增加 0.1%以确保安全。所以即使你的 GPS 那天完全在轨道上，读数稍长也是正常的。

随着时间的推移，软件和硬件的进步使得设备更加精确。Runkeeper 的数据分析师克里斯·德鲁因解释了为什么新手机可以给出更准确的结果，以及为什么不同手机的准确度不同:

> *   新型手机[片上系统]的设计可能会更好，以减少对 GPS 的可能干扰源。
> *   新手机通常有更多/更新/更好的传感器(包括更多更好的加速度计、陀螺仪、磁力计、计步器等)。可用作传感器融合解决方案的一部分)。
> *   *新手机倾向于支持新的手机操作系统，谷歌和苹果多年来在地理定位 API 方面都取得了稳步进展*
> 
> 也就是说，差异是双向的。新款手机和操作系统在电池使用方面也越来越积极。一般来说，这是一件好事——我们都喜欢更多的电池！-但如果手机在最后一圈进入省电模式，它可能会找到被跟踪活动的终点。

应用程序还可以将自己的逻辑应用到从硬件获得的数据点上，例如删除一个远离跑步者似乎正在行进的路径的读数，或者将突然的方向改变变成一个平滑的曲线。

### 如何获得最准确的读数

有两个地方你的 GPS 不能很好的工作:在建筑物中，和在树中:

*   建筑物(尤其是高层摩天大楼)会干扰卫星读数，因为信号会被建筑物反射。你的设备假设信号是以直线传播的，但是反弹增加了一段距离，这改变了它认为你所在的位置。建筑物也可以物理地阻挡信号；当设备有一个清晰的天空“视图”时，GPS 工作得最好。
*   树木覆盖也有同样的两个问题:它会阻碍卫星信号到达你的设备，从某种意义上说，树叶中的水分会为信号反弹提供一个表面。弹跳的幅度取决于你所在的森林有多厚，树木的种类以及一年中的时间。

Garmin 的代表告诉我，云和风暴不会明显影响 GPS 的精度。不过，如果你在一个平坦开阔的地方跑步，你的设备的精确度应该相当不错。

Douin 说，这使得农田听起来像是精确的理想场所，但如果你在一个没有很多手机信号塔的偏远地区，那就很难获得初始 GPS 锁定——并在设备最终确定你的位置时引起一次大的跳跃。他的观点:

> 如果你想用手机或其他 GPS 设备记录下最精确的跑步记录，我建议你找一条长的、相对直的路线，没有高大的障碍物……尤其是任何坚固的、直接在头顶上的东西(如桥梁或隧道)。

为了获得额外的准确性——尤其是如果你有时在室内跑步——许多设备都可以与脚架配合使用，比如 Garmin 的 [或 Nike](https://buy.garmin.com/en-US/US/shop-by-accessories/fitness-sensors/foot-pod/prod15516.html) 的 [这款脚架可以与他们的 iPhone 应用程序配合使用。你校准它，这样设备就能知道你的步幅有多长，并将其计算在内。](http://www.amazon.com/Nike-Stand-Alone-Sensor-Kit/dp/B001L6LJJS?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-accurately-do-running-apps-track-your-distance-1734172510&asc_source=&tag=kinjalifehackerlink-20) [基于加速度计](https://en.wikipedia.org/wiki/Accelerometer) 的 Garmin 设备有一个 [自定义步长功能](https://support.garmin.com/support/searchSupport/case.faces?caseId=%7B1a89a040-b2fb-11e4-6728-000000000000%7D) 代替，这是相同的想法，但没有脚 pod。

因此，如果你正在寻找 GPS 手表或手机的最佳读数，很可能会非常接近——但你仍然必须接受这样一个事实，即你永远不能指望你的设备在任何时候都完全准确。如果你在为自己的短距离计时(比如，你能跑四分之一英里，甚至一英里多快)，找到一条跑道或测量路径，然后 [学会阅读标记](http://vitals.lifehacker.com/how-to-add-speedwork-to-your-running-to-get-stronger-a-1695337461) 。如果你出于训练目的试图达到一个特定的配速，GPS 设备 [可以帮助](http://digitalcommons.wku.edu/cgi/viewcontent.cgi?article=1453&context=ijes) 但是你会想要有一个备用计划(即使那是“凭感觉跑”)，以防条件不完美。不过，对于测量长距离跑或简单跑，或者了解一周内你跑了多少英里，你的手机或手表就足够了。

*形象由* [*内曼贾*](http://www.shutterstock.com/pic-180218021/stock-vector-runner-with-jogging-gear.html?src=atKNuPSBY6tnebNlxZ865A-1-42)*(*[*Shutterstock*](http://shutterstock.com)*)。*

* * *

[](http://vitals.lifehacker.com/)**是来自 Lifehacker 的一个关于健康和健身的新博客。* [*关注我们这里的*](https://twitter.com/VitalsLH) *。**

*[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=1631241162,5732971,1527504722&title=If you're going to measure something, measure it right)*