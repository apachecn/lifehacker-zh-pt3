# 在整洁的浏览器中自动打开 YouTube 链接

> 原文:[https://life hacker . com/automatically-open-YouTube-links-in-an-uncomined-view-1825389630](https://lifehacker.com/automatically-open-youtube-links-in-an-uncluttered-view-1825389630)

如果你喜欢使用替代网站观看 YouTube 视频(像极简主义者，我们 [最近报道过](https://lifehacker.com/avoid-unexpected-youtube-bing-watching-sessions-with-tu-1825275041) ，或者*更多的*极简主义者 [Surprise.ly](http://surprise.ly/v/?RPS-Cq4uMFs) ，我们 [很久以前报道过](https://lifehacker.com/suprise-ly-shares-links-to-clutter-free-youtube-videos-1513284946) ，那么你可以设置一个 Chrome 扩展来在你每次点击 YouTube 链接时重定向你。

Watch

要将 YouTube 视频重定向到 Tube，安装 [重定向器](https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd?hl=en) Chrome 扩展。从 Chrome 工具栏打开扩展，点击“创建新的重定向”，像这样填写:

```
Description: YouTube to Tube
Example URL: [https://www.youtube.com/watch?v=1234](https://www.youtube.com/watch?v=1234)
Include pattern: [https://www.youtube.com/watch?v=*](https://www.youtube.com/watch?v=*)
Redirect to: [https://tube.quinzel.tech/watch?v=$1](https://tube.quinzel.tech/watch?v=$1)
Pattern type: Wildcard
```

(1234 只是占位符；您可以在那里键入不同的随机字符串。*是通配符，$1 表示您希望保留原始 URL 中的视频 ID。)

点击保存，你就完成了。

你可以用 [Surprise.ly](http://surprise.ly/v/?RPS-Cq4uMFs) 或任何其他 YouTube 查看器设置类似的重定向。当然，您可以使用这个扩展将任何类型的 URL 重定向到任何其他类型的 URL。

如果你不喜欢处理通配符和变量，试试 [Requestly](https://chrome.google.com/webstore/detail/requestly-redirect-url-mo/mdnleldcmiljblolnjhpnblkcekpdkpa) 来代替，它让你只命名你总是想改变的 URL 的一部分，而不需要通配符。