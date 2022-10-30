# 既然 PGP 遭到破坏，如何保护您的电子邮件

> 原文：<https://lifehacker.com/how-to-secure-your-email-now-that-pgp-is-compromised-1826008338>

如果你一直使用 PGP——Pretty Good Privacy 的缩写——来发送和接收加密电子邮件，那么可能是时候换一种不同的服务来维护你的通信隐私了。一个全新的漏洞，被戏称为 EFAIL， [可以明文泄露你的电子邮件](https://gizmodo.com/email-no-longer-a-secure-method-of-communication-after-1826002682#_ga=2.160849021.1392401934.1526304012-3846207152.1521480874) (在某些情况下甚至是更老的电子邮件)的内容。再见，秘密。



如果你只是使用你最喜欢的电子邮件服务给朋友发送常规消息， [阅读令人敬畏的时事通讯](https://lifehacker.com/the-lifehacker-staffs-favorite-email-newsletters-1821200598) ，或者让你生气的业务爆炸，这些问题根本不会影响你。你会知道你是否在使用 PGP，因为这个程序的整个前提是基于 [使用公钥和私钥](https://lifehacker.com/how-to-encrypt-your-email-and-keep-your-conversations-p-1133495744)——巨大的文本串——来加密和解密消息。理想情况下，秘密信息不仅仅是你想发送给你的另一半的有趣的猫图片。

现在有一些关于 EFAIL 漏洞实际上有多大问题的辩论，因为一些公司和有安全意识的人注意到，如果你只是确保你没有收到 HTML 电子邮件，而是切换到明文，你会没事的。正如 GnuPG 的 [沃纳·科赫的](https://lists.gnupg.org/pipermail/gnupg-users/2018-May/060315.html) 写道:

> *“有两种方法可以减轻这种攻击*
> *——不要使用 HTML 邮件。或者，如果您真的需要阅读它们，请使用适当的 MIME 解析器，并禁止对外部链接的任何访问。*
> *——使用认证加密。”*

无论问题出在 PGP 和 S/MIME，正如电子前沿基金会指出的，还是电子邮件客户端本身，你对加密通信的适应程度将决定你的下一步行动。正如 [efail.de](https://efail.de/#mitigations) 所指出的，你可以采用一些技巧来减轻 efail 对你的安全通信的影响:

> *“短期:邮件客户端不解密。防止 EFAIL 攻击的最好方法是只在电子邮件客户端之外的单独应用程序中解密 S/MIME 或 PGP 电子邮件。首先从你的电子邮件客户端删除你的 S/MIME 和 PGP 私钥，然后通过复制&将密文粘贴到一个单独的应用程序中为你解密来解密收到的加密电子邮件。这样，电子邮件客户端就无法打开渗透通道。这是目前最安全的选择，缺点是这个过程越来越复杂。*
> 
> *短期:禁用 HTML 渲染。EFAIL 攻击滥用活动内容，主要是 HTML 图像、样式等形式。禁止在你的电子邮件客户端显示 HTML 格式的邮件将会关闭攻击电子邮件的最主要途径。请注意，在电子邮件客户端中还有其他可能的与 HTML 无关的反向通道，但这些通道更难利用。*
> 
> *中期:修补。一些供应商将发布补丁，要么修复 EFAIL 漏洞，要么使它们更难被利用。*
> 
> *长期:更新 OpenPGP 和 S/MIME 标准。EFAIL 攻击利用了 MIME、S/MIME 和 OpenPGP 标准中的缺陷和未定义的行为。因此，标准需要更新，这需要一些时间。"*

我们的建议？也许是时候停止使用电子邮件进行加密通信了。EFF 认为这至少是一个临时的解决方案:

> 我们的建议反映了研究人员的观点，即立即禁用和/或卸载自动解密 PGP 加密电子邮件的工具。在论文中描述的缺陷被更广泛地理解和修复之前，用户应该安排使用替代的端到端安全通道，如 Signal，并暂时停止发送特别是阅读 PGP 加密的电子邮件。”

正如《连线》2017 年的一篇文章 中所描述的那样，具有端到端加密功能的应用程序，如 Signal、WhatsApp、confident，甚至是[【Skype】](https://lifehacker.com/how-to-get-end-to-end-encryption-in-skype-1822028186)—[等等，都非常适合发送受保护的通信(就目前而言)。](https://lifehacker.com/secure-messaging-app-showdown-whatsapp-vs-signal-1794684943)

虽然这并不是说这些应用程序中的任何一个，甚至他们用来保护你的消息的信号协议，都不会受到未来的攻击(所有[品种](https://lifehacker.com/how-to-make-sure-your-disappearing-signal-messages-actu-1825921690) )，但内置端到端加密的消息应用程序可能值得考虑作为电子邮件的替代方案来处理你最私人的消息。它们并不是万无一失的，特别是如果有人在另一端有一个受损的设备，但如果你能忍受这种差异，它们总比没有好:

 [https://lifehacker.com/embed/inset/iframe?id=twitter-995950831466876928&autosize=1](https://lifehacker.com/embed/inset/iframe?id=twitter-995950831466876928&autosize=1)