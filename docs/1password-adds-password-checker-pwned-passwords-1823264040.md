# 通过向 1Password 添加“Pwned 密码”,查看您的密码是否已被泄露

> 原文：<https://lifehacker.com/1password-adds-password-checker-pwned-passwords-1823264040>

任何意识到像 Equifax 或 [Kickstarter](https://lifehacker.com/15-million-hacked-kickstarter-and-bitly-passwords-are-n-1819216049) 这样的公司在处理敏感信息时记录不佳的人，可能都会好奇他们的密码有多强。通过随机生成的密码通常比你自己发明的密码更安全(看着你，“abc123”)。现在，您可以使用 1Password 检查您的密码是否是不断增加的泄露密码 [的一部分，该软件刚刚将破解的密码数据库](https://blog.agilebits.com/2018/02/22/finding-pwned-passwords-with-1password/) [Pwned 密码](https://haveibeenpwned.com/Passwords) 集成到其应用程序中。



特洛伊·亨特是“我被密码了吗” 的开发者，这是一个免费网站，允许用户输入他们的电子邮件地址，并将其与受损账户的数据库进行比较。还记得几年前 Kickstarter 和 bit . lyT5 被攻陷的时候吗？嗯，你可以使用我有没有被密码，看看你的帐户是否在名单中被攻破的帐户。使用 Pwned 密码，您可以检查您使用的其他密码的强度和受欢迎程度，并将其与超过 5 亿个公开可用密码的数据库进行比较，这些密码都与受攻击的帐户相关联。

要开始在 1Password 中使用 Pwned 密码，您需要在 1Password 的网站上通过 [登录您的账户](https://start.1password.com/) 来启用该功能。选择一个登录项目，如果你在 macOS 电脑上，点击 *Shift-Control-Option-C* ，或者在 Windows 上点击 *Shift-Ctrl-Alt-C* 。然后，您将看到“检查密码”选项，这将让您知道该密码是否存在于 Pwned 密码数据库中。

 [https://lifehacker.com/embed/inset/iframe?id=youtube-video-6VyvFJgu-jw&start=0](https://lifehacker.com/embed/inset/iframe?id=youtube-video-6VyvFJgu-jw&start=0) 

如果您的密码在数据库中被发现，那么它比不在 Pwned Password 的破解密码列表中的密码更有可能遭到破坏。黑客采用“凭据填充”等方法，使用用户名和密码对的数据库来快速找到容易被攻破的帐户。如果您的字符串不是使用 1Password 这样的密码管理器随机生成的，您应该使用 Pwned 密码来验证您当前选择的强度( [，然后再更改它](https://lifehacker.com/how-to-create-a-strong-password-1797681069) )。