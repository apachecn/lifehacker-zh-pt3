# 在任何操作系统上安装 Android 的 ADB 和 Fastboot 工具的最简单方法

> 原文：<https://lifehacker.com/the-easiest-way-to-install-androids-adb-and-fastboot-to-1586992378>

如果你曾经尝试过 [root 你的安卓手机](https://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) 或者 [flash a ROM](http://lifehacker.com/how-to-flash-a-rom-to-your-android-phone-30885281) ，你可能听说过 ADB 和/或 fastboot。这两个工具惊人地强大，但是安装起来有点过于复杂。下面是简单的方法。



*更新:Google* [*最近发布了 ADB 和 fastboot 作为独立下载*](http://lifehacker.com/google-finally-lets-you-download-adb-and-fastboot-as-st-1790840830) *。现在你不需要下载一个巨大的开发者工具包来修改你的手机了！我们已经更新了下面的指南，以反映这些变化，并使用谷歌的官方下载，而不是第三方服务。*

### 什么是 ADB 和 Fastboot？

这两个工具允许你通过 USB 从你的电脑发送终端命令到你的手机。它们都提供不同的功能，但是它们可以相对容易地同时安装，所以两者都有帮助。下面是这些工具的(非常)简要的分类:

*   **Android Debug Bridge (ADB):** 这个工具允许你在任何时候向你的手机发送各种各样的终端命令——包括但不限于 [基本的 Linux shell 命令](http://lifehacker.com/how-can-i-quickly-learn-terminal-commands-1494082178) ，加上一些专业的开发者命令(只要你在手机上启用了调试)。您可以在手机开机启动时发送命令，甚至可以在手机处于恢复模式时发送命令。虽然 ADB 通常与寻根或修改手机结合使用，但您也可以使用 ADB 向未寻根的设备发送终端命令。
*   **Fastboot:** 当你需要修改手机固件时，Fastboot 就是你需要的工具。这允许你发送命令到引导装载程序，这意味着你可以刷新/修改像自定义恢复这样的东西。你不能用它来闪存整个 rom，但它对很多 ADB 做不到的事情很有帮助。并非所有手机都支持快速启动，因此您可能需要检查您的特定设备。

这两个工具都附带了 Android SDK，但是坦白地说，这是一个非常大的下载量，大多数对 ADB 和 fastboot 感兴趣的用户并不需要。幸运的是，谷歌最近让这两个没有所有垃圾的东西变得容易了。

### 步骤 1:下载平台工具包

Google 将 ADB、fastboot 和其他一些工具统称为平台工具包。这里 可以从 SDK 网站下载平台工具包 [。Windows、Mac 和 Linux 有单独的软件包，因此请下载适合您平台的版本。](https://developer.android.com/studio/releases/platform-tools.html#download)

下载完平台工具包后，提取。将文件压缩到一个文件夹中，您可以在以后找到它(比如“C:\Android\platform-tools”)。您实际上不需要安装 ADB 和 fastboot 来使用它们，但是您可以采取额外的步骤来使它们对您更方便。

默认情况下，你要么必须导航到你解压平台工具包的文件夹，然后从那里 [运行任何 ADB 或快速启动命令](http://lifehacker.com/the-most-useful-things-you-can-do-with-adb-and-fastboot-1590337225) ，要么写出每次你想运行命令时 ADB 所在的完整路径。例如，这是一个简单的命令，用于查看哪些设备连接到您的系统:

`adb devices`

但是，如果您的命令提示符没有打开到您提取平台工具的位置，您将必须键入如下内容:

`c:\Android\platform-tools\adb.exe devices`

每当你想调整手机上的某些东西时，都要经历这种痛苦。为了解决这个问题，我们可以修改路径变量，这样无论你在哪个文件夹，你都可以运行 ADB 和 fastboot 命令。

### 步骤 2:编辑路径变量

PATH 变量是查找命令行工具的主列表。默认情况下，你的电脑已经知道在哪里可以找到 [几个真正有用的工具](http://lifehacker.com/the-best-tools-hidden-in-windows-command-line-1553193077) 。这里，我们将把 ADB 和 fastboot 添加到列表中，以便将来更容易使用它们。您需要知道在最后一步中您将平台工具包解压到了哪里，所以请将该文件夹放在手边。

#### Windows 操作系统

根据您使用的 Windows 版本，这些步骤可能会略有不同。要将 ADB 添加到 PATH 变量中，请按照下列步骤操作:

1.  打开“开始”菜单，搜索“高级系统设置”
2.  点按“查看高级系统设置”
3.  单击标有“环境变量”的方框
4.  在“系统变量”下，点击名为“路径”的变量。
5.  单击“编辑...”
6.  (Windows 7，8):在“变量值”框的末尾添加`;[FOLDERNAME]`，用提取平台工具的文件夹路径替换【FOLDERNAME】。请确保在开头包含分号，以便 Windows 知道您正在添加新文件夹。
7.  (Windows 10):点击“新建”，粘贴提取平台工具的文件夹路径。按回车键，然后单击确定。

现在，当你想使用 ADB 或 fastboot 时，只需从“开始”菜单打开命令提示符并输入命令。

#### MacOS/Linux

编辑 macOS 和 Linux 路径文件比在 Windows 上稍微复杂一些。然而，如果你习惯使用命令行，它的 [还是相当简单的](http://hathaway.cc/post/69201163472/how-to-edit-your-path-environment-variables-on-mac) 。这种方法会在您每次登录系统时自动将 ADB 和 fastboot 的位置添加到您的路径中:

1.  通过导航到“应用程序/实用工具”或在 Spotlight 中搜索来打开终端窗口。
2.  输入以下命令打开 Bash 概要文件:`touch ~/.bash_profile; open ~/.bash_profile`

3.  的。bash_profile 文件应该在默认的文本程序中打开。
4.  将这一行添加到文件的末尾:export PATH = " $ HOME/[FOLDERNAME]/bin:$ PATH "将[FOLDERNAME]替换为您提取 ADB 和 fastboot 的位置。
5.  保存文件，然后按 Cmd+Q 退出文本编辑器。
6.  在您的终端中输入`source ~/.bash_profile`第一次运行您的 Bash 概要文件。

从现在开始，任何时候你打开一个终端窗口，你都可以从任何地方运行 ADB 和 fastboot 命令。