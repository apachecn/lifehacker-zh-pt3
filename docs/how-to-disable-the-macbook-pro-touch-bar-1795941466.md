# 如何禁用 MacBook Pro Touch Bar

> 原文：<https://lifehacker.com/how-to-disable-the-macbook-pro-touch-bar-1795941466>

自去年秋天以来，新的 MacBook Pro 型号已经用触摸条取代了功能键， [是键盘顶部的一个精巧的触摸感应显示器](https://gizmodo.com/the-macbook-pros-touch-bar-is-a-gimmick-thats-not-worth-1788931016) 。这需要一些时间来适应，你可能会发现自己摸索着删除键并调高耳机音量，或者无所事事地将手指放在退出键上并丢失你的工作。



OS X 的内置键盘设置让你可以定制 Touch Bar，这样你就可以删除键盘亮度等无意义的功能，并将其他功能移向中间，这样你就不太可能擦伤它们。但他们不会让你禁用退出键或整个触摸条。

为此你需要 [TouchBarDisabler](https://github.com/HiKay/TouchBarDisabler) ，这是一个 GitHub 项目，可以让你切换触摸条，并自动将亮度和音量控制重新分配给按键组合。

由于 Touch Bar Macs 没有真正的 escape 键，你也需要重新分配它。TouchBarDisabler 的创造者 HiKay 推荐使用 OS X 的键盘设置来 [分配 escape 功能给 caps lock 键](https://github.com/HiKay/TouchBarDisabler/issues/1) 。或者使用强大的键盘再映射器 [BetterTouchTool](https://www.boastr.net/) 将其分配给更方便的键，如~ `。所有这些重新映射可能会让人感觉很轻松，但擦过触摸栏并失去所有工作(或听力)也是如此。