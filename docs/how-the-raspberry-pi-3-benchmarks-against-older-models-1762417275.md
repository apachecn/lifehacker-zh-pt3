# Raspberry Pi 3 如何与旧型号进行对比

> 原文:[https://life hacker . com/how-the-raspberry-pi-3-benchmarks-against-older-models-1762417275](https://lifehacker.com/how-the-raspberry-pi-3-benchmarks-against-older-models-1762417275)

[树莓派 3 于本周发布](https://lifehacker.com/the-raspberry-pi-3-adds-built-in-wi-fi-and-bluetooth-g-1761317416) 虽然它的主要卖点是内置 Wi-Fi 和蓝牙，但它仍然有点慢。那么，让我们来看看它比 Pi 2 和 a Model B+快多少。

Watch

为了简单起见，我们决定坚持进行一些非常简单的测试，内存测试，CPU 测试，然后是引导时间。这里比较的所有 Raspberry Pi 型号都以正常速度运行，并且没有超频。因为这是你启动时注意到的第一件事，所以让我们先来看看启动时间。

毫不奇怪，树莓 Pi 2 和 Pi 3 的启动速度更快。树莓 Pi 比 Pi 2 快 3 英寸，快了大约 1 秒(17 秒对 18.4 秒)。这是一个小凸起，但仍然值得注意。我们来看看 CPU 减速带。

为了得到这些数字，我们运行 [SysBench](https://github.com/akopytov/sysbench) 来计算质数。这是对 CPU 的一个很好的全面测试，让我们对 Pi 的速度有一个大致的了解。Raspberry Pi 2 和 Pi 3 有四个核心处理器，所以我们使用一个核心和所有四个核心进行计算。B+只有一个内核，所以我们只能用一个来测试。从图中可以看出，Raspberry Pi 3 比单核的 B+快了近三倍，比 Pi 2 快了约 60%。当使用所有四个内核时，情况也是如此，其中 Pi 3 比 Pi 2 提升了 60%。

对我们大多数人来说，这可能在拉斯边最为明显。Pi 2 最终让 Raspbian 觉得可以作为一台真正的计算机使用，Pi 3 延续了这一趋势。这也意味着你*应该*能够在 Pi 3 上运行类似 [Playstation 模拟器的东西，而不需要超频。](https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192)

同样，我们在这里使用 SysBench。这一次，我们将测试内存工作负载。基本上，SysBench 分配一个内存缓冲区，然后测试读写速度。就百分比而言，Pi 3 远远超过了我们，但是我们在这里工作的时间很短，你可能不会真正注意到在真实世界测试中的差异。

当然，这是一个非常快速的纲要。还有很多其他基准可以测试其他因素。 [Hack 一天跑了一堆](http://hackaday.com/2016/03/01/pi-3-benchmarks-the-marketing-hype-is-true/) 显示类似的 3D 渲染、Python 等结果。基本上，在大多数测试中，Raspberry Pi 3 的基准测试速度比 Pi 2 快 40-60%。

* * *

<small>*联系作者在*</small>[<small></small>](mailto:thorin@lifehacker.com)*<small>*。*T15】</small>*