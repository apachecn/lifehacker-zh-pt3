# 如何检查您网络上的网络中立违规

> 原文：<https://lifehacker.com/how-to-check-for-net-neutrality-violations-on-your-netw-1822200634>

网络中立可能会在参议院 卷土重来，但同时你可能会有点担心你的互联网提供商会利用 [FCC 的宽松新规则](https://lifehacker.com/what-the-end-of-net-neutrality-means-for-you-1820647171#_ga=2.76946195.785031894.1516112040-1313785359.1499701416) 。要是有某种服务可以测试你的网络的节流和审查就好了。



事实证明，有几个不同的应用程序就是专门为此而设计的。最新的名为 [Wehe](http://dd.meddle.mobi/) 可以帮助显示哪些流媒体服务被你的互联网提供商减慢了速度。

你不会在 App Store 里找到 Wehe。最近被苹果拒绝的是 [，但是你还有一些选择。](https://motherboard.vice.com/en_us/article/j5vn9k/apple-blocking-net-neutrality-app-wehe)

### Wehe 如何工作(以及苹果为什么屏蔽它)

Wehe 背后的前提很简单。它可以测试七个流行应用程序(YouTube、亚马逊、NBCSports、网飞、Skype、Spotify 和 Vimeo)的流媒体速度，然后告诉你哪些应用程序被你的互联网提供商人为减慢了速度。利用这些信息，你可以向你的网络提供商投诉，或者向美国联邦贸易委员会提交一份正式报告。

现在安卓 已经有了 [版本，但是还不清楚你什么时候(如果有的话)能下载 iOS 版本。根据](https://play.google.com/store/apps/details?id=mobi.meddle.wehe&hl=en) [主板](https://motherboard.vice.com/en_us/article/j5vn9k/apple-blocking-net-neutrality-app-wehe) 的说法，苹果公司并没有对其决定做出太多解释，只是简单地告诉开发者它“对用户没有直接好处”。该公司没有透露更多细节，只是称之为“令人反感的内容”，这实际上是对任何被拒绝的内容的统称。

因此，如果你没有 Android 设备，你现在就不走运了，但谢天谢地，Wehe 不是这个类别中唯一的应用程序。还有一项服务存在的时间更长，已经可以在 iOS 上使用了。

### Ooniprobe 如何工作

OONI，代表网络干扰开放观测站，是 [Tor 项目](https://lifehacker.com/what-is-tor-and-should-i-use-it-1527891029) 的一部分。其 ooniprobe 应用最初于 2017 年初推出，目标是绘制全球在线审查的地图。然后，在 8 月份，该应用程序增加了一项新的测试，旨在找出违反网络中立的行为。

 [https://lifehacker.com/embed/inset/iframe?id=twitter-898484130333294594&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-898484130333294594&autosize=1) 

[DASH 流媒体测试](http://www.testyourinter.net/) 通过假装播放 30 秒的视频来检查网络质量。这将测量您的互联网的强度以及它如何处理未被识别的视频服务。Ooniprobe 在应用程序中显示这些信息，但它也将这些信息与来自世界各地的其他结果进行汇编，然后 [在网上发布其调查结果](https://api.ooni.io/) 。

Ooniprobe 还可以向你展示哪些网站被审查以及如何被审查。如果你正试图绕过办公室互联网的一个街区，或者你生活在一个政府正在切断重要网站访问的国家，这是非常有用的信息。

现在可以为 [iOS](https://itunes.apple.com/us/app/id1199566366) 和 [Android](https://play.google.com/store/apps/details?id=org.openobservatory.ooniprobe) 下载 ooniprobe。

### 可能的风险

关于政府审查的话题，OONI 指出，根据你在哪里，使用这个应用程序可能会有一些风险。任何监视你的互联网活动的人(比如你的互联网提供商、你的政府、你的老板，如果你在工作的话)都会知道你在使用这个应用。如果你的公司发现你在应该工作的时候试图访问被屏蔽的网站，可能会有大麻烦，在中国等互联网限制严格的国家做同样的事情可能会让你被罚款，甚至坐牢。

从积极的一面来看，OONI 说，目前还没有人因为使用这个应用程序而面临任何后果。至于 Wehe，它没有那么大的风险，因为你真的只是检查流媒体速度——它不像 ooniprobe 那样寻求更多的审查。尽管如此，如果你不想引起任何负面的注意，在工作中或在某些国家旅行时不使用这两个应用程序可能不是一个好主意。