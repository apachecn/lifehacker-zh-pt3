# 在安装 10 月更新之前备份 Windows 10，否则可能会丢失文件

> 原文：<https://lifehacker.com/back-up-windows-10-before-installing-the-october-update-1829556930>

我们都在绞尽脑汁想知道 Windows 10 十月更新是如何通过微软的质量保证团队的。据众多报道称，更新可能会删除 Windows 10 用户文件夹中的内容——你知道，你的文档、照片、音乐、视频等。



正如一位 Reddit 用户 所描述的:

> *“正如我在另一篇文章中提到的，升级删除了%userprofile%\documents 和\pictures，它们不是默认文件夹(即“我的文档”、“我的图片”库的一部分)。我的默认文件夹过去和现在都在 OneDrive 中，升级时没有动过。仅删除了%userprofile%中的文件夹，即使它们不是空的。*
> 
> 大胆猜测:也许问题不在于安装程序错误地删除了内容，而是它认为某些文件夹不再被使用而没有迁移它们？我不熟悉升级过程的内部，但我可以想象安装程序首先将旧内容复制到“Windows.old ”,然后删除旧安装(从而删除所有文件),执行操作系统的全新安装，最后从“Windows.old”恢复用户数据。这就解释了为什么我在“Windows.old”中找不到我的文件——由于遇到了一些未知的情况，安装程序没有在第一时间复制它们，因此无法在以后恢复任何东西。"

而 [另一个](https://www.reddit.com/r/Windows10/comments/9l2v3z/windows_1809_update_wiped_my_documents/e75rgu4/) 写道:

> *“我的 D:\Document 文件夹丢了。它没有被配置为文档库，甚至不在系统驱动器中！我没有这方面的备份，因为我认为系统升级不应该触及非系统驱动器。”*

不管这些删除为什么会发生——微软正“ [积极调查](https://wccftech.com/windows-10-october-2018-update-deleting-user-data/) ”这个问题——以下是你如何避开这个巨大的 Windows 混乱。

### 在重大更新之前备份您的系统

我很懒。当一个大的系统更新到来时，我总是迫不及待地点击“检查更新”链接，让所有这些可爱的新功能和修复从 Redmond(或任何地方)流到我的桌面上。Windows 10 十月更新对我和所有人都是一个很好的提醒，我们应该在安装任何重大更新之前备份我们的系统。

如果你能完全复制你的主硬盘，那太好了！如果更新出现任何糟糕的问题，你可以恢复到之前的操作系统版本。否则，你至少应该定期备份你的重要文件。

程序和应用程序可以重新安装，但 C:\ Users \[你的名字]中的任何主要文件夹，如文档、图片、视频、桌面等，也应该位于其他位置。也许还有两个地方。提醒每周将它们复制到 [云存储服务](https://lifehacker.com/google-one-is-now-open-for-everyone-but-is-it-a-good-d-1826049257) 。定期用像 [Backblaze](https://lifehacker.com/how-do-you-back-up-your-data-in-the-cloud-1828396275) 这样的应用程序备份它们。在外部驱动器或网络连接存储设备上为您的大型照片库创建一个副本归档。不管你怎么做，没有理由让你不能理解丢失的文件只存在一个地方。不不不。

### 如何恢复 Windows 10 删除的文件

如果你刚刚安装了 Windows 10 十月更新，发现它销毁了你的一些(或所有)关键用户文件夹，而你没有在其他地方备份它们，请立即停止你正在做的事情。不做别的。去下载免费版的 [Recuva](https://lifehacker.com/how-can-i-recover-data-from-a-dead-or-erased-hard-drive-5951822#_ga=2.161364283.765649883.1538688414-396842925.1520800403) 。安装它，在你的 Windows 驱动器上运行一个扫描，你也许能保存你的数据。不敢保证，但这是你目前最好的选择。

如果你之前打开了 Windows 的内置文件历史工具，你也可能会很幸运，该工具允许你恢复文件和文件夹的旧副本。您可以通过**设置**app>T6】更新&安全 T12】T8】备份打开文件历史。要恢复文件历史以前保存的文件夹，在文件资源管理器中导航到其父文件夹，右键单击它，选择属性，然后单击“以前版本”选项卡。