# 增强命令行功能的五个初学者工具

> 原文：<https://lifehacker.com/five-tools-for-beginners-that-power-up-the-command-line-1791515136>

无论您是经验丰富的老手还是命令行新手，您都不可能记住每个命令、手册页或工具提示。幸运的是，我们有一些工具可以让新手不那么害怕命令行，也可以帮助老用户记住在一些常见的情况下应该怎么做。

Watch

### 家酿使得在 Mac 上安装应用程序更加容易

Homebrew 是一个用于 Mac 的软件包安装程序，可以很容易地从命令行下载和安装应用程序。您还需要它来安装我们下面讨论的一些工具。

在 之前，我们已经讨论过使用 [家酿作为批量应用安装程序，所以我们不会在这里深入讨论，但基本思想是简化安装你需要的任何应用。键入一个命令，比如`brew install appname`，Homebrew 就会下载并安装它。](https://lifehacker.com/how-to-make-your-own-bulk-app-installer-for-os-x-1586252163)

有了家酿，你还可以使用一个名为 [家酿木桶](https://caskroom.github.io/) 的工具创建一个安装程序脚本，只需一个命令，它就可以在几分钟内将所有你喜欢的应用程序安装到一台新电脑上。

### Mac-Cli 和 Climate 简化了您最常用的命令

当你兴高采烈地记住一些需要 30 秒才能键入的复杂命令时，你会获得一定的声望，但我们大多数人都没有时间或毅力去做这件事。前面提到的、 [Mac-CLI](https://github.com/guarinogabriel/Mac-CLI) 和 [Climate](https://github.com/adtac/climate) 都是通过将一些最常见的命令转换成正常的人类语言来简化它们的工具。Climate 是为 Linux 做的，而 Mac-CLI 是为 Mac 做的。两者做的事情本质上是一样的，只是命令不同。气候需要`Climate`命令。Mac-CLI 需要使用`Mac`命令。

以下是我们在 Mac-CLI 中最喜欢的几个，让您了解如何使用它们:

*   `mac update`:安装软件更新、Ruby gems、自制更新、npm 更新等等。
*   `mac find`:最大文件:搜索并显示当前目录下最大的文件。
*   `mac system`:显示系统信息，查看性能。
*   `mac xcode:cleanup`:清理 Xcode 文件。
*   `mac git:branch`:显示所有 Git 分支
*   `mac dev:optimize-images`:针对网页优化当前目录中的所有图像。

Climate 的工作方式类似，但是使用了特定于 Linux 的工具:

*   `climate update`:更新你的气候安装。
*   `climate find biggest-files`:搜索并显示当前目录下最大的文件。
*   `climate overview`:显示我们系统的性能概述。
*   显示所有 Git 分支的列表。

这应该会让你对这里的情况有所了解。在 GitHub 的 [Mac-CLI](https://github.com/guarinogabriel/Mac-CLI) 和 [气候](https://github.com/adtac/climate) 页面查看所有命令的完整列表。两者的基本思想都是通过标准化命令来使命令行对初学者来说不那么可怕，但是对于那些不记得不经常使用的命令的有经验的用户来说，它真的很有用。Mac-CLI 不是你在这里唯一的选择 Mac， [m-cli](https://github.com/rgcr/m-cli) 基本上是一样的，但是不需要相同的第三方依赖。它不是一个非常健壮的工具包，但是如果你好奇的话，仍然值得一看。

### 用简单的英语说明欺骗最短的手册页

您通过在命令行键入`man`来访问的手册页通常非常长，长达数页。当您真的需要深入研究并弄清楚一些事情时，这是很有用的，但更多的时候，您只是在浏览手册页，以找到您可以运行的命令。 [骗子](https://github.com/chrisallenlane/cheat) 拿那些手册页，把它们缩小。

例如，如果你现在直接在命令行输入`man tar`，你会看到几页文档。《作弊》给了你一本更实用的手册。输入`cheat tar`，这就是你得到的结果:

> #要提取未压缩的归档文件:
> 
> tar -xvf /path/to/foo.tar
> 
> #要创建未压缩的归档文件:
> 
> tar-CVF/path/to/foo . tar/path/to/foo/
> 
> #要提取. gz 档案:
> 
> tar -xzvf /path/to/foo.tgz
> 
> #要创建. gz 归档文件:
> 
> tar-czvf/path/to/foo . tgz/path/to/foo/
> 
> #列出。广州档案:
> 
> tar -ztvf /path/to/foo.tgz
> 
> #要提取. bz2 归档文件:
> 
> tar -xjvf /path/to/foo.tgz
> 
> #要创建. bz2 归档文件:
> 
> tar-cjvf/path/to/foo . tgz/path/to/foo/
> 
> #要列出. bz2 归档文件的内容:
> 
> tar -jtvf /path/to/foo.tgz
> 
> #创建一个. gz 档案并排除所有 jpg、gif，...来自 tgz
> 
> tar czvf/path/to/foo . tgz—exclude = \ *。{jpg，gif，png，wmv，flv，tar.gz，zip} /path/to/foo/
> 
> #使用压缩算法的并行(多线程)实现:
> 
> 塔尔-z 我不知道-塔-伊普吉斯我不知道
> 
> 焦油 j...-> tar -Ipbzip2...
> 
> tar -J ... -> tar -Ipixz ...

这是更有用的信息，对吗？

作弊并不是这类工具中唯一的一种。如果出于某种原因你不是一个骗子的粉丝，看看和 [Bro Pages](http://bropages.org/) 。两者都与欺骗非常相似，但在如何向你展示信息方面采取了稍微不同的方法。

### Howdoi 搜寻常见问题的答案

虽然更短、更容易阅读的手册页可以帮助你找到大多数问题的根源，但它并不能帮助你解决所有问题。 [Howdoi](https://github.com/gleitz/howdoi) 是一个可以帮助完成其余工作的实用程序。

Howdoi 的结构就像一个问答系统。你问了一个关于如何运行一个命令的问题，doi 试图如何回答这个问题。让我们再来看一个例子。如果您在命令行中键入以下内容:

`Howdoi create tar archive`

你会得到一个小小的操作指南作为回应:

`Tar czf file.tar.gz file.txt`

Howdoi 并不完美，有时你不得不稍微欺骗一下你的措辞来得到你想要的答案，但它仍然比打开浏览器在谷歌上搜索答案要容易得多。还可以给 [阿尔弗雷德](http://blog.gleitzman.com/post/48539944559/howdoi-alfred-even-more-instant-answers)T3】或者T5】懈怠 加上 Howdoi。 

### 他妈的纠正你最后的控制台命令

[他妈的](https://github.com/nvbn/thefuck) 只做一件事:当你把上一个命令搞砸的时候，纠正它。因此，如果您键入了错误的命令，错过了必需的 sudo，或者忘记使用连字符，请键入`fuck`来更正该命令。虽然这并不总是对你犯的每一个错别字都有效，但他妈的在发现你的错误方面出奇的聪明。这里有一些你如何使用它例子:

*   `apt-get install vim`
    `fuck`
    T2】
*   `git brndh`
    `fuck`
    T2】

你明白了。你没必要盲目同意他妈的说什么。在命令运行之前，您需要确认正确的命令，这样您就不会意外地搞砸任何事情。如果你像我一样，你一直在命令行中输入错别字，所以他妈的是救命稻草。

有很多其他工具可以满足非常特殊的需求。 [牛逼 Shell](https://github.com/alebcay/awesome-shell) 是 GitHub 上的一个精选列表，有更多适合各种不同需求的内容。

山姆·伍利的插图。T3】