# 如何恢复 Chrome 的旧外观——并修复 Windows 上的模糊文本

> 原文:[https://life hacker . com/how-to-return-to-chromes-old-look-and-fix-the-fuzzy-te-1828828207](https://lifehacker.com/how-to-return-to-chromes-old-look-and-fix-the-blurry-te-1828828207)

谷歌在周二 推出了新版 Chrome 浏览器 [，其外观和感觉都有很大变化。正如任何这种规模的变化一样，并不是所有人都满意。事实上，对于切换浏览器，或者至少恢复到 Chrome 的旧外观，有相当多的抱怨。](https://lifehacker.com/the-best-new-features-to-try-in-chromes-latest-update-1828809071) 

Watch

如果你对新的 Chrome 有问题(或者只是不喜欢它的外观)，这里有一些让你的浏览器回到正轨的方法。

### 回到 Chrome“经典”

幸运的是，将 Chrome 的用户界面恢复到上周的样子其实非常容易。只需在地址栏中输入`chrome://flags`，进入切换 chrome 实验功能的页面，将“浏览器顶部 Chrome 的 UI 布局”设置从“默认”改为“正常”。一旦你点击应用并重启浏览器，Chrome 的标签页和搜索栏就会恢复原样。

需要明确的是，这并没有将 Chrome 完全恢复到 68 版。一些新功能，比如在搜索栏中寻找简单问题的答案，仍然有效。其他的，比如密码生成器，则没有。还值得指出的是，这只影响工具栏、选项卡和屏幕顶部的其他元素。“空白”标签页仍然具有新的圆形搜索栏。

### 但是为什么文字模糊不清？

不幸的是，并不是每个人的问题都是纯粹的美学问题。许多 Windows 7 和 10 用户报告称，“周年更新”使文本模糊，导致眼睛疲劳。

一些用户报告说所有的文本都很模糊，其他人说工具栏中的文本看起来很好，但是页面文本很模糊。Reddit 上的其他人报告说，只有当 Chrome 窗口最大化时，文本才会变得模糊。大多数报告指出，当您将文本大小设置为 125%时会出现问题，尽管关于缩小到 100%是否会有所帮助，存在相互矛盾的报告。

在谷歌的社区论坛和 Reddit 上，用户已经在进行临时修复。第一个也绝对是最简单的修复是摆弄你的窗口和文本缩放，看看改变是否有帮助。为此，请转到 Windows 系统设置中的显示器，选择标有“更改文本、应用程序和其他项目的大小”的滑块

如果这不起作用，用户报告说，在 Chrome 中添加一个启动参数会重新调整目标字段。在 Reddit 和 Google 的社区论坛上，这为每个尝试过并反馈的用户缓解了问题。下面是要做的事情:

要添加参数，右键单击 Google Chrome 应用程序或快捷方式，并从下拉列表中选择“属性”。在属性菜单中，选择“快捷方式”选项卡，并将以下字符串添加到“目标”框中文本的末尾:

**`/high-dpi-support=1 /force-device-scale-factor=1`**T3】

从那里，点击“应用”,你应该准备好了。

这只是权宜之计。鉴于投诉的数量，我预计谷歌会在不久后纠正这个问题，但这并不是伤害你眼睛的理由 Chrome 新标题栏上的包括你、 [灰色文本](https://chrome.google.com/webstore/detail/just-make-the-title-bar-t/jagdmopiaokbihcginhnafbgamlmgpgm) 。