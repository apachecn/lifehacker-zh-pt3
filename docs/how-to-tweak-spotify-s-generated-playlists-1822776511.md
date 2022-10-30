# 如何调整 Spotify 生成的播放列表

> 原文：<https://lifehacker.com/how-to-tweak-spotify-s-generated-playlists-1822776511>

Spotify 的算法生成的播放列表在尝试，但它们并不总是命中目标。如果你想稍微改变一下食谱，可以试试 Spotify 播放列表生成器 [Nelson](https://nelson.glitch.me/) ，它可以让你根据你喜欢的音乐类型(或音乐元素)定制播放列表上显示的内容。

Watch

由 Spotify 开发者倡导工程师[Arielle Vaniderstine](https://twitter.com/imariari)创建的 [Nelson](https://nelson.glitch.me/) ，为你想听更多的内容提供了更细致的选择。你首先挑选五种你感兴趣的风格，然后调整对应于特定音乐元素的滑块(你可以在 0.0 到 1.0 之间调整参数)。然后:观看自定义播放列表在您眼前生成。当然，您可以将新生成的播放列表保存到您的 Spotify 帐户中。

### **滑块实际做什么**

如果你想知道每个设置如何影响出现在你的播放列表上的歌曲， [看看 Spotify 的文档](https://beta.developer.spotify.com/documentation/web-api/reference/tracks/get-audio-features/#audio-features-object) 描述了每个选项以及它如何与呈现的音乐相关联。这也凸显了你完全原创的和不一致的音乐品味是多么容易预测。例如，可跳舞性(根据 Spotify)是“...基于音乐元素的组合，包括速度、节奏稳定性、节拍强度和整体规律性。值 0.0 最不适合跳舞，1.0 最适合跳舞。想要词少的歌？降低“语音度”因子，它“检测轨道中是否存在口语单词”歌曲中的单词越多，其语音等级就越接近 1.0。

Spotify 已经在学习你以前播放的歌曲方面做了足够的工作，但对这十个参数进行调整，以及选择正确的流派列表，可能是你的家庭派对播放列表是成功还是失败的决定性因素。