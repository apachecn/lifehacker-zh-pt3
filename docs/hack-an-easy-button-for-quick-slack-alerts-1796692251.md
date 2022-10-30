# 破解一个“简单”按钮，快速发出松弛警报

> 原文：<https://lifehacker.com/hack-an-easy-button-for-quick-slack-alerts-1796692251>

戴着耳机工作通常意味着你不想被打扰，但有时也意味着你只是在工作时听点东西。如果你想在罐头打开的情况下还能保持在线，为什么不自己设计一个提醒按钮呢？

Watch

开发人员 [Nick Sypteras](https://www.nicksypteras.com/projects/easy-button-desk-alert-hack) 想解决同事在他戴着耳机时请求他注意的问题。在一个小隔间里工作，他写道，“除了在我面前挥动他们的手，在我身后制造很大的噪音等等，没有任何方法能让我注意到我。”所以他拿出了烙铁、一个 Staples Easy 按钮和一个 Adafruit 微控制器。

<aside class="sc-1rh3ayr-6 eaNzNC inset--story branded-item branded-item--lifehacker" data-commerce-source="inset">[![Image for article titled Hack an &quot;Easy&quot; Button for Quick Slack Alerts](../Images/aef335eb562a1da6957ce25a574b4aa1.png)](https://lifehacker.com/how-can-i-make-my-cubicle-more-comfortable-and-less-bor-5987607) [###### 如何让我的小隔间更舒适，不那么无聊？](https://lifehacker.com/how-can-i-make-my-cubicle-more-comfortable-and-less-bor-5987607) 

亲爱的 Lifehacker，我注定要被困在一个矮墙小隔间里。我知道 Lifehacker

[Read more](https://lifehacker.com/how-can-i-make-my-cubicle-more-comfortable-and-less-bor-5987607)</aside>

Sypteras 在 [MicroPython](https://micropython.org/) 中编写了发送松弛警报的代码，这是一种为微控制器板设计的编程语言版本。[Adafruit Feather HUZZAH](https://www.adafruit.com/product/2821)微控制器根据按钮是否被按下来监听数值的变化。

通过使用 Slack 的 API ，他能够向一个私人频道发送消息，这个频道是他专门为自己办公桌上的简易按钮创建的。虽然这条消息只是让他知道他有一个访客，但你可以对它感兴趣，并使用 Slack 的 API 将更多信息附加到你的警报中。