# 五年来我摆弄树莓派的经验告诉我

> 原文:[https://life hacker . com/what-I-ve-learn-from-tamping-the-raspberry-pi-1793236686](https://lifehacker.com/what-i-ve-learned-from-tinkering-with-the-raspberry-pi-1793236686)

[Lifehacker's Complete Guide to Raspberry Pi](https://raspberrypiguide.kinja.com)) : title[![](../Images/051582a87daf38ca09cf7f704ce5f720.png)](https://raspberrypiguide.kinja.com)[Lifehacker's Complete Guide to Raspberry Pi](https://raspberrypiguide.kinja.com)Everyone wants a tiny little computer that can do it all, but how do you get started? Use this guide to master your brand-new Raspberry Pi.

今天是圆周率日，还有什么比回顾一下每个人最喜爱的 35 美元业余爱好者电脑树莓派更好的方式来庆祝每个人最喜爱的数学常数呢？自从树莓派发布以来，我已经写了大量的指南、博客和一本 [已经过时的书](https://www.amazon.com/Idiots-Guides-Raspberry-Thorin-Klosowski/dp/1615647783?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/what-i-ve-learned-from-tinkering-with-the-raspberry-pi-1793236686&asc_source=&tag=kinjalifehackerlink-20) 关于你可以用它做的各种项目。在那段时间里，我学到了很多。

Watch

### 故障排除是你必须练习的生活技能

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-wivyPH4AF1Q&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-wivyPH4AF1Q&start=0) 

我从为一些愚蠢的问题找到解决方案中获得的快乐是吸引我开始研究树莓派的主要原因之一。幸运的是，树莓 Pi 项目这些年来变得越来越容易了。以前制作一张 SD 卡需要的复杂过程，而现在的 [几乎是全自动的。尽管如此，树莓派还远没有像个人电脑或苹果电脑那样用户友好。那是功能，不是 bug。Raspberry Pi 旨在迫使您学习故障排除，这仍然是我最喜欢的事情之一。](https://lifehacker.com/the-always-up-to-date-guide-to-setting-up-your-raspberr-1781419054)

在业余爱好者迷上 Raspberry Pi 之前，它是一台主要面向儿童学习如何编码的计算机。从那以后，吸引力扩大了，但是一个项目仍然不可能跳出框框“工作”。你将不得不调整某些东西，钻研命令行，或者花几个小时在一个不知名的互联网论坛上寻找似乎只有你才有的问题的解决方案。你会把头往墙上撞，大喊一声，对你试图做的每个项目至少扔一次你的树莓派。

对于你完成的每一个项目，你消灭的每一个 bug，你纠正的每一个错别字，你的胃里都会有一种小小的、发光的感觉，这种感觉是值得你去努力的。故障排除是处理整个世界的一种方式，但是如果你不反复测试这些假设技能，你就会失去它们。

### Linux 很痛苦，但是值得学习如何使用它

在 Raspberry Pi 之前，我在 Linux 上的经历包括一次设置音乐服务器的失败尝试。现在，虽然我仍然没有兴趣每天使用它，但我对它的整体感觉很好。尽管使用起来还是很痛苦。

当我第一次开始开发 Raspberry Pi 时，除了使用命令行之外，我最大的障碍是试图了解何时以及何时不使用`sudo`命令。如果说我在 Windows PCs 上的成长岁月和后来在 Mac 上的岁月中学到了什么，那就是乱搞系统级文件、文件夹和权限设置肯定会毁掉你的电脑。我不得不打破这个思维过程，因为很多 T2 的树莓 Pi 项目需要超级用户访问。好消息是破解树莓派本身几乎是不可能的，尽管我已经破解了很多 SD 卡。

我仍然惊讶于你能用 Linux 做这么多事情。你可以让它屈从于你的意志，强迫它做你想做的任何事情。这包括将树莓派变成怪异的 [，微型点唱机](http://lifehacker.com/how-to-build-a-raspberry-pi-jukebox-any-non-geek-can-us-1712107103) ， [全网广告拦截器](http://lifehacker.com/create-a-network-wide-ad-blocker-with-a-raspberry-pi-1727295925#_ga=1.229622556.1646006925.1460757386) ，或者便携式黑客设备。这也意味着你可以经常复制大量的商业产品。 [亚马逊 Echo](http://lifehacker.com/how-to-build-your-own-amazon-echo-with-a-raspberry-pi-1787726931) 是这里最值得注意的例子，但是 [安全摄像头](http://lifehacker.com/the-raspberry-pi-zero-makes-a-great-motion-sensing-secu-1791167441)[天气显示器](http://lifehacker.com/build-a-raspberry-pi-powered-weather-forecast-display-1783350558) ，以及 [DIY 安全系统](http://lifehacker.com/everything-you-need-to-do-to-secure-your-raspberry-pi-h-1767083627) 也起作用。见鬼，我们甚至看到了新产品的创造，像 [科幻启发的智能镜子](http://lifehacker.com/this-raspberry-pi-powered-magic-mirror-can-be-set-up-wi-1791708352) 。要完成最复杂的 Raspberry Pi 项目，你需要至少了解一点 Linux、、T33、Python 、或者两者。在现代计算机时代，学习 Linux 的怪癖似乎是一种毫无意义的追求，但是我向你保证，最终这是值得的。

对我来说，从日常驱动的角度来看，Linux 的可扩展性一直是无用的，但在 Raspberry Pi 的情况下是有用的。Linux 让我可以把我最愚蠢的想法从一个白痴的计划变成一个半工作的项目，比如一个 [动画 GIF 相框](https://lifehacker.com/make-an-animated-gif-photo-frame-with-a-raspberry-pi-1658839211) 。那个愚蠢的相框仍然是我最喜欢的 Pi 项目，不管它值多少钱。

### 树莓派是一款很棒的游戏主机，但是当它不工作的时候会让人感觉怀旧

虽然我们都爱 [家庭自动化系统](http://lifehacker.com/build-an-entire-home-automation-system-with-a-raspberry-1640844965)[DIY 声控电脑](http://lifehacker.com/delight-or-horrify-your-friends-by-cramming-a-diy-alexa-1790526910) ，或者 [巧妙的便携式电脑设计](http://lifehacker.com/build-a-nintendo-ds-sized-portable-raspberry-pi-1767147400) 买树莓最流行的理由是把它变成 [复古的视频游戏机](https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) 。

我第一次尝试建造 Pi 驱动的仿真机器是在 2013 年 5 月的。正如我当时的大多数 Pi 项目一样，我的第一次尝试在等待了大约 13 个小时后失败了，因为一堆模拟器工具无法下载，然后破坏了我的 SD 卡。

一旦失败，我继续深入挖掘，直到我发现了超级任天堂 Pi ，它链接到一个名为 RetroPie 的全新项目。它 [当时还处于开发初期](http://blog.petrockblock.com/2013/02/10/retropie-project-image-download/) 。我为 Lifehacker 的第一版《Raspberry Pi 视频游戏机指南》 建立了这两套指令。RetroPie 是我发现的用 Raspberry Pi 构建仿真机器的最简单的工具，但是如果你想使用控制器，即使这样也需要你手动编辑文本文件。现在，这一过程非常简单，只需不到五分钟的时间就可以让整个系统启动并运行。

RetroPie 的简单性加上树莓 Pi 的开源、廉价特性意味着人们已经用这两者做了很酷的事情，像 [构建手持设备](http://lifehacker.com/build-a-truly-pocket-sized-video-game-console-with-a-ra-1775832832) 、 [控制台塞进控制器](http://lifehacker.com/cram-a-raspberry-pi-retro-console-inside-a-snes-control-1787227404) ，当然还有 [全尺寸街机机柜](http://www.iliketomakestuff.com/raspberry-pi-arcade-part-1/) 。

游戏仿真在树莓派之前就已经存在很久了。如果你是一个 30 多岁的人，几乎可以肯定你在人生的某个时刻下载了一些 SNES 模拟器和一个非法的超级马里奥世界副本来玩一个怀旧的游戏。对于所有年龄段的极客来说，至少尝试一次仿真就像是建造自己的计算机的成年礼。然而，尽管在 PC 和 Mac 上一直都可以使用仿真，Pi 却让这一切看起来更好。

这可能有明显的逻辑原因。树莓派售价 35 美元，即使有一个好的控制器和你需要的一切，你也可以用不到 80 美元来建造你的游戏主机。你甚至可以花 330 美元 买一套 [小桌面橱柜。我不认为低成本是唯一的吸引力。怀念旧游戏是一回事，怀念玩那些游戏的*体验*是另一回事。Raspberry Pi 不仅模拟了游戏本身，而且笨拙的设置过程更符合我在 20 世纪 80 年代和 90 年代设置游戏主机的记忆。对 child-Thorin 来说，一个控制台需要看起来像成千上万的电缆才能连接到电视上。即使在游戏机安装好之后，它们也不总是能工作。](http://www.retrobuiltgames.com/diy-kits-shop/mini-arcade-kits/porta-pi-arcade-10-hd/) [对墨盒吹气](http://gizmodo.com/anyone-else-blow-on-busted-hardware-like-its-an-nes-car-5849969) [可能什么都没做](http://mentalfloss.com/article/12589/did-blowing-nintendo-cartridges-really-help) ，但这是我们大多数人学到的第一个故障排除技巧。甚至在离开盒式磁带时代之后，我记得我不得不把我的 [PlayStation 倒过来，以便它能够读取光盘](https://en.wikipedia.org/wiki/PlayStation_(console)#Hardware_problems) 。似乎每一次控制台迭代，都有一些常见问题的荒谬修复。这个 [一直持续到今天](http://gizmodo.com/people-are-trying-to-fix-the-switchs-dumb-design-issues-1793020785) ，但是和以前不一样了。

对于孩子的大脑来说，旧游戏机的一切都显得笨拙而怪异，虽然树莓 Pi 没有重现任何这些故障诊断时刻，但它在创造自己的故障诊断时刻方面做得很好。每次 RetroPie 起作用时，它仍然感觉像一个小胜利。当你加载一个游戏时，那种胜利的感觉就像打开一个 PlayStation 来加载最终幻想 7 一样强烈。