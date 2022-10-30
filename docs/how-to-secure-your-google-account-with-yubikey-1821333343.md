# 如何使用 Yubikey 保护您的 Google 帐户

> 原文：<https://lifehacker.com/how-to-secure-your-google-account-with-yubikey-1821333343>

如果你还没有给你的谷歌账户添加第二层安全 的 [，你会比你意识到的更加脆弱。如果你使用短信来保护你的账户，你可能会认为你是安全的，但与](https://lifehacker.com/plug-the-security-holes-in-your-two-factor-authenticati-1798403323) [替代验证选项](https://lifehacker.com/which-form-of-two-factor-authentication-should-i-use-1784769336) 相比，即使这样也有其自身的安全问题。你可以使用更安全的认证应用程序，但这需要你在每次登录新设备或应用程序时输入多位数密码。不要只是为了发送一些聊天信息而经常复制和粘贴号码，而是考虑使用一个 [Yubikey](https://lifehacker.com/gifts-for-the-privacy-loving-person-in-your-life-1821227116) 。这是一个微型 USB 驱动器，作为多种服务和操作系统的双因素认证工具。现在，让我们先锁定你的谷歌账户。

Watch

### **yubi key 如何工作**

Yubikeys 是基于硬件的安全密钥，看起来像微型 USB 驱动器(抱歉，你不能在上面存储任何东西)。它们基本上是一键式身份认证工具，你可以将它放入电脑(或者，如果是兼容型号，可以点击你的 NFC 智能手机)来验证你的身份。[Windows](https://www.yubico.com/why-yubico/for-business/computer-login/windows-login/)[MAC OS](https://www.yubico.com/support/knowledge-base/categories/articles/how-to-use-your-yubikey-with-macos-sierra/)[Linux](https://www.yubico.com/why-yubico/for-business/computer-login/linux_login/)都支持基于硬件的认证工具，而 [【脸书](https://www.yubico.com/why-yubico/for-individuals/facebook/) 、Google、Dropbox、Github 等网站也在 [支持的 50 多种服务](https://www.yubico.com/solutions/#) 之列。

它不应该是您使用的唯一形式的双因素身份验证，您还应该尽可能使用双因素身份验证应用程序。您还可以将多个 Yubikeys 与一个帐户关联，因此，如果您的钥匙串上有一个帐户，而您的个人电脑或办公室电脑上有另一个帐户，那么使用这两个帐户可以在您丢失一个帐户时为您提供更多的安全性。即使有人窃取了它，如果没有用户名和密码，他们也无法访问您的帐户，您可以使用您的第二个 Yubikey 或其他授权方法远程停用您已经安全的帐户中的密钥。

### **首先保护您的谷歌账户**

要设置安全密钥，你需要进入谷歌账户的安全设置。你可能启用了双因素认证(我希望使用应用程序而不是短信)，或者将智能手机作为你的 [一键式谷歌登录提示](https://lifehacker.com/googles-one-tap-two-factor-authentication-will-show-inf-1792667945) ，但你必须禁用后者才能启用你的硬件安全密钥。此外，在设置之前，请确定您的密钥没有连接到电脑。

首先，进入你的 [谷歌账户的登录和安全页面](https://myaccount.google.com/security) ，在这里你可以选择配置你的登录选项。选择“登录谷歌”，然后点击双因素认证。向下滚动直到你看到安全密钥选项，然后点击“添加安全密钥”

按照 Google 的提示，插入、点击并命名您的 Yubikey，将其与您的帐户相关联。完成一次性设置后，您将在双因素认证选项列表中看到您的 Yubikey。

要试用它，请注销您的 Google 帐户。当您重新登录时，在输入您的电子邮件地址和密码后，系统会提示您点击触控式 Yubikey 来传输您的身份验证代码，无需任何应用程序。

### **摆脱你的短信认证**

现在你已经有了一个认证应用和一个 yubi key——两种认证你的账户的安全方法——你应该放弃你的短信验证选项这一最薄弱的环节。在谷歌的两步验证页面中，点击你的电话号码旁边的编辑按钮，然后选择“移除电话”现在，你的谷歌账户不仅可以免于脆弱的短信认证，而且由于你可以随身携带的物理硬件(或者变成一个功能强大的时尚配件[)而得到进一步保护。](https://motherboard.vice.com/en_us/article/vbze3d/yubikey-earrings)