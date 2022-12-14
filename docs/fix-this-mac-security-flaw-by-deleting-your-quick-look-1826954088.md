# 通过删除您的快速查看缓存来修复此 Mac 安全缺陷

> 原文：<https://lifehacker.com/fix-this-mac-security-flaw-by-deleting-your-quick-look-1826954088>

今天流传的一份令人不快的新报告很好地提醒了人们，你 Mac 的快速查看功能——尽管它可能有助于通过捣碎空格键来预览文件——[存储关于你连接到系统的加密 USB 驱动器](https://gizmodo.com/one-of-macos-most-useful-features-may-be-making-your-f-1826919516#_ga=2.109195843.775378703.1529327013-1723114163.1524514905) 的内容的信息。



换句话说，连接一个你之前通过 macOS 或使用第三方加密工具加密的驱动器，在你的 Mac 上快速打开它的内容——比如一些你间谍活动的秘密照片——你的 Mac 就会为你打开的内容生成一个缓存。它把这个缓存存储在你的(大概)未加密的硬盘上，而且它 [访问](https://wojciechregula.blog/your-encrypted-photos-in-macos-cache/) 它的内容，你浏览过的文件的名字和缩略图也不是那么棘手。

如果你非常注重隐私，希望你的 Mac 不要泄露你的加密 USB 密钥的秘密内容，你有一些方法来解决这个问题:

*   不要让别人碰你的 Mac。要查看您的 Quick Look 缓存，必须有人能够物理访问您的系统，这也是一种绕过您的安全性、验证您的机器并进行一些窥探的方法。防止这种情况的最简单的方法是使用强密码，用触控 ID 锁定您的系统(如果适用)，并且不要让您的 Mac 离开您的视线。
*   给你的 Mac 加密。如果你使用 FileVault，这整个问题就不再是问题了。“快速查看”仍会将缓存文件存储在您的系统上，但您的系统文件将被加密。因此，即使有人偷了你的笔记本电脑，并试图了解你用它查看的所有秘密，他们也不会走得太远，除非他们能以你的身份登录。如果他们可以的话，世界上没有任何加密技术可以阻止他们做任何他们想做的事情或者查看任何他们想看的东西(很明显)。
*   **删除您的快速查看缓存。**为了更加安心，您可以简单地定期 [删除您系统的快速查看缓存](https://objective-see.com/blog/blog_0x30.html) 。打开终端，输入这个，然后按回车键:`qlmanage -r cache`