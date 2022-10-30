# 如何在你的台式机或笔记本电脑上隐藏 Gmail 的“智能回复”

> 原文：<https://lifehacker.com/how-to-hide-gmails-smart-replies-on-your-desktop-or-lap-1829195425>

Gmail 的智能回复功能现已整合到该服务针对桌面客户端的最新设计更新中，当你不想打出一个真正的回复时，这是一个发送简洁回复的好方法。当然，它们可能会惹恼收件人；你甚至可能会点击错误的回复，无意中告诉你的老板“ [爱它！当他或她要求你这个周末加班时。但是它们不是很方便吗？](https://www.wsj.com/articles/very-interesting-awesome-love-it-gmail-users-confront-chipper-smart-reply-1537282569)



如果你不喜欢智能回复——以至于你等不及谷歌让你在桌面上完全删除——你可以用这个小技巧永远隐藏它们。

首先为你的浏览器下载 Ublock Origin([Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=en)， [Firefox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) ， [Safari](https://github.com/el1t/uBlock-Safari) ， [Edge](https://www.microsoft.com/en-us/p/ublock-origin/9nblggh444l4#activetab=pivot:overviewtab) )。我们会等的。安装好后，拉起 [Gmail](http://www.gmail.com) 。确保 Gmail 的 Ublock Origin 已打开(浏览器工具栏中的图标应该是红色的，而不是灰色的)，然后点击收件箱中的邮件，直到看到一个弹出 Gmail 智能回复功能的邮件。它看起来会像这样:

在最后一个智能回复的右侧轻轻单击鼠标右键，然后选择出现在上下文菜单中的“阻止元素”选项。它看起来会像这样:

当你这样做时，一个大的红色覆盖应该出现，包含智能回复。如果没有，请单击突出显示的内容，然后将鼠标悬停在智能回复上，直到您看到类似这样的内容(然后单击以锁定您的选择):

一旦你被锁定(你的鼠标光标应该是一个有一条线穿过的圆圈)，向右移动光标，直到它激活 UBlock Origin 的灰色覆盖——因为没有更好的方法来描述它:

点击“创建”设置新的过滤规则，然后在浏览器中刷新 Gmail。您应该不会再在任何邮件上看到智能回复。如果，无论什么原因，你错过了它们，只需调出 Ublock Origin 的选项(通常通过右键单击浏览器工具栏中的 Ublock Origin 图标)并访问“我的过滤器”选项卡。删除“mail.google.com”条目，点击应用更改，您的智能回复应该会返回。