# 使用 Chocolatey GUI 一次安装和更新所有 Windows 应用程序

> 原文：<https://lifehacker.com/install-and-update-all-your-windows-apps-at-once-with-t-1827588626>

**Windows:** “软件包管理器”这个词听起来有点不祥，但是如果你聪明的话，你已经用它给你的 Windows PC 配备了所有的基本功能: [尼尼特](https://ninite.com/) 。这个网站再简单不过了。你选择你想要的程序，它为所有的东西创建一个安装文件，双击它立刻安装你选择的所有东西。



之后，你就靠自己了。

如果你想要另一只手来确保你最喜欢的应用程序保持更新——或者从一个更大的用户维护包(应用程序)目录中挑选——考虑巧克力 。不，不是美味的糖果，也不是基于命令行的应用程序安装程序。好吧。算是吧。 [Chocolatey GUI](https://chocolatey.org/packages/ChocolateyGUI) 是你想要检查的，因为它为你提供了一个可爱的图形界面来安装和管理你的应用程序，这比大量的命令行输入更容易处理。

在 之前，我们已经 [介绍过巧克力，但距离我们谈论它(或有用的 GUI 附加组件)已经有一段时间了。这里有一个如何开始的快速复习。首先，点击 Windows 中的开始按钮，输入“命令”当命令提示符出现在您的结果中时，右键单击它并选择“以管理员身份运行”然后，复制](https://lifehacker.com/chocolatey-brings-lightning-quick-linux-style-package-5942417) [这段文字](https://chocolatey.org/install) ，粘贴到命令提示符下，按回车键。

一旦你这样做，巧克力将开始安装自己。不需要很长时间。当一串文本滚动过去，Chocolatey 显示完成时，键入以下内容并按 Enter:

`choco install chocolateygui`

将会出现更多的文本，并且会提示您在某一点上点击“y”来确认您想要继续安装。一旦 Chocolatey GUI 完成安装，您的屏幕应该看起来像这样:

然后，您可以在 Windows 开始菜单中查找新安装的程序，调出 Chocolatey GUI。当它加载时，你会看到所有你已经安装在你的电脑上的应用程序(通过 Chocolately 图形用户界面，所以，只是...巧克力状 GUI)。要查看还有什么，点击左侧边栏的“chocolatey”。为了让一切看起来更漂亮，点击右上角的图标，它看起来像一个由四个窗口组成的网格:

默认情况下，您看到的应用程序按受欢迎程度排序。双击任何东西来查看它的描述，或者右键单击来弹出一个菜单，在那里你可以开始安装你熟悉的应用程序。你应该能够“重新安装”你系统上已经有的应用程序，而不会搞砸任何事情。当你这样做时，或者当你通过 Chocolatey GUI 安装新应用时，它们将出现在你的“这台电脑”列表中。您还可以查看您的应用程序是否有任何新的可用版本，并进行相应的更新，只需轻轻一点。