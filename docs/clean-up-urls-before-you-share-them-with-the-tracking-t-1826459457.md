# 在与“跟踪令牌剥离器”扩展共享 URL 之前，请清理它们

> 原文：<https://lifehacker.com/clean-up-urls-before-you-share-them-with-the-tracking-t-1826459457>

有多少次你去和朋友分享一个有趣的故事(或漫画)——这是一个非常标准的过程——却发现你以为你在复制和粘贴的短网址实际上是一个巨大的、混乱的文本段落。你可以感谢所有的服务和网站，它们在网址上附加了大量的垃圾信息，这样它们就可以更好地了解你是如何访问这个网站的，你浏览了什么，你要去哪里。

Watch

作为斯坦福大学的前商业经理，我明白。网络跟踪很重要，因为它允许网站以一种令人愉快和引人注目的方式优化内容。(谁不想看看他们的内容有多吸引人，或者网站设计或特色项目的小小调整能对如此美妙的广告收入产生多大影响呢？)

尽管如此，没有人喜欢看起来像帕特里克·罗斯富斯小说的网址。虽然突出显示和删除 URL 中你不想要的部分很容易，但这可能是一个费时的过程，有点反复试验的味道。删除太多，链接可能不起作用。

或者你可以只为 [Chrome](https://chrome.google.com/webstore/detail/tracking-token-stripper/kcpnkledgcbobhkgimpbmejgockkplob?hl=en) 或 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/utm-tracking-token-stripper/) 安装跟踪令牌剥离器(也可以在 GitHub [这里查看](https://github.com/jparise/chrome-utm-stripper) )。一旦您启动并运行了扩展，您所要做的就是安装它，跟踪令牌剥离器将自动删除任何以以下任何文本开头的 URL 令牌:

*   utm_source
*   utm_medium
*   utm _ 术语
*   utm_campaign
*   utm_content
*   utm_cid
*   utm_reader
*   utm_name

正如该扩展的创建者 Jon Parise 所指出的，删除过程发生在 web 请求发出之前的“T0 ”,导致了更私密的浏览和更美观的 URL。你的朋友和社交媒体关注者会感谢你的。