# 用这个漂亮的工具跟踪脸书认为你认识的人

> 原文:[https://gizmodo . com/keep-track-of-who-Facebook-this-ni-1819422352](https://gizmodo.com/keep-track-of-who-facebook-thinks-you-know-with-this-ni-1819422352)

脸书在不断地 [注视着你](https://gizmodo.com/tag/people-you-may-know) 。现在，你可以看着脸书回来。Gizmodo Media Group 的特别项目部正在为那些想研究脸书推荐给他们的朋友的人发布一个工具。它叫做“你可能认识的人督察”要使用该工具:

1.  在 Mac 电脑上下载 [应用安装程序](https://s3.amazonaws.com/pymk-inspector/pymk-inspector-0.1.1.dmg) 。(这在智能手机或非 Mac 上不起作用。)
2.  下载应用程序安装程序后，打开它并将“PYMK 检查器”应用程序拷贝到“应用程序”文件夹
3.  转到应用程序文件夹，打开应用程序。您应该会看到它在任务栏中弹出。
4.  前往“检查器设置”并输入您的脸书凭据。(对于那些启用了双因子的用户，你需要在第一次运行应用程序时输入第二个因子。)
5.  您可以通过单击“立即运行”来测试它是否正常工作

Watch

***我们为什么要做这个:***

脸书的“你可能认识的人”功能在问世十年来一直让用户感到困惑和不安:一张熟悉的面孔出现在盒子里，但你和这个人没有共同的脸书朋友。脸书是怎么知道谁是你的二年级老师的？为什么你前任新女友的妈妈会在那里？脸书怎么知道你的妇科医生或精神病医生是谁？

我们写了很多关于你可能认识的人的故事——脸书喜欢称之为 PYMK——试图找出更多关于算法黑匣子里面的东西。这项功能的迷人之处在于，鉴于其拥有的海量数据:来自智能手机的位置信息、他们使用过的 Wi-Fi 网络、他们登录过的 IP 地址、数百万人的通讯录、他们在脸书查看过的账户，理论上脸书*可以通过多少种方式*联系人们...

该公司表示，它主要依靠 [上传的联系人](https://gizmodo.com/how-facebook-figures-out-everyone-youve-ever-met-1819822691) 、共同的朋友和共享的网络(如学校或工作岗位)——但它也表示，还有数十种其他未指明类型的信息可供使用。

即使脸书给了你一个侵入性的(或有害的 )建议——比如当它向客户公开性工作者的真实姓名，或者将医生的病人相互介绍——公司也不会向你展示它用来建立联系的数据。(有时脸书自己 [似乎对该功能的具体工作原理感到困惑](https://gizmodo.com/people-at-facebook-don-t-know-how-facebook-works-1819408514) 。)

由于脸书不会讨论它使用的输入，替代方案是研究它产生的输出:跟踪你朋友的建议，看看它们每天是如何变化的。通过观察建议或建议的模式，有可能找到脸书的公开解释没有涵盖的联系，并试图找出它们是如何发生的。

我们制作了 [PYMK 督察 app](https://s3.amazonaws.com/pymk-inspector/pymk-inspector-0.1.1.dmg) (下载链接)让脸书用户可以做到这一点。一旦你将它下载到你的计算机上，并输入你的脸书凭据，它将每 6 小时检查你的“你可能认识的人”建议，并将这些信息保存到你的计算机上，这样你就可以查看谁在那里出现过，何时出现，以及出现的频率。

我们设计这个工具时考虑到了您的隐私。您的脸书密码和从脸书收集的任何数据都存储在您的计算机上。只有你有权限。我们没有收集任何数据，但是如果您看到一些有趣的东西(或者更确切地说是一些人)，我们很乐意收到您的来信。我们让它开源；这里是 [到工具源代码](https://github.com/GMG-Special-Projects-Desk/pymk-inspector) 的链接。我们还委托了一个来自比特踪迹的安全审查。

从夏天开始，我们就一直在使用这个工具。在内部测试时，我们已经发现了一些奇怪的事情。我们中的一个人就是这样发现脸书正在 [推荐一个不知名的亲戚](https://gizmodo.com/facebook-figured-out-my-family-secrets-and-it-wont-tel-1797696163) 。我们已经记录了一些人根本没有任何好友推荐的事实。“你可能认识的人”模块没有出现在我们的编辑汤姆·斯考卡面前，没有出现在整个网站上，也没有出现在 [的好友请求页面](https://www.facebook.com/friends/requests/) 上，其他人都可以看到。

虽然汤姆再也看不到这个工具，但他仍然出现在里面。他是作为朋友推荐给我们的，就一次，6 月中旬。(我们没有加他为好友。对不起，汤姆！)虽然我们确实认识汤姆，但他只在 PYMK 出现过一次，而其他我们不认识的人却日复一日地出现在那里，一次就出现几个月。

现在我们邀请你加入我们的研究。如果你对脸书是如何跟踪你自己的联系感到好奇，请 [下载工具](https://s3.amazonaws.com/pymk-inspector/pymk-inspector-0.1.1.dmg) 并开始研究你自己的结果。如果你看到一些你无法解释的事情，或者一些脸书不应该知道的事情， [告诉我们](mailto:tips@gizmodomedia.com) 。在你的帮助下，也许我们能更清楚地看到黑匣子。

* * *

<section class="q35npn-0 MZtuu">![](../Images/aef335eb562a1da6957ce25a574b4aa1.png)

#### 联系特别项目服务台

本帖由 Gizmodo Media 的 [特别项目组制作。](https://specialprojectsdesk.com) 通过电话、短信、信号或 WhatsApp 联系我们的团队，电话:  ，电子邮件:[【tips@gizmodomedia.com】](mailto:tips@gizmodomedia.com)，或使用 [SecureDrop](https://specialprojectsdesk.com/securedrop/) 安全地联系我们。

</section>

* * *