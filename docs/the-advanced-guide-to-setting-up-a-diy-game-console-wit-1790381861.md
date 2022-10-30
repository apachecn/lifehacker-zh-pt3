# 用树莓派设置 DIY 游戏机的高级指南

> 原文:[https://life hacker . com/the-advanced-guide-to-setting-a-DIY-game-console-wit-1790381861](https://lifehacker.com/the-advanced-guide-to-setting-up-a-diy-game-console-wit-1790381861)

众所周知，把一个 [树莓派变成一个复古游戏控制台](https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) 无疑是你可以用一个 Pi 做的最流行、最简单、最有趣的项目。这份最初的指南仅仅是个开始，如果你真的想从你的 DIY 小游戏中获得更多，你会想要深入了解一些高级技巧。

Watch

*这是我们的* [*设置指南的后续内容*](https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) *，因此我们将假设您已经启动并运行，复制了您的 rom，并设置了互联网访问。你还需要一个键盘来完成这些，或者你可以在一台台式电脑上使用*[*SSH*](https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md)*。如果您没有设置这些，请在继续之前查阅原始指南。*

### 更新至 RetroPie 的最新版本

首先，您需要确保安装了 RetroPie 的最新版本:

1.  启动安装了 RetroPie 的 Raspberry Pi，然后退出命令行(菜单>退出)。
2.  输入`sudo ~/RetroPie-Setup/retropie_setup.sh`并按回车键。
3.  这将加载安装脚本。选择“更新所有已安装的软件包”，然后按下 Enter 键。

让 RetroPie 做它的事情。如果你不是最新的，这可能需要 20-30 分钟。完成后，选择“执行重启”来重启系统。

### 为您的所有游戏添加插图

在你 [将你的 rom 添加到](https://github.com/retropie/retropie-setup/wiki/Transferring-Roms) 之后，你可以整理一个无聊的列表来挑选一个游戏来玩。这很好，但大多数人对盒子艺术的怀念就像他们对游戏本身的怀念一样。令人欣慰的是，用一种叫做“刮刀”的软件来添加艺术框非常容易。运行 scraper 后，这个乏味的旧列表现在包括了图片、发布日期等等。

有几种不同的方法可以将这些数据添加到您的追溯表中。第一个尝试的方法是内置刮刀。这要求您手动批准元数据。您可以从 RetroPie 本身访问此权限，只需确保您的 Raspberry Pi 连接到互联网:

1.  从主控制台选择屏幕，按下菜单按钮。
2.  选择刮刀。
3.  现在选择 Scape。
4.  如果你想为所有系统上的游戏收集插图，确保在系统下选择“全部”(或者更改为你想要的任何一个)，然后选择开始。
5.  每个游戏都会弹出一个提示，点击“A”接受结果。

现在，RetroPie 将收集更多关于你所有游戏的信息。取决于你有多少游戏，这可能需要一段时间，所以如果你有一吨，这是一个可怕的方式来勉强通过它们。相反，您会希望牺牲手动批准数据的能力，而让自动系统做出最佳猜测并为您转储所有数据。这样，scraper 扫描艺术品和其他数据，而不需要您批准每个条目。为此，您需要返回到您更新 RetroPie 的同一菜单:

1.  退出到命令行(菜单>退出)，键入:`sudo ~/RetroPie-Setup/retropie_setup.sh`并按回车键。
2.  向下滚动到配置/工具，然后按回车键。
3.  向下滚动到 Scraper 并按 Enter 键。这将安装 [史蒂芬塞尔夫的刮刀工具](https://github.com/sselph/scraper/releases) 。
4.  安装完成后，再次选择“Scraper”并按回车键。

等待刮刀工具完成。这可能需要一段时间，所以给它一些时间。

### 使用着色器获得更“精确”的图像

当你第一次在 RetroPie 中启动一些游戏时，你会注意到它们可能看起来过于清晰。这是因为现代的 LCD 屏幕比大多数老式游戏的老式 CRT 屏幕要清晰得多。 [着色器本质上是过滤器，用于校正这个更清晰的图像](https://lifehacker.com/add-crt-filters-to-game-emulators-for-a-more-realistic-5850124) 。他们添加扫描线，有点模糊，甚至模拟屏幕弯曲。

RetroPie 允许您在系统级别上设置着色器，或者使其与特定游戏一起工作。以下是如何为每个游戏设置着色器:

1.  在 RetroPie 开始任何游戏。
2.  在控制器上，同时轻按“选择”和“X”(或您映射到这些键的任何按钮)。这将弹出游戏内的菜单系统，看起来非常古老。
3.  选择“快速菜单>着色器>加载着色器预设”。
4.  在这里，你会发现一个*吨*不同的着色器，改变你的游戏外观。大多数人会对上图的着色器感到满意。如果你不是，尝试一下这里的选项，找到一个你喜欢的。完成后，用“A”按钮选择它，然后轻触“B”退出。
5.  选择“应用着色器更改”并按下“A”按钮。点击“B”退出菜单，选择“继续”返回游戏。

如果您不想对每个游戏都这样做，您可以配置一个着色器在所有模拟器中使用:

1.  退出到命令行(菜单>退出)，键入: `sudo nano /opt/retropie/configs/all/retroarch.cfg`并按回车键。
2.  用箭头键滚动文本文件，找到行`# video_shader_enable = false`并将其改为`video_shader_enable = true`
3.  将`# video_shader =`改为`video_shader = pathtotheshaderyouwanttouse`，例如`video_shader = /opt/retropie/emulators/retroarch/shader/crt-pi.glslp`
4.  按 Ctrl+X 保存并退出。继续并重启你的 Raspberry Pi 来确保效果被应用。

默认情况下，所有游戏都将使用该着色器，但您可以随时使用上述第一种方法为某些游戏手动更改它。

### 添加自定义主题和闪屏

自己制作游戏主机的部分吸引力在于定制。如果你不想使用 RetroPie 自带的默认主题，很容易就可以换成不同的主题。

首先，你必须手动添加主题到 RetroPie。有很多可供选择，你可以在 [RetroPie Wiki](https://github.com/RetroPie/RetroPie-Setup/wiki/themes) 上找到一个带有截图的列表。一旦您知道您想要哪个，您需要使用现在熟悉的 RetroPie 配置屏幕来添加它:

1.  在终端中，键入:`sudo ~/RetroPie-Setup/retropie_setup.sh`并按 Enter 键。
2.  选择配置/工具并按回车键。
3.  选择“审美”并按回车键。
4.  选择你想安装的主题，然后按回车键。
5.  回到终端，输入`emulationstation`并按回车键重启 RetroPie。
6.  轻按“菜单”按钮，然后选择“UI 设置”>“主题集”以选择您安装的主题。

如果你不喜欢任何预制的主题，你可以自己制作，但要做好大量工作的准备。如果你愿意走这条路，这本指南 会带你经历你需要的一切。

对于比完全自定义主题简单一点的东西，您可能还想更新启动时出现的闪屏。这很容易做到:

1.  创建一个您希望显示为闪屏的图像，然后将其从 PC 复制到`/home/pi/RetroPie/splashscreens`文件夹中。当您设置 RetroPie 时，此文件夹已自动共享，因此您应该能够从本地网络访问它。如果没有，回头参考我们的 [初始设置指南](https://lifehacker.com/how-to-turn-your-raspberry-pi-into-a-retro-game-console-498561192) 。
2.  在你的 Raspberry Pi 上，打开命令行并输入:`sudo ~/RetroPie-Setup/retropie_setup.sh`
3.  选择 Splashscreen 并按 Enter 键。
4.  选择选择闪屏并按回车键。
5.  选择您在第一步中复制的文件。

现在，当你启动你的 Raspberry Pi，它将显示自定义图像。如果你正在做一个复古游戏机作为礼物，或者你打算把它 [放在街机柜](https://lifehacker.com/build-your-own-two-player-bartop-arcade-machine-1655975529) 里，这就特别方便了。

### 为旧游戏设置成就

如果你真的喜欢在现代游戏中完成任务所获得的成就，你会很高兴知道你可以把它加入到老游戏中。RetroPie 使用 [RetroAchievements 系统](http://retroachievements.org/) ，适用于 NES、SNES、创世纪、游戏男孩、游戏男孩颜色和游戏男孩进阶。下面是设置它们的方法:

1.  [在](http://retroachievements.org/createaccount.php) 创建一个账户(在你的电脑上完成)。
2.  回到你的 Raspberry Pi，退出到命令行(菜单>退出)。
3.  输入`sudo nano /opt/retropie/configs/all/retroarch.cfg`并按回车键。
4.  在空行的任意位置键入以下内容，用您的追溯成就登录信息替换`yourusername`和`yourpassword`:

```
cheevos_username = “yourusername”
cheevos_password = “yourpassword”
cheevos_enable = true
```

完成后，按 Ctrl+X 保存并退出。

现在，你将在所有那些旧游戏中获得成就，就像你在现代游戏中一样。你可以在追踪你所完成的事情。

这样，你就可以真正定制你的 RetroPie 游戏机来满足你的需求了。当然，这是一个 Raspberry Pi 项目，所以即使是这个高级指南也只是触及了可能的表面。有可能，如果您能想到您想在 RetroPie 中更改的东西，只要您愿意深入研究一些配置文件，您可能就能做到。

山姆·伍利的图片。T3】