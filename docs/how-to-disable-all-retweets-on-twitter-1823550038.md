# 如何禁用 Twitter 上的所有转发

> 原文:[https://life hacker . com/how-to-disable-all-retweets-on-Twitter-1823550038](https://lifehacker.com/how-to-disable-all-retweets-on-twitter-1823550038)

《大西洋月刊》刚刚为 [关闭你在 Twitter](https://www.theatlantic.com/magazine/archive/2018/04/the-case-against-retweets/554078/) 上关注的每个人的转发做了一个很好的案例，但他们没有告诉你如何做。所以我们做了一个工具来做这件事。

Watch

Twitter 允许你一次关闭一个用户的转发，但不是一次关闭所有用户的转发。手动关闭它们是一件痛苦的事情。因此，我们的同事迈克尔·赫茨伯格写了一个脚本，可以自动点击你关注的每个人的“关闭转发”。

## **如何**

1.  转到[https://twitter.com/following](https://twitter.com/following)，继续向下滚动，直到你加载完你关注的所有人。(如果你关注一千多人，这需要几分钟。)
2.  打开开发人员控制台。在 Chrome 中，那是视图>开发者>开发者工具。
3.  在开发人员控制台底部的命令行中，粘贴以下代码并按 enter 键。(同样，这可能需要几分钟时间，但您可以让它在后台运行。)

`a=Array.prototype.slice.call(document.querySelectorAll("div.ProfileCard-content div.dropdown"));a.forEach(function(e) {e.querySelector("button").click(); e.querySelector("li.retweet-off-text button").click(); })`

如果这个方法不能抓住每个用户，试着一次只做几个屏幕长度:加载“Following”页面，只向下滚动一点点，然后运行代码；向下滚动一两页，然后再次运行代码；诸如此类。你做这个的时候可能想放个播客。

每当你关注一个新的人，你仍然需要关闭转发。哈哈，对不起。但从好的方面来看，*你*仍然可以转发。

要颠倒这个过程，执行上面所有的操作，但是在代码中用`on`替换`off`(在短语`"li.retweet-off-text button"`内)。

## **为什么**

正如亚历克西斯·马德里加尔在《大西洋月刊》上所说，转发倾向于传播点击诱饵和愤怒。关掉它们，你可能会有一个更平静的饲料。你会错过很多笑话和政治更新，但也许这对你来说是值得的！这绝对是一种与默认截然不同的体验。

每当我们写到从 Twitter 上隐藏你不喜欢的东西时，总有人评论“过滤气泡”是的，如果你用推特来寻找不同的观点，那就打开消防水管。但是你不应该因为把你的推特信息限制在你真正选择关注的人身上而感到羞愧。没有人有义务阅读所有的推文。你甚至不需要看总统的推特；随便看看报纸或者博客。

## **可悲的是**

禁用转发不会禁用引用推文。经典推特！

它也没有隐藏那些“你关注的三个人喜欢这个陌生人的推文”推文，或者任何 Twitter 的其他烦恼。当然，它不会关闭推文的屏幕上限。对于一个真正安静的 feed，你只需要将那些引用太多的著名账户静音，并且不要关注那些频繁引用的 Twitter 账户。

如果还不够的话， [试着登出](https://lifehacker.com/how-to-disconnect-from-social-media-but-stay-connected-1822927183#_ga=2.75277521.2106951.1520269989-1297080755.1497980211) 。