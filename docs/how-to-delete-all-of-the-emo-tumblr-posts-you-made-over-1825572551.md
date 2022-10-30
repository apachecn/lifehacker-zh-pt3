# 如何删除你这些年来发表的所有 Emo Tumblr 帖子

> 原文:[https://life hacker . com/how-to-delete-all-of-the-emo-Tumblr-posts-you-made-over-1825572551](https://lifehacker.com/how-to-delete-all-of-the-emo-tumblr-posts-you-made-over-1825572551)

可能有一些原因让你想保留你的 [Tumblr](https://www.tumblr.com/) 账户，但删除你所有的帖子。也许你抢到了一个很棒的 Tumblr 用户名或网址，你不想 [放弃它](https://www.tumblr.com/account/delete) ，但是你宁愿人们不知道你在过去几年里对动画 gif 有多着迷，你对亨利·卡维尔的黑暗痴迷，或者你在朝九晚五的工作周中多久发布一次关于猫的帖子。诸如此类的事情。

Watch

Tumblr 提供了一个 [批量帖子编辑器](https://www.tumblr.com/mega-editor/) ，你可以使用它一次为一堆帖子添加或编辑标签，或者完全删除帖子。但是，如果你一直在翻滚(Tumblring？)在一段时间内，这将是一个艰巨的过程，因为在执行批量删除之前，你必须逐个点击每一篇文章。

不，点击一个帖子并按住 shift 键点击另一个帖子来快速选择一个群组是行不通的。不过，这是个好主意。

### 节省你(一些)时间的 Javascript 技巧

幸运的是，有一个小技巧可以让你一次选择 100 篇帖子，你可以继续重复这个过程——选择、删除、选择更多、删除更多等等——直到你永远清空了你的 Tumblr。是的，如果你有成千上万的帖子，这仍然需要一点时间，但至少比单独点击每一个要好得多。

正如 [路易李](http://louisrli.github.io/blog/2013/05/11/how-to-delete-all-tumblr-posts/#.Wt_GTMgvz-g) 所描述的，你首先要拉起 [群发帖子编辑](https://www.tumblr.com/mega-editor/) 。然后，将这段 Javascript 复制并粘贴到浏览器的地址栏:`javascript:$('.overlay').slice(0, 100).click()`

你可能不得不重新加入“javascript:”部分，因为大多数大型浏览器(如 Chrome、Edge 和 Firefox)都将这部分从你的复制粘贴工作中剥离出来。

这里有一个简单的方法:在浏览器的书签工具栏中创建一个书签，用整个 javascript 字符串作为 URL。这样，你只需点击书签来激活代码，而不必处理大量的复制和粘贴。

为了确保代码捕获尽可能多的帖子，请确保在大量帖子编辑器中继续向下滚动，以调出更多的旧帖子。一旦你觉得你已经达到了 100 左右，运行 Javascript，删除帖子，然后继续。我们建议你在删除的时候放一些舒缓的音乐——一旦你删除了，你就不太可能在你刚清理过的 Tumblr 上发布这些东西。