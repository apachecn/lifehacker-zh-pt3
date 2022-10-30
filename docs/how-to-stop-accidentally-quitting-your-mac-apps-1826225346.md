# 如何停止意外退出您的 Mac 应用程序

> 原文：<https://lifehacker.com/how-to-stop-accidentally-quitting-your-mac-apps-1826225346>

这种情况每天至少发生一次，总是在我正在处理重要事情的时候:我不小心刷到了 Command+Q 组合键，而不是 Command+W 来关闭浏览器标签，让我退出了 Chrome。叹气。



虽然只是重新启动一个浏览器并回到浏览 [/r/aww](https://www.reddit.com/r/aww/) 并没有那么烦人，但在其他应用程序中不小心点击 Command+Q 会让你有点悲伤，特别是如果你有一段时间没有保存你的工作。值得庆幸的是，有一种方法可以防止你这样做，同时仍然保留 Command+Q 的有用性。(只有放弃者 [会将键盘命令](https://www.theinternetpatrol.com/how-to-stop-command-q-from-closing-your-apps/) 重新映射到其他东西。)

应用 [SlowQuitApps](https://github.com/dteoh/SlowQuitApps) 确实如其名。现在，你不再只是点击 Command+Q 来杀死一个程序，而是必须按住 Command+Q 一秒钟。一个小小的循环倒计时会在你的屏幕上弹出，一旦完成就关闭你的应用。就是这样。

虽然如果你想一次关闭一堆应用程序，这种延迟会有点烦人，但如果你没有因为过早关闭应用程序而意外删除过去一个小时一直在做的事情，你会更开心。哎呀。

而且，正如该工具的开发人员所指出的，你可以随时将“保持”时间调整为你想要的任何时间(以毫秒为单位)，你还可以将特定的应用程序列入白名单，这样一旦你按下 Command+Q，它们就会被关闭——不需要延迟。

如果你认为你会调整应用程序的设置，我建议通过 [家酿](https://lifehacker.com/five-tools-for-beginners-that-power-up-the-command-line-1791515136#_ga=2.39456355.1369191435.1526907270-1723114163.1524514905) 安装，这将使过程变得容易得多。如果你已经在酝酿了，只要打开终端，输入:

`$ brew tap dteoh/sqa`

`$ brew cask install slowquitapps`