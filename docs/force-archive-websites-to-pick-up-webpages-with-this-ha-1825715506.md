# 使用这个方便的工具强制归档网站抓取网页

> 原文：<https://lifehacker.com/force-archive-websites-to-pick-up-webpages-with-this-ha-1825715506>

当你需要查看旧版本的网站时，像 [互联网存档:时光倒流机](http://archive.org/web/) 这样的网站存档服务非常有用——无论是为了怀旧的还是因为你正在寻找已经被覆盖或删除的特定信息(例如，像你为前雇主写的故事)。



然而，这些服务并不完美。有时候，归档站点可能不会制作站点的快照—通常，正是在您最需要该快照的时候。或者可能有人配置了他们网站的 robots.txt 文件 [来阻止存档服务](https://splinternews.com/the-internet-archive-trashes-joy-reids-dubious-claim-th-1825506987#_ga=2.52269995.367633666.1525095724-3846207152.1521480874) 执行自动抓取。不好玩。

多亏了主板 的一个新工具 [，你现在可以尝试一次通过三个不同的存档服务来存档一个网站的当前版本:Wayback Machine、Archive.is 和 Perma.cc(如果你已经在他们那里设立了一个免费账户的话)。](https://github.com/motherboardgithub/mass_archive)

安装 Motherboard 的存档工具需要一点跑腿的工作，但这并不太棘手。你首先需要安装 Python 的 [请求](https://code.tutsplus.com/tutorials/using-the-requests-module-in-python--cms-28204) 、 [json](http://developer.rhino3d.com/guides/rhinopython/python-xml-json/) 和 [archiveis](https://github.com/pastpages/archiveis) 模块，这些都是主板的 mass_archive 工具工作所需要的。(唉，这不仅仅是您可以运行的一些简单的可执行文件或实用程序。)安装 requests 和 json 的最好方法是先安装 [pip](https://pip.pypa.io/en/stable/installing/) ，然后用它来下载模块。你会在这里找到 archive is，你也可以使用 pip 安装它。

你还需要从前面提到的 GitHub 项目 的 [中获取 mass_archive.py 脚本。一旦你准备好了，在 macOS 或 Linux 中打开一个终端，输入这个(显然，用你想要存档的网站代替 example.com):](https://github.com/motherboardgithub/mass_archive) 

`python mass_archive.py example.com`

如果你在 Windows 中通过 [提升命令提示符使用 Python，你可以](https://lifehacker.com/the-best-tools-hidden-in-windows-command-line-1553193077) [从代码中省略最初的“Python”](https://en.wikibooks.org/wiki/Python_Programming/Creating_Python_Programs)。