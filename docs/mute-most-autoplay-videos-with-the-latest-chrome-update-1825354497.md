# 使用最新的 Chrome 更新静音自动播放视频

> 原文：<https://lifehacker.com/mute-most-autoplay-videos-with-the-latest-chrome-update-1825354497>

Chrome 66 已经过时了，如果你是那种不在乎你的网络浏览器何时有新的更新的人，你可能要重新考虑这个版本的方法了。虽然你的浏览器会自动更新到 Chrome 66(技术上来说，是 66.0.3359.117)，但你应该现在就手动触发更新 以获得额外的安心。



虽然它最初计划在 Chrome 64 中首次亮相，但谷歌最终在 Chrome 66 中推出了预期的“自动静音”功能。我们的意思是，你的浏览器——一旦升级——会自动阻止网站未经你同意播放嘈杂、恼人的视频。你现在可以回去浏览网络上几乎所有的新闻网站，而不会觉得你必须关掉扬声器才能跟上当天的事件。

然而，对于 Chrome 的“沉默锥”,有一些警告。首先，Chrome 并没有屏蔽所有的自动播放视频。如果发布者默认将视频设为静音，它将会播放；如果不是，Chrome 只会在你试图浏览时阻止它发出噪音。如果一个出版商做了一件烦人的事情，他们把一个视频粘在你浏览器窗口的底部(或者网站的侧边栏)，你仍然会看到它。它会保持沉默，我们认为这总比什么都没有好

### 为什么视频还在播放？

Chrome *将*允许视频自动播放声音，如果浏览器已经确定你确实参与了该网站。如果你点击或轻敲网站域名内的任何地方，你将开始获得带声音的视频。借用 [谷歌的例子](https://developers.google.com/web/updates/2017/09/autoplay-policy-changes) :

> *“local news site . com 既有文字内容，也有视频内容。大多数人通过主页进入网站，然后点击新闻文章。由于用户与域的交互，新闻文章页面上的自动播放将被允许。不过，应该注意确保用户不会对自动播放内容感到惊讶。”*

如果你使用的是移动版 Chrome，在主屏幕上添加一个网站将允许它自动播放带声音的视频。如果你在桌面上浏览，谷歌还会使用 [(一种稍微复杂一点的算法](https://developers.google.com/web/updates/2017/09/autoplay-policy-changes) )来判断你是否与该网站进行了足够的互动，从而触发取消静音的自动播放:

> “[媒体参与指数]衡量个人在网站上消费媒体的倾向。Chrome 的 [*当前方法*](https://docs.google.com/document/d/1_278v_plodvgtXSgnEJ0yjZJLg14Ogf-ekAFNymAJoU/edit) *是每个原点的重要媒体播放事件的访问次数之比:媒体(音频/视频)的消费必须大于 7 秒；音频必须存在且未静音；* *标签页有视频被激活；视频的大小(以像素为单位)必须大于*[*200 x140*](https://chromium.googlesource.com/chromium/src/+/1c63b1b71d28851fc495fdee9a2c724ea148e827/chrome/browser/media/media_engagement_contents_observer.cc#38)*。*
> 
> 由此，Chrome 计算出媒体参与度得分，该得分在定期播放媒体的网站中最高。当它足够高时，媒体播放只允许在桌面上自动播放。"

您可以在此地址 查看您的媒体参与指数