# 如何安全处置固态硬盘

> 原文：<https://lifehacker.com/how-to-securely-dispose-of-an-ssd-1793336156>

固态硬盘(SSD) [的工作方式](http://lifehacker.com/how-to-securely-erase-a-solid-state-drive-on-mac-os-x-1580603733) 与硬盘稍有不同，而 [再多的钻孔、消磁或归零](https://lifehacker.com/how-to-erase-and-format-a-hard-drive-1525128357) 实际上也无法正确保护 SSD。如果你需要摆脱固态硬盘，你有几个选择， [加密](https://lifehacker.com/a-beginners-guide-to-encryption-what-it-is-and-how-to-1508196946) 或粉碎。以下是你需要知道的。

Watch

如果你对传统格式化或硬盘销毁不是安全擦除固态硬盘上数据的最佳方式的技术原因感到好奇， [Backblaze 有一个很好的指南](https://www.backblaze.com/blog/how-to-securely-recycle-or-dispose-of-your-ssd/) 详细说明了为什么旧的硬盘方法不起作用。简而言之，没有标准的方法可以安全地从固态硬盘中删除数据，这意味着固态硬盘没有普遍接受的安全格式选项。一些制造商开发了自己的软件来格式化他们自己的硬盘，但是很难独立验证其中的任何一个。

相反，Backblaze ( [和其他](http://www.computerworld.com/article/2506511/solid-state-drives/can-data-stored-on-an-ssd-be-secured-.html) )建议两种方法，加密 SSD 并扔掉密钥，或者粉碎它。粉碎固态硬盘需要一台我们大多数人都无法使用的特殊机器，所以我们只关注加密方法。这对于我们大多数不从事绝密项目的人来说已经足够好了，因为没有加密密钥，加密的 SSD 基本上只是一个充满随机 1 和 0 的驱动器。

无论出于什么原因，如果你要放弃固态硬盘，过程很简单，首先加密，格式化，如果你想超级小心，再加密一次。

本指南假设您想要删除、销毁并永远不再访问您计算机上的数据，因此请确保所有数据都已备份，因为您将无法再访问这些数据。

### 如何在 Windows 上加密固态硬盘

Windows 内置了名为 Bitlocker [的加密软件，非常容易设置](https://www.howtogeek.com/234826/how-to-enable-full-disk-encryption-on-windows-10/) ，但仅限专业用户使用。所以，作为一个免费和可访问的选项，我们喜欢 [VeraCrypt 也同样喜欢](https://lifehacker.com/windows-encryption-showdown-veracrypt-vs-bitlocker-1777855025) 。

1.  下载安装 [VeraCrypt](https://veracrypt.codeplex.com/) 。
2.  启动 VeraCrypt 并选择系统>加密系统分区/驱动器。
3.  出现提示时，选择普通加密，然后单击下一步。
4.  选择“加密整个驱动器”
5.  假设您只安装了一个操作系统，选择单引导并单击下一步。
6.  对于加密选项，您可以保留默认设置:AES 用于加密算法，SHA-256 用于哈希算法。
7.  创建一个密码。在这个过程结束之前，你需要再输入一次，所以现在把它写下来。
8.  按照屏幕上的指示移动鼠标，完成后单击下一步。
9.  当要求创建救援盘时，单击“下一步”。这是一个必需的恢复选项，假设您想继续使用此 SSD。
10.  为擦除模式选择“1 遍”,然后单击下一步。
11.  最后，单击 Test 测试所有内容。一旦你的电脑重新启动，你会被要求输入密码。输入密码，然后按照屏幕上的说明完成加密过程。

一旦你完成，你可以扔掉加密密钥，使任何人都几乎不可能从 SSD 恢复数据，如果他们发现。

### 如何在 Mac 上加密固态硬盘

您可以使用内置的加密工具 FileVault 在 Mac 上轻松加密您的固态硬盘:

1.  打开“系统偏好设置”,进入“安全性与隐私”>“FileVault”。
2.  点按锁图标并输入您的密码。
3.  点按“打开 FileVault”
4.  出现提示时，选取“创建恢复密钥，不要使用我的 iCloud 帐户”,然后按下“继续”。通常，您会特别记下这个恢复密钥，以便以后可以访问它。既然你在破坏固态硬盘，那就不是问题了。
5.  出现提示时，重新启动计算机。

您 Mac 的固态硬盘现在已加密。

您现在可以 [格式化驱动器](https://lifehacker.com/how-to-erase-and-format-a-hard-drive-1525128357) 。如果你想特别小心，格式化之后，再加密一次。这确保了第一加密密钥被完全覆盖。这样做不会对有人访问它的可能性产生很大的影响，但对安心来说更好一点。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled How to Securely Dispose of an SSD](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-to-erase-and-format-a-hard-drive-1525128357) [###### 如何擦除和格式化硬盘](https://lifehacker.com/how-to-erase-and-format-a-hard-drive-1525128357) 

格式化硬盘是一个令人讨厌的项目从头开始的最佳方式。你会想…

[Read more](https://lifehacker.com/how-to-erase-and-format-a-hard-drive-1525128357)</aside>