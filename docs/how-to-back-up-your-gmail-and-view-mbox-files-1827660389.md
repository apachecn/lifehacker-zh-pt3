# 如何备份您的 Gmail 和查看？MBOX 文件

> 原文:[https://life hacker . com/how-to-back-up-your-Gmail-and-view-mbox-files-1827660389](https://lifehacker.com/how-to-back-up-your-gmail-and-view-mbox-files-1827660389)

你想备份你的 Gmail 账户有很多原因，比如:有一份你最重要的数据的备份是件好事；你即将被解雇，你想挽回你所做的一切；你会只是想要一点额外的保护，以防有人侵入你的账户并接管(或删除)。

Watch

虽然我们大多数人可能相信我们的 Gmail 账户会永远存在——因为这是谷歌的问题，而不是我们的——但备份你的电子邮件总是值得的。最坏的情况？你永远不需要后援。最好的情况？当灾难降临时，你可以防止精神崩溃。这样你就能拿回你的数据了。

### 从谷歌下载一切

备份 Gmail 最简单的方法恰好来自谷歌自己。进入谷歌账户设置的“ [下载你的数据](https://takeout.google.com/settings/takeout) ”部分，通过“不选”框取消所有选择(否则这个过程将花费更长的时间)，向下滚动直到你看到邮件选项。选择那个。如果你不想备份你所有的 Gmail，只想要带有特定标签的电子邮件，你也可以点击向下箭头来获得关于谷歌保存的更具体的信息。

一旦你做出选择——“包含你所有的邮件”对大多数人来说已经足够了——滚动到页面底部，点击下一步。我倾向于在下一个屏幕上保留所有选项的默认值，但是如果您认为您有大量的电子邮件和附件需要备份，并且想要处理较少的文件，您可以随时更改归档大小。你也可以指示谷歌自动将你的备份转储到你的 Google Drive 或者 Dropbox、OneDrive、box。我通常只是让谷歌给我发一个下载链接，这样我就可以把我的备份存储在我的电脑、NAS box 或其他便携式存储设备上。

当你准备好了，点击“创建档案”,当谷歌备份你的东西时，花些时间放松一下。

### 我该怎么处理这个。MBOX 文件？

一旦你解压缩谷歌的档案，你会看到一个(或几个)。MBOX 文件。查看他们的内容——你的电子邮件——可能是一个繁琐的过程。首先，抢雷鸟——Mozilla 的 [未死](http://forums.mozillazine.org/viewtopic.php?f=39&t=366405) 邮件客户端。如果你只是需要一个快速简单的版本来查看档案。MBOX 文件，我推荐下载 [雷鸟](https://portableapps.com/apps/internet/thunderbird_portable) 的便携版而不是完整的 [雷鸟客户端](https://www.thunderbird.net/en-US/) 。你的电话。

一旦你进入雷鸟，点击工具，然后加载项。点击左侧边栏顶部的 Get Add-ons，搜索[ImportExportTools](https://addons.mozilla.org/en-US/thunderbird/addon/importexporttools/)。安装那个。

返回“本地文件夹”选项卡。再次点击工具，向下滚动到导入导出工具，并选择“导入 mbox 文件。”选择对您最有意义的选项—导入单个。MBOX 文件或多个——然后找到。您从 Google 下载的 MBOX 文件。

将你的邮件转储到 Thunderbird 可能需要一点时间，这取决于它需要处理多少封邮件，但你应该会看到它们都作为一个文件夹(或多个文件夹)在 Thunderbird 中弹出。现在，您可以随意点击它们(并重新保存附件)。

这也是你用来将你的邮件 [恢复到你的 Gmail 账户](http://onedoor.cdnis.edu.hk/2016/10/restore-gmail-backup-into-another-account/) 的过程的一部分——或者将它们复制到一个新的 Gmail 账户，如果你的旧账户一切正常的话。

如果你不想对雷鸟和一个附加软件大惊小怪，你可以试试这个应用程序 [CutePieSMPT 守护程序](https://github.com/elFua/cutepiesmtp) ，它也可以让你非常容易地查看一个附加软件的内容。MBOX 文件。当我使用这款应用时，感觉有点滞后，还崩溃过一次，但如果你只是需要快速查看你下载的 Gmail 存档中的一些东西，这是一个不错的选择。我也喜欢它的名字。

如果你在 Mac 上，你可以使用苹果的邮件应用程序来导入。MBOX 文件。打开应用程序，点击文件，然后点击“导入邮箱”确保“mbox 格式的文件”被选中，然后找到您的。MBOX 文件。您导入的任何内容都将被放入 Mail 的“在我的 Mac 上”部分，作为新“导入”文件夹的子文件夹。