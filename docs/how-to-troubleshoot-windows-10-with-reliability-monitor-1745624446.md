# 如何使用可靠性监视器排除 Windows 10 故障

> 原文:[https://life hacker . com/how-to-trouble shooting-windows-10-with-reliability-monitor-1745624446](https://lifehacker.com/how-to-troubleshoot-windows-10-with-reliability-monitor-1745624446)

解决 Windows 中的问题可能是一种痛苦，但内置的可靠性监视器通过在一个简单的视图中显示计算机的可靠性和问题历史来帮助您。

Watch

可靠性监视器是那些很少有人知道或费心的 [令人敬畏的 Windows 功能](http://lifehacker.com/7-awesome-features-youve-forgotten-about-in-windows-7-5932456?trending_test_two_e&utm_expid=66866090-68.hhyw_lmCRuCTCg0I2RHHtw.4&utm_referrer=https%3A%2F%2Fwww.google.com%2F) 之一。但是它非常有用。Windows 会自动跟踪应用程序和系统故障，尽管使用古老的事件查看器可以看到相同的信息，但可靠性监视器会以易于浏览的基于时间的视图显示这些故障。

### 如何读取可靠性历史记录

要启动可靠性监视器，请单击“开始”，键入“可靠性”，然后选择“查看可靠性历史记录”。你首先看到的是一张图表，显示了你的电脑在过去两周左右的可靠性历史。您可以使用左右箭头在时间上向后或向前滚动图表，并且可以按周而不是按天查看图表。这个图表中有很多东西，所以首先让我们把它分解一下。

顶部是一个线形图，表示系统稳定性指数(SSI)。那只是一个从 1(不可靠)到 10(非常可靠)的数字，而且是基于你遇到的问题数量。第一次安装 Windows 时，SSI 从 10 开始。每次报告一个问题，它就会下降，然后随着时间的推移逐渐回升，直到报告另一个问题。在我的截图中，您可以看到该图从大约 5 开始，通常会攀升，但每次红色 X 表示应用程序失败时都会出现下降。

在图表下方，您将看到特定类型问题的行:应用程序、窗口和其他故障，以及系统警告和信息。通常，在进行故障诊断时，您需要注意的是应用程序和 Windows 警告。

### 向下钻取特定问题

您将看到的许多故障是一种自我修复，即使在运行良好的系统上，您也会看到它们不时地出现。甚至一个“关键”事件也可能只是一个失败(或启动失败)的重要服务，然后能够在以后启动。

如果您正在对您遇到的特定问题进行故障诊断，您会想要查找问题群、重复出现的问题或在您注意到电脑有问题的特定时间发生的问题。

单击图表中的特定日期，查看当天发生的问题列表。您也可以单击窗口底部的“查看所有问题报告”链接，在一个方便的列表中查看所有问题报告。

对于每个问题，您将看到一个摘要以及问题发生的确切日期和时间。如果在 Windows 中启用了错误报告，某些问题还会在“操作”列中有一个解决方案链接的复选标记。让 Windows 检查一下不会有什么坏处，但是很少成功。如果打开了错误报告，通常会在发现问题时应用解决方案，因此不太可能在可靠性监视器中显示出来。如果可检查的解决方案没有问题，您将看到一个查看技术细节链接。

大多数细节对你来说没什么意义，但有几个通常可以帮助你找到解决方案:

*   **出错应用程序名称。**这将显示失败的服务或应用程序的名称。
*   **异常代码**。异常代码有时也称为停止错误或停止代码，是识别问题或事件的十六进制数字。

这两个细节在追踪和解决问题时都非常有用。尝试将出错的应用程序名称(不包括版本和时间戳信息)和异常代码插入到 Google 或 Microsoft 支持搜索中，您很可能会找到针对您所面临的任何问题的解释(希望附有解决方案)。

偶尔检查一下可靠性监视器可以让您很好地了解系统中正在发生的事情，而不必让您的大脑陷入像事件查看器这样的工具和它提供的所有无关的细节中。希望它能帮助你更容易地找到一些重复出现的或停止播放的问题。

如果您遇到了无法解决的问题，您还可以将您的可靠性历史记录保存为 XML 文件，然后展示给可能会提供帮助的人。