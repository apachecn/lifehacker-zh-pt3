# 使用 Android Doze 应用程序，从手机中挤出更多电池

> 原文:[https://life hacker . com/how-to-squeeze-out-of-your-phone-with-andr-1791336715](https://lifehacker.com/how-to-squeeze-more-battery-out-of-your-phone-with-andr-1791336715)

Android Doze 是一个无名英雄， [当你不使用手机的时候节省你的电池](https://lifehacker.com/how-android-doze-works-and-how-to-tweak-it-to-save-you-1785921957) 。像[Greenify](https://play.google.com/store/apps/details?id=com.oasisfeng.greenify)[force doze](https://play.google.com/store/apps/details?id=com.suyashsrijan.forcedoze)和 [Naptime](https://play.google.com/store/apps/details?id=com.franco.doze&rdid=com.franco.doze) 这样的第三方应用程序可以从你的手机中榨出更多的能量，但如果你调整它们，它们可以做得更多。

Watch

### **第三方应用改善了 Doze 令人印象深刻的电池节省**

Android Doze 的工作原理是 [当你有一段时间没有使用手机时，暂时禁用网络访问等功能](https://lifehacker.com/how-android-doze-works-and-how-to-tweak-it-to-save-you-1785921957) 。在 Android 6.0 中，当你的手机静止不动，屏幕关闭几个小时后，这项功能就会生效。Android 7.0 增加了打开 Doze 的功能，即使你的手机在你的口袋或钱包里(仍然会记录为移动)，只要屏幕关闭。然而，在这两种情况下，Doze 都需要几个小时才能发挥作用。如果你每隔一个小时左右检查一次手机，你就不会得到这些好处。

另一方面，像 [Greenify](https://play.google.com/store/apps/details?id=com.oasisfeng.greenify) 这样的第三方应用程序可以调整 Doze，使其在几分钟而不是几小时后激活。你还可以调整 Doze 工作方式的某些方面，比如它是否在充电时打开，或者它是否禁用 Wi-Fi。有几个这样的应用程序，它们都有不同的优点和缺点，所以我们将逐一介绍它们以及它们的用途。

### **使用 Greenify 进行简单的电池改进，无需 Root**

甚至在 Doze 问世之前，Greenify 就已经是生活黑客最喜欢的 了。它的 [主动瞌睡模式](http://lifehacker.com/use-greenifys-aggressive-doze-mode-to-save-even-more-ba-1760534654) 强制瞌睡在几分钟而不是几小时内激活，为你节省大量电池寿命。如果你使用的是 Android Marshmallow，即使你的设备在移动，它也可以激活 Doze，这通常是为 Nougat 用户保留的功能。

虽然 Greenify [不需要 root](http://lifehacker.com/everything-you-need-to-know-about-rooting-your-android-5789397) ，但是你需要 [输入几个 ADB 命令](http://lifehacker.com/the-easiest-way-to-install-androids-adb-and-fastboot-to-1586992378) 来启用激进的瞌睡模式。第一次运行 Greenify 时，它会使用这里的 步骤引导您完成这个过程 [。如果你已经习惯了 ADB，把你的手机插入你的电脑，根据你的设备输入适当的命令。](https://greenify.uservoice.com/knowledgebase/articles/749142-how-to-grant-permissions-required-by-some-features)

要在 Android 7.0+上启用激进瞌睡(非 root):

`adb -d shell pm grant com.oasisfeng.greenify android.permission.WRITE_SECURE_SETTINGS`

要在旅途中启用瞌睡功能:

`adb -d shell pm grant com.oasisfeng.greenify android.permission.DUMP`

要在禁用休眠的设备或 ROM 上启用主动休眠:

`adb -d shell pm grant com.oasisfeng.greenify android.permission.DUMP`

要为运行 Android 4.4 到 5.x 的旧手机启用唤醒关闭:

`adb -d shell pm grant com.oasisfeng.greenify android.permission.WRITE_SECURE_SETTINGS`

这就是你需要做的！在此之后，Greenify 会每隔几分钟左右自动启用 Doze。如果你在吃棉花糖，你也会得到很多牛轧糖的好处。Greenify 最适合那些想设置好就忘记的人，以及那些不想麻烦调整太多设置的人。

### **ForceDoze 让你在自己的日程上使用 Doze，无 Root 权限**

像 Greenify 一样， [ForceDoze](https://play.google.com/store/apps/details?id=com.suyashsrijan.forcedoze) 可以调整手机上的 Doze，即使你没有 root 访问权限，也可以使用 ADB 命令给予它所需的权限。与 Greenify 不同，它提供了一些额外的选项，可以让 Doze 按照你想要的方式工作。当你第一次运行 ForceDoze 时，它会检查 root。如果你没有它，你需要把你的手机连接到电脑上，运行下面的 ADB 命令:

`adb -d shell pm grant com.suyashsrijan.forcedoze android.permission.DUMP`

之后，点击 ForceDoze 应用程序主屏幕上的大开关将其打开。默认情况下，这将使 Doze 比平时更快地启动。但是，如果您点击菜单按钮并选择设置，您可以更改几个其他有用的选项:

*   **充电时关机:**这个选项会告诉 ForceDoze 在手机插入充电器时使用标准系统设置。如果你把手机放在桌子上，想要及时收到信息，这是很方便的。
*   **忽略锁屏超时:**这个选项会强制 Doze 在你关闭屏幕后立即启动，这样可以节省更多的电池。但是，如果您在关机后立即打开手机，可能需要几秒钟才能重新连接。
*   **在打瞌睡时禁用 Wi-Fi:**如果你经常移动，这可以通过防止你的手机在打瞌睡时不断连接和断开不同的网络来节省电池。然而，如果你经常呆在一个地方，并且总是连接到一个无线网络， [，你可能会更好地离开这个禁用的](http://lifehacker.com/top-10-ways-to-improve-the-battery-life-on-your-phone-a-1725843518) 。
*   **禁用 Doze 的动作感应:**这类似于 Greenify 中的“移动中的 Doze”功能。启用此选项后，即使您的手机在移动，Doze 也会激活——例如，如果它在您的口袋或钱包中。
*   **Doze delay:** 在这里，您可以自定义 Doze 在屏幕关闭后等待多长时间才会激活。如果你喜欢对你的手机行为有很大的控制权，这是你的选择。

ForceDoze 比 Greenify 允许更多的定制，但不幸的是，它不支持 Android 牛轧糖。对于一些功能，如禁用动作感应，这无关紧要，因为 Nougat 已经这样做了，但其他功能如设置自定义延迟会很方便。如果你在吃牛轧糖，想改进 Doze，Greenify 可能是你最好的选择，但 ForceDoze 为棉花糖用户提供了更简单的选择。

### Naptime 给了你更多的选择，但是需要 Root 用户

Greenify 和 ForceDoze 对于那些没有 root 权限的人来说很方便，但是如果你已经给你的手机 设置了 root 权限，那么 [Naptime](https://play.google.com/store/apps/details?id=com.franco.doze&rdid=com.franco.doze) 是你最好的选择。它提供了大多数与 ForceDoze 相同的定制选项。它也不像 Greenify 那样需要任何繁琐的 ADB 命令。你可以禁用运动感应，在屏幕关闭时立即打开 Doze，在充电时禁用 Doze。最重要的是，它还包含了许多其他应用程序没有的功能:

*   **传感器应用白名单:**这允许你选择一个仍然可以使用运动传感器的应用，即使你禁用了所有其他应用的运动传感器。例如，你可以让你的健身应用程序在跑步过程中继续跟踪你的步数，而其他一切都被禁用以节省电池。
*   **不活动超时:**这个高级设置让你决定停止使用手机后多长时间 Doze 应该开启。它是以毫秒为单位设置的，所以要准备一点数学知识。您还可以自定义传感器和定位功能关闭前的等待时间。
*   **定位精度:**此设置可让您自定义手机确定您位置的精度。确定您的精确位置需要更多的电池，因此这可以帮助您节省电力，以换取不太精确的位置数据。

Naptime 有很多高级功能，如果你不知道自己在做什么，你可能不应该乱用。然而，对于根用户来说，这些基本特性已经大大超过了标准的 Doze 功能。

* * *

所有这些应用程序方法都以略微不同的方式做大致相同的事情。每一个都有不同的优势，这取决于你运行的是哪个版本的 Android，你是否有 root 用户，以及你想在多大程度上调整你的设置。然而，所有这些都将有助于你的手机持续一整天。