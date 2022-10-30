# 加密您的闪存驱动器，确保您高枕无忧

> 原文：<https://lifehacker.com/encrypt-your-flash-drive-to-ensure-your-peace-of-mind-1820010000>

我们都丢了一两个闪存盘。无论是包含一些宣传材料的廉价 USB 驱动器，还是详细说明与某个英国女王旅行计划有关的安全协议的绝密驱动器，有时我们会忘记事情，不得不希望我们的敏感信息不会落入坏人之手。通过事先加密您的闪存驱动器来保护您的硬件，可以防止未经授权的个人进入您放错位置的介质。它不会让你的闪存盘恢复得更快，但你会知道，当你的 USB 逍遥法外时，你和你的数据不会有危险。

Watch

### **Mac 用户:Finder 可以给你加密**

如果你用 Mac 加密你的闪存盘，你需要在加密之前对闪存盘做一些小的修改。Apple 使用 HFS+文件系统来加密可移动媒体，因此您需要使用该文件系统来格式化驱动器。打开“磁盘工具”应用程序，选择您的 USB 驱动器，然后选择“抹掉”。选择 MacOS 扩展(日志)格式，擦除驱动器，用正确的文件系统格式化。

现在你可以加密你的硬盘了。在 Finder 中，右键单击您的 USB 驱动器。选择“加密”并输入密码，以防不速之客进入。加密不是即时的，因此您可能需要等待几分钟，这取决于您的闪存驱动器有多大。尽管如此，你最终还是会有一个安全的闪存盘，不用担心在希思罗机场泄露皇室的秘密路线。

### **Windows 用户:试试 BitLocker 或 Veracrypt**

Windows 自带内置文件加密软件， [戏称为 BitLocker](https://lifehacker.com/windows-encryption-showdown-veracrypt-vs-bitlocker-1777855025) 。它存在于 Windows Vista 的专业版、旗舰版或企业版以及更高版本中，包括 Windows 10。BitLocker 适用于 NTFS、FAT 或 FAT32 文件系统。右键单击你的驱动器并选择“格式化”将让你选择你想要在新格式化的驱动器上使用哪个文件系统。

从那里开始，加密你的移动硬盘是相当容易的。在文件浏览器中选择驱动器，点击顶部的管理选项卡。选择 BitLocker，然后打开 BitLocker。您必须输入两次密码，或者使用智能卡(如果有的话)。然后，您可以将恢复密钥(以防忘记实际密码)保存到您的 Microsoft 帐户、PC 上的文件中，或者打印出来并存储在安全的地方。

如果你使用的是不同版本的 Windows，或者出于某种原因宁愿避免使用 BitLocker，你总是可以使用 [VeraCrypt](https://www.veracrypt.fr/en/Home.html) 。可爱的读者们，这是 [中最受欢迎的文件加密应用](https://lifehacker.com/most-popular-file-encryption-tool-veracrypt-1685273934) 之一。