# 如何保护您的 BitTorrent 客户端免受这种潜在的黑客攻击

> 原文：<https://lifehacker.com/how-to-protect-your-bittorrent-client-from-this-potenti-1822123134>

还在用 [BitTorrent](https://lifehacker.com/torrenting-showdown-transmission-vs-qbitorrent-vs-tor-1786122054) 专门下载合法获取的内容比如操作系统镜像或者 [你想私下分享给好友的文件](https://lifehacker.com/how-to-create-a-super-private-bittorrent-community-for-5952148) ？如果是这样，你可能需要仔细检查你的安全设置，以保护自己免受谷歌 Project Zero 的研究人员所说的影响传输和其他流行的 BitTorrent 客户端的“低复杂性黑客”的攻击。该缺陷可能会使您的计算机容易受到恶意黑客的控制，但您可以通过遵循一些步骤来保护自己，直到官方修复到位。

Watch

Ars Technica 解释说, 的概念验证攻击会影响通过网络浏览器控制 BitTorrent 客户端的用户，让他们远程管理传输。许多启用了远程访问的客户端不受保护，并且不要求用户输入密码。

Project Zero 研究员蒂姆·奥曼迪解释说，这个缺陷利用了松懈的安全性，让黑客通过 web 界面执行命令，将你的 BitTorrent 客户端变成一个接入点，错误的人可以在获得你的 Torrent 下载后运行他们想要的任何代码。

虽然 Project Zero 在提供修复后才披露了传输中的缺陷，但根据这条来自奥曼迪 的 [推文讨论了未指明的 BitTorrent 客户端中存在的缺陷，其他 BitTorrent 客户端可能会面临类似的安全问题。](https://twitter.com/taviso/status/951526615145566208)

 [https://lifehacker.com/embed/inset/iframe?id=twitter-951526615145566208&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-951526615145566208&autosize=1) 

### **如何保护自己**

一名代表告诉 Ars Technica，一个补丁来自传输，但是你可以通过修改一些安全设置来保护自己免受黑客攻击。为了快速使黑客无用，你需要在你的 BitTorrent 客户端禁用远程访问服务。在传输中，您可以简单地访问您的首选项，点击远程标签，并取消选中“启用远程访问”选项。

如果你宁愿让你的远程访问选项保持启用，你至少应该确保对它进行密码保护( [，并将该信息存储在你的密码管理器](https://lifehacker.com/what-to-put-in-your-password-manager-1822118327) )。您可以从启用(或禁用)对计算机的远程访问的“远程”选项卡中执行此操作。

[BitTorrent 用户当心:漏洞让黑客控制你的电脑](https://arstechnica.com/information-technology/2018/01/bittorrent-users-beware-flaw-lets-hackers-control-your-computer/) | **Ars Technica**