# 如何用苹果的 HomeKit 控制未经批准的智能家居小工具

> 原文：<https://lifehacker.com/how-to-control-unapproved-smart-home-gadgets-with-apple-1820775984>

苹果的 [家庭应用](https://gizmodo.com/apple-joins-the-smarthome-wars-with-a-siri-powered-app-1781900675) 可以让你轻松地从 iPhone 上控制你所有的智能家居技术，但因为这是我们正在处理的苹果，它也有一些限制。最大的缺点是，Home 只能与一小部分 [HomeKit](https://lifehacker.com/apple-releases-tvos-10-with-smarter-siri-homekit-suppo-1786590814) 认可的智能灯、开关和其他小工具一起工作。

Watch

这通常意味着要支付额外的费用才能留在苹果的生态系统中，但有一种方法可以绕过 HomeKit 的限制。只需要一个叫做 Homebridge 的程序和一点编码。

### 什么是 Homebridge，它是如何工作的？

Homebridge 是运行在 [Node.js](http://www.lifehacker.co.uk/2015/03/06/comprehensive-guide-node-js-iot-development) 上的服务器。顾名思义，它充当了苹果 HomeKit 和其他设备之间的桥梁。还支持T5】if TTTT7】。

这使得 homebridge 非常适合通过苹果的 Home 应用程序控制所有智能家居设备。一位 Reddit 用户 [建议](https://www.reddit.com/r/apple/comments/7ftpmo/homebridge_raspberry_pi_aliexpress_the_cheapest/?st=jaicgoxl&sh=5ff630cf) 购买小米的廉价智能插头，把你的整个家变成一个智能房子。基本上，任何不直接与苹果软件一起工作的东西都应该从这个变通办法中受益。

一个很大的缺点是，你可能会让自己暴露在黑客和其他风险面前。如果想要获得 HomeKit 的批准，苹果要求每台设备都要经过大量测试，并遵循严格的安全规则。这可能会限制被批准的设备的数量，但也意味着你不必太担心安全性。Homebridge 也是开源的，所以你要依靠一个松散的开发者社区来更新它，而不是像苹果这样值得信赖的公司。

### **如何安装 HomeBridge**

如果你家里有一台一直运行的 Mac 电脑(比如台式电脑或者兼做媒体播放器的 Mac Mini ),那可能是最好的选择。 [iMore](https://www.imore.com/how-connect-non-homekit-devices-homekit-using-homebridge) 有在 macOS 上安装 Homebridge 的详细指南。只是别忘了先备份你的电脑，以防出错。

如果你手头没有 macOS 电脑，也可以在 Windows 上安装 home bridge[。但同样，您需要确保这是一台始终运行软件的电脑。](https://github.com/nfarina/homebridge/wiki/Install-Homebridge-on-Windows)

如果你还没有一台运行 Homebridge 的电脑，最好的选择可能是买一台便宜的 [树莓派](https://lifehacker.com/top-10-raspberry-pi-projects-for-beginners-1791002723)T3】电脑，把它作为你的中枢。在这种情况下， [Github](https://github.com/oznu/docker-homebridge/wiki/Homebridge-on-Raspberry-Pi) 会一步一步地引导你完成这个过程。