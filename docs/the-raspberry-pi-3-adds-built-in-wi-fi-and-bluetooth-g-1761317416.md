# 树莓 Pi 3 增加了内置 Wi-Fi 和蓝牙，速度提高了 50%

> 原文：<https://lifehacker.com/the-raspberry-pi-3-adds-built-in-wi-fi-and-bluetooth-g-1761317416>

众所周知，我们是树莓派 的忠实粉丝，今天又有一款新品上市。Raspberry Pi 3 采用了新的更快的处理器，但更重要的是，它最终在板上配备了 Wi-Fi 和蓝牙。它仍然只是 35 美元。



这里的大新闻真的来自树莓 Pi 3 上内置的 Wi-Fi 和蓝牙。以前，你需要花大约 10 美元购买一个 USB Wi-Fi 适配器，并在蓝牙加密狗上浪费宝贵的 USB 空间。现在，所有这些都是内置的，这意味着您不仅可以节省一点钱，还可以访问更多的 USB 端口。

另一个大消息来自减速带，它将 CPU 提升到 64 位 1.2 GHz 芯片(应该比 Pi 2 快 50%)和图形芯片的速度略有提高，现在是 400 MHz。

在花了一些时间实际操作 Raspberry Pi 3 之后，很明显速度提升是有用的，但不是完全革命性的。总而言之，在使用 Raspbian 时，Pi 3 感觉与 Pi 2 非常相似。然而，Raspbian 的更新版本也将于今天发布，这将提高兼容性。我们确实试着运行了一些基准，但是没有新版本的 Raspbian 来测试，它们不是特别可靠，所以我们需要稍后再来看看。

好消息是，Wi-Fi 和蓝牙几乎可以开箱即用，如果你启动 Raspbian 图形界面，设置两者就像在任何现代操作系统上一样。右键单击 Raspbian 右上角的 Wi-Fi 网络图标，然后输入您的网络信息。至于从命令行设置 Wi-Fi， [的工作方式和它一直使用的](https://www.raspberrypi.org/documentation/configuration/wireless/wireless-cli.md) 一样，但是你不再需要为那个适配器追踪驱动程序了。

Raspberry Pi 3 保留了 Raspberry Pi 2 的外形，因此您可能已经选择的任何情况都可以与最新版本配合使用。

与 Pi 的前几次迭代一样，您需要等待 Raspbian 之外的操作系统更新兼容性。这包括备受喜爱的 [RetroPie，它将你的 Pi 变成复古游戏机](http://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) 和 [Kodi](http://kodi.wiki/view/Raspberry_Pi) 。从历史上看，两者通常都会快速更新。像往常一样，如果您希望为 Pi 3 更新当前的 Raspbian 版本，您可以从命令行执行一些操作。只需在命令行中键入以下内容，然后点击 Enter:

```
sudo apt-get update && sudo apt-get upgrade
```

您的 Pi 现在将更新到新版 Raspbian，这意味着当它到来时，您可以将 microSD 卡交换到 Pi 3 中。

在 发布时，树莓 Pi 3 可以从 [通常的经销商列表中获得，随后会添加更多。希望它的](http://www.raspberrypi.org/products/) [不像圆周率 0 的](http://lifehacker.com/the-raspberry-pi-zero-is-a-5-computer-the-size-of-a-st-1744253282) 那样难以追踪。

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=5976912,5978871,498561192&title=Now What Am I Supposed to Do With It?)

* * *

<small>*联系作者在*</small>[<small></small>](mailto:thorin@lifehacker.com)*<small>*。*T15】</small>*