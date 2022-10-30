# 如何保护自己免受 Meltdown 和 Spectre(最新的处理器安全缺陷)的影响

> 原文：<https://lifehacker.com/how-to-protect-yourself-from-meltdown-and-spectre-the-1821781392>

几乎你所有的设备中都有一对安全漏洞，这可能会让黑客窃取密码和其他个人信息。Spectre 和 Meltdown 这两个漏洞利用了设备微处理器设计中的实际缺陷。你的电脑、智能手机和其他设备可能会在未来几年受到影响或变慢，但在找到长期解决方案的同时，公司已经提供了补丁，至少可以部分保护你免受眼前的威胁。

Watch

### 【Spectre 和 Meltdown 如何工作

处理器漏洞 [Meltdown 和 Spectre](https://meltdownattack.com/) (后者是一对两个类似的漏洞)，本质上是针对处理器优化某些动作的方式，这种功能被称为“投机执行”该漏洞允许他们查看其他程序和服务内部的内存(包括个人信息),直到操作系统的核心。你的杀毒软件解决不了这个问题。Meltdown 缺陷主要影响英特尔驱动的机器，如台式机或 MacBook，而 Spectre 缺陷影响 AMD 和 ARM 的处理器。这意味着你的智能手机也可能受到处理器缺陷的影响。

### **如何保护自己不被熔毁**

幸运的是，微软和谷歌等公司已经在修补这个漏洞。为确保您是最新的，请遵循您的操作系统的说明。

**微软** : [微软](https://support.microsoft.com/en-us/help/4072699/important-information-regarding-the-windows-security-updates-released) 已经发布了针对 Windows 10 修补漏洞的更新，即将发布 Windows 7 和 Windows 8 的补丁。如果您在安装自动安全更新时遇到问题，微软建议您的反病毒软件可能是罪魁祸首。如果是这样，关闭你的反病毒程序，使用 Windows Defender 或 Microsoft Security Essentials([或编辑你的注册表](https://support.microsoft.com/en-us/help/4072699/important-information-regarding-the-windows-security-updates-released) ，如果你确信你不会搞砸的话)。 [如果你使用的是 Windows 10](https://support.microsoft.com/en-us/help/12373/windows-update-faq) ，很可能你已经自动下载了更新，或者已经按照设定的时间表进行了更新。高级用户可以在命令行 中运行 [微软的验证测试来检查自己是否受到影响。](https://support.microsoft.com/en-us/help/4073119/windows-client-guidance-for-it-pros-to-protect-against-speculative-exe?ranMID=24542&ranEAID=nOD%2FrLJHOac&ranSiteID=nOD_rLJHOac-cUyR1xyRduFhNJVGwlEG1A)

**苹果**:虽然苹果尚未对该漏洞发表评论，但 Windows 安全专家 [亚历克斯·约内斯库](https://twitter.com/aionescu/status/948609809540046849) 指出，macOS 的 [新 10.13.3 更新](https://lifehacker.com/how-to-clean-up-and-optimize-your-sluggish-mac-1794877821) 中存在一个修复程序。

**浏览器** : [谷歌 Chrome](https://support.google.com/faqs/answer/7622138#chrome) ， [Mozilla 的 Firefox](https://blog.mozilla.org/security/2018/01/03/mitigations-landing-new-class-timing-attack/) 和微软 Edge 都已经更新或计划更新以修补安全漏洞。你可以在 1 月 23 日将谷歌 Chrome 更新到最新的补丁版本，或者 [下载火狐最新更新](https://lifehacker.com/why-you-should-check-out-the-new-firefox-quantum-browse-1820430885) 。

Android :据谷歌称，运行最新版本 移动操作系统的 Android 用户 [受到保护。](https://support.google.com/pixelphone/answer/4457705)

### **如何保护自己免受幽灵的伤害**

虽然你可以保护自己免于崩溃，但很难抵御更具侵入性的 Spectre 缺陷。据参与发现和报告这两个漏洞的研究人员 称，修补 Spectre 中特定漏洞的软件更新是可能的，尽管目前还没有可用的软件，或者能够完全解决漏洞，而无需重新设计操作系统和微处理器本身。