# 为什么我的 USB 不能在我的电脑上显示？

> 原文：<https://lifehacker.com/why-wont-my-usb-show-up-on-my-pc-1823887066>

欢迎来到每周第一期的 Tech 911，这是我们全新的技术建议专栏，旨在帮助您解决您的台式机、笔记本电脑或其他喜爱的设备所遇到的问题。



在本周的创刊号中，我们来看看丢失 USB 设备的奇怪案例——这个问题不应该成为问题，因为这个标准应该是世界上最容易处理的。你插上东西，等待 *ba-donk* 声(至少在 Windows 上)，然后开始浏览你的闪存盘/听你的耳机/使用你插在电脑上的任何东西。

有时候，这种情况不会发生。

### 我的 u 盘去哪了？

Lifehacker 读者[](https://kinja.com/John--W)**写道:**

**现在，我的电脑无法识别我的 usb 闪存驱动器。我把它插在几个不同的端口上，但没有成功。我把它插在另一台电脑上，它能很好地识别它。我尝试卸载并做“扫描硬件变化”,但没有骰子。有什么解决办法吗？**

**对于寻找丢失的 USB 设备，没有一刀切的解决办法，但我至少可以建议一些技术，希望能帮助您发现您的计算机似乎已经丢失或忽略的设备。**

### **先排除更大的问题**

**首先，我假设这是 Windows 的问题。我以前在微软的操作系统上遇到过这个问题，但从未在 Mac 上遇到过。(不是说这不可能；只是没碰到而已。)**

**我先告诉你最坏的结果:你的电脑可能有一些奇怪的硬件问题，使得你的系统现在看不到任何 USB 设备。也许你的 USB 端口 [损坏了](https://www.makeuseof.com/tag/dead-usb-port-heres-how-to-diagnose-and-fix-it/) 或者你的系统控制器已经完全死机了。**

**如果是这样，那就没有什么是你可以(或者可能应该)自己解决的了。假设你还在保修期内，你需要联系你的电脑制造商寻求保修服务。如果你自己构建了你的桌面系统，如果这个问题真的困扰你，可能是时候换一个新的主板了。(你也可以买一个通过 PCI 插在主板上的第三方内置 USB 卡，这样至少会给你*一些* USB 的功能。)**

### **使用设备管理器做一些检测工作**

**假设我们不是在处理一个灾难性的硬件问题，一个了解正在发生什么的好方法是在你插入 USB 设备后看看 Windows 的设备管理器。在 Windows 10 中，你可以点击开始按钮，输入“设备”，或者你可以打开控制面板，点击“设备管理器”。**

**我想做的第一件事是告诉 Windows 手动扫描 USB 设备。单击您的计算机名称，单击操作菜单，然后单击“扫描硬件更改”运气好的话，Windows 会找到您丢失的设备(不管是什么原因丢失的)，您将能够再次访问它。**

**如果当您启动设备管理器时，您的计算机的一个设备类别被扩展，并且在一个特定的列表旁边有一个令人不愉快的警告图标，那么是时候深入挖掘了。硬件连接可能是正常的，但无论什么原因，Windows 没有找到它以前识别的设备。**

**我的第一个想法是确保您的设备拥有来自制造商的最新驱动程序——然而，这并不真正适用于您的情况，因为您的 USB 闪存驱动器不太可能需要任何特殊的驱动程序才能工作。(如果你有 USB 打印机之类的问题，那就另当别论了。)**

**您可以尝试右键单击带有警告图标的设备，卸载它，然后再次扫描硬件更改。如果这不起作用，打电话给你的台式机或笔记本电脑的制造商——或者，根据你的系统，你的主板制造商——看看是否有任何更新的 USB 控制器驱动程序。安装这些也可能解决问题。(确保您的系统运行的也是最新的 BIOS，您通常可以通过台式机、笔记本电脑或主板制造商提供的一些软件实用程序检查并自动安装。)**

**既然你在专门谈论 USB 闪存的问题，life hacker reader[**WhiskeySnob**](http://lifehacker.com/1823826296)**指出，Windows 可能只是在为你的设备分配驱动器盘符时遇到了问题。插入 USB 设备后，点击开始菜单，输入“计算机管理”，然后选择它。(你也可以在你的常规控制面板下找到“电脑管理”。)****

****在那里，找到左侧边栏中的存储部分，然后单击“磁盘管理”您的 USB 闪存盘是否出现在存储设备列表中？它有驱动器号吗？尝试通过右键单击分区来给它分配一个驱动器号(或更改其驱动器号)。****

****微软自己建议确保你的 u 盘不会因为任何原因意外断电，你可以通过禁用设备的选择性挂起来解决这个问题(向下滚动到 [方法 5](https://support.microsoft.com/en-us/help/2654149/error-usb-device-not-recognized-when-you-try-to-access-a-usb-external) )。****

****最后，有可能你的 u 盘只是坏了。将它插入你拥有的另一台台式机或笔记本电脑，甚至一个朋友的系统，它能工作吗？你能访问你的文件吗？如果不是，你的设备可能是罪魁祸首，而不是你的电脑。是时候去买一个新的 USB 驱动器了！****

****如果你有一个让你挠头的技术问题，或者你只是想得到关于完成某项技术任务的最新和最佳方法的建议，请在评论中告诉我们！ *您也可以将您的问题电邮至*[](mailto:david.murphy@lifehacker.com)**。这些问题不会按照收到的顺序来回答，但它们可能会出现在下周的专栏中！******