# 我是如何把简历变成聊天机器人的

> 原文：<https://lifehacker.com/how-i-turned-my-resume-into-a-chat-bot-1775565350>

很明显，机器人有一个时刻。甚至在脸书在他们的开发者大会上发布用于信使 的 [机器人之前，已经有大量的](https://developers.facebook.com/blog/post/2016/04/12/bots-for-messenger/) [投资](https://betaworks.com/botcamp/)[争议](http://fortune.com/2016/03/24/chat-bot-racism/)[批评](http://gizmodo.com/facebook-messenger-chatbots-are-more-frustrating-than-h-1770732045#_ga=1.189639083.1224299049.1454957731) 。所以我想学习如何制作自己的机器人——并让它发挥作用！

Watch

一方面，聊天机器人并不是什么新鲜事。它们自 20 世纪 60 年代以及伊莱扎 的时代就已经存在了。但是突然之间，创建有意义的、个性化的对话的工具很容易大规模部署。我们有 API，持续监控和解析消息相关性的能力，以及用于分发的巨大消息平台——这是人们这些天花费 [大部分时间](http://www.businessinsider.com/the-messaging-app-report-2015-11?IR=T) 的地方。

为了对机器人世界有所了解，我决定试着做一个。

### 介绍 EstherBot:我作为机器人的简历

我的目标是创造一些简单的东西，所以我想我应该解决一个我很熟悉的主题——我自己！

领英简介 在过去十年里没有太大变化。当然，它们比简历更有吸引力，但也没有更吸引人。它本质上只是一个日期、标题和流行语的列表——这对淘汰 90%的候选人来说是完美的。但是一旦你找到了一个感兴趣的候选人，你怎么知道她是否在找工作呢？你如何确定他是否符合*文化*？如果你想看他们工作的例子呢？

我认为机器人可以在招聘过程的这个阶段介入，因为机器人可以很容易地回答重复出现的问题(让我们面对现实吧:招聘人员基本上都问同样的问题)。机器人还可以为简历中的行项目提供更多的背景信息，并让人感觉到某人的个性。有大量关于你自己的信息可以用来帮助你找到更好的机会，比如你的爱好、价值观、地点偏好、你作品的多媒体样本等等。一份简历不能包含所有这些，但是机器人可以。我希望 [EstherBot](http://estherbot.com/) 能够展示我的一些古怪兴趣，并讨论我的个人价值观。

### **寻找不太技术性的解决方案**

我不是开发人员，只知道 HTML、CSS 和 JS 的基本框架，所以我需要找到一个简单的方法来创建一个机器人。像 [Howdy 的 BotKit](http://howdy.ai/botkit/) ， [微软 Bot 框架](https://dev.botframework.com/) ， [Kik Bot Kit](https://dev.kik.com/#/home) ， [Gupshup](https://www.gupshup.io/developer/home) ， [Api.ai](https://api.ai/) ， [Wit.ai](https://wit.ai/) 这样的构建者提供了更多的功能，但由于其技术要求，基本上无法入门。

我*能够很快地使用其他一些消息服务，包括[【TextIt】](https://textit.in/)(我喜欢它的可视化编辑器) [Sonar](https://www.sendsonar.com/) ，并决定使用[**Smooch**](https://smooch.io/)。有几个备选方案——今天创建一个机器人最简单的平台是 [Telegram](https://telegram.org/) ，使用 [机器人平台 2.0](https://core.telegram.org/bots/2-0-intro) 你可以在几分钟内设置一个基本的机器人，这要感谢“ [机器人父亲](https://telegram.me/BotFather) ”*

*我使用 [Smooch](http://smooch.io) 是因为它们可以让跨平台发送图像、gif 和动作按钮变得容易。此外，他们有我需要的关键集成——Twilio(用于短信/彩信)、Messenger、Telegram 和 Slack(用于跟踪对话)。我不想要他们的任何其他集成，但我喜欢我可以改变主意，如果我想的话，可以添加其他平台。*

*在引擎盖下，Smooch 连接了大量其他渠道:Android、iOS、脸书、Shopify、Telegram、WordPress 和网络。你可以接受 Stripe 的付款，或者从一系列其他服务中选择，通过打开 Front、Help Scout、HipChat 或 Zendesk 来简化客户支持方面的工作。由于所有的对话都是自动同步的，并通过 Slack 进行路由，所以每当我的机器人做介绍时，我都可以实时加入并打招呼。*

### *如何制作自己的机器人*

*我对 Smooch [示例代码](https://github.com/smooch/smooch-bot-example) 和 [做了一些调整，简化了指令](https://github.com/esthercrawford/EstherBot/blob/master/README.md) 。即使你不是程序员，也不要被你将使用 GitHub *的事实吓倒。*以下是如何开始:*

1.  *创建一个免费的 [拥吻](http://smooch.io) 账号。使用左侧的下拉菜单创建一个新应用程序。确定要使用的消息传递通道并连接它。在我的例子中，我使用了 Twilio。*
2.  *登录 [GitHub](https://github.com) 进入 [EstherBot](https://github.com/esthercrawford/EstherBot) 。点击“Fork”(这只是意味着你正在将文件复制到你的帐户，以便你可以根据需要编辑文件)。*

*创建这个版本会给你一个基于网络的聊天应用程序。通过 Smooch 内部的一些集成(如 Twilio ),你可以让你的机器人在其他平台上说话，包括 SMS、脸书和 Telegram。接下来我们设置我们新的 Smooch app(这些方向改编自 [Smooch 自己的例子](https://github.com/smooch/smooch-bot-example) ):*

1.  *创建新的 Smooch 应用程序后，转到“设置”选项卡，记下您的应用程序令牌。此外，生成一个新的密钥，并记下密钥 ID 和密钥。*

1.  *从 GitHub 上分叉的 EstherBot 中，将您的应用程序部署到 Heroku。(你会在 [自述](https://github.com/esthercrawford/EstherBot/blob/master/README.md) 中找到部署按钮。)这是一项托管应用程序的服务，所以如果你还没有帐户，就去注册吧——这是免费的。你需要在应用的`SMOOCH_APP_TOKEN`、`SMOOCH_KEY_ID`和`SMOOCH_SECRET`配置设置中指定你的应用令牌、密钥 ID 和密码。*
2.  *你的应用现在应该可以在 Heroku 上运行了，但是你还没有完成。记下 Heroku 应用程序运行的 URL，例如:`https://foo-bar-4242.herokuapp.com`。您需要在 Heroku app `SERVICE_URL`配置变量中指定这一点。你可以在 Heroku 控制面板的*设置* > *下配置变量*来完成。(如果您没有看到已经存在的变量，请添加“Service_URL”作为键，添加您的应用程序的 URL 作为值)。*
3.  *仍然在 Heroku，请确保进入“部署”并连接到您的 GitHub 帐户。然后，从主分支启用“自动部署”(这意味着无论何时你对你的机器人的脚本进行编辑，它将在几秒钟内自动更新和对话)。*
4.  *你应该都准备好了。打开你的 Heroku 应用程序，开始与你的新机器人聊天！*

### *教你的机器人说话*

*现在你有了一个机器人，你需要决定它会说什么。这就是文件 **script.json** 出现的地方。你需要编辑这个文档来让你的机器人说话。*

*点击铅笔图标，在 GitHub 上编辑文档。关键词在左边，机器人的回应在右边。例如，如果用户键入“你好”，那么机器人会说“亲爱的，让我们这样做吧……”*

*对于用户来说，关键字不区分大小写。你唯一不想改变的两个关键词是“连接我”和“断开连接”。“连接我”会关闭自动聊天，因此机器人将停止响应关键词。断开连接将重新打开机器人。此外，最初的脚本以“所以你想了解埃丝特？..."但是你当然会想改变它。可以在 script.js 文件中编辑。*

*不出所料，打造引人注目的对话流真的很难。可能是整个过程中最难的部分。能够添加天赋、阴谋和个性是一种不同于建造机器人的技能。我一开始是在纸上绘制一个对话树，但是如果你的互动更复杂，你应该使用一个更复杂的工具，也许是像 [MindMup](https://www.mindmup.com/) 这样的东西。我使用 [Bot UI 套件](https://bots.mockuuups.com/) 尝试用图像、gif 和按钮让终端用户看到对话的样子。(你可以免费下载我的实际草图文件的来开始。)*

*如果你想用换行符、图像和交互式按钮来定制你的消息，请在 GitHub 上的我的 [自述文件](https://github.com/esthercrawford/EstherBot/blob/master/README.md) 中了解更多信息。*

* * *

*瞧啊。您向互联网添加了另一个机器人。* 

*剧透:我的机器人作为一个招募者正在杀死它。我和各行各业的人聊过天，也把我介绍给了脸书、微软和谷歌的人——还有六个更小的、引人注目的团队。你有什么看法？自从应用商店革命以来， [机器人和对话式用户界面是](http://www.businessinsider.com/evernote-founder-phil-libin-creating-incubator-for-bots-2016-3) 出现的“最令人兴奋”的东西吗？会不会有一天，我们都有机器人充当中介？* 

* * *

*[*<small>埃丝特·克劳福德</small>*](https://twitter.com/EstherCrawford) *<small>是一位热衷于讲故事和设计的产品营销人员。点击</small>*[*<small>Esther bot</small>*](http://www.estherbot.com/)*<small>了解更多。本文改编自 Esther 的</small>* [*<small>原帖上媒</small>*](https://medium.com/life-learning/how-i-turned-my-resume-into-a-bot-and-how-you-can-too-f03847352baa) *<small>。图片由</small>* [<small>*欧文史密斯 via Getty*</small>](http://www.gettyimages.com/license/512138811)<small>*。*T47】</small>*