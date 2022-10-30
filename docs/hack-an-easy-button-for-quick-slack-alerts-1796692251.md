# 破解一个“简单”按钮，快速发出松弛警报

> 原文：<https://lifehacker.com/hack-an-easy-button-for-quick-slack-alerts-1796692251>

戴着耳机工作通常意味着你不想被打扰，但有时也意味着你只是在工作时听点东西。如果你想在罐头打开的情况下还能保持在线，为什么不自己设计一个提醒按钮呢？



开发人员 [Nick Sypteras](https://www.nicksypteras.com/projects/easy-button-desk-alert-hack) 想解决同事在他戴着耳机时请求他注意的问题。在一个小隔间里工作，他写道，“除了在我面前挥动他们的手，在我身后制造很大的噪音等等，没有任何方法能让我注意到我。”所以他拿出了烙铁、一个 Staples Easy 按钮和一个 Adafruit 微控制器。



Sypteras 在 [MicroPython](https://micropython.org/) 中编写了发送松弛警报的代码，这是一种为微控制器板设计的编程语言版本。[Adafruit Feather HUZZAH](https://www.adafruit.com/product/2821)微控制器根据按钮是否被按下来监听数值的变化。

通过使用 Slack 的 API ，他能够向一个私人频道发送消息，这个频道是他专门为自己办公桌上的简易按钮创建的。虽然这条消息只是让他知道他有一个访客，但你可以对它感兴趣，并使用 Slack 的 API 将更多信息附加到你的警报中。