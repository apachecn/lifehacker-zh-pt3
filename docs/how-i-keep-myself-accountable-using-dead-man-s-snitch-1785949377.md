# 我如何用死人的告密者来让自己负责

> 原文:[https://life hacker . com/how-I-keep-I-self-accountable-using-dead-man-s-snick-1785949377](https://lifehacker.com/how-i-keep-myself-accountable-using-dead-man-s-snitch-1785949377)

说到要完成的事情，我是一个列清单的人，以至于我的清单上都有清单。但是如果我忘记了一项任务，谁来让我负责或者提醒我呢？我从我们的开发者那里获得了一些灵感，用 Todoist，Zapier 和 Dead Man 's Snitch 设置了一个警报。

Watch

*本帖原载于* [*集体想法博客*](http://collectiveidea.com/blog/archives/2016/08/26/keeping-on-task-using-dead-mans-snitch/) *。*

这里只是我众多清单中当前项目的一个例子

*   把我汽车后备箱里的衣服带到慈善机构
*   修习
*   给狗洗澡
*   打电话给奶奶制定晚餐计划
*   为个人博客集思广益
*   应聘成为 [逃亡中的女孩](https://www.girlsontherun.org/) 蔻驰

正如你所看到的，这些项目中的一些并没有真正的截止日期，只是需要完成。我想确保我能继续处理我那长得吓人的清单，所以我告诉自己每周至少要从清单上划掉一项。但是当我忘记做那件事的时候会发生什么？

嗯，这是我从办公室里的天才开发人员那里获得一点灵感的地方。他们中的许多人经常使用 [死人的飞贼](http://www.deadmanssnitch.com/) ，这是我们在 [集体创意](http://collectiveidea.com/) 的产品之一，用于监控像 cron jobs(Unix/Linux 环境中的调度任务)或[Heroku Scheduler](https://elements.heroku.com/addons/scheduler)这样的周期性任务。死人的告密者是如何工作的，你为每一个你想要监控的工作、任务或过程设置一个“告密者”。每个告密者都有一个与之关联的 URL，每次所述过程发生时，该 URL 都会被查验。如果告密者没有登记，你会收到一个提醒，让你知道这件事。

为了让死人的飞贼工作，我需要一个飞贼设置来提醒我，如果我们每周忘记在我的待办事项列表中标记一项任务。这就是扎皮尔 的用武之地。Zapier 有几个连接到它的待办事项应用程序，在看完所有程序后，我决定使用 [Todoist](https://todoist.com/) 。

### 如何设置每周提醒

所以，为了开始，我们需要做的第一件事是在 Zapier 上创建一个新的“Zap”，点击“Make a Zap！”在那里，它会要求你“选择一个触发应用程序”,这就是你要搜索 Todoist 的地方。这是因为 Todoist 将会是一个触发器，每当你从待办事项列表中标记一个项目时，它就会 pings 你的告密者的 URL。

选择 Todoist 作为触发 App 后，选择“新完成任务”作为实际触发。每当一个新任务完成，扳机就被击中。

出现提示后，连接您的 Todoist 帐户并加载您的项目(或者换句话说，您想要标记的内容列表)。您应该会看到 Todoist 帐户中所有列表的下拉菜单。我只有一个叫“私人”的。

下一个窗口将要求您“通过获取一个现有的完整任务来测试您的 Todoist 触发器。”这就是事情变得有点不稳定的地方。回到 Todoist 应用程序，在列表中添加一个测试项，然后将该测试项标记为完成。

现在回到你在 Zapier 的 Zap，点击“获取并继续”。如果工作正常，它会说“测试成功！”

现在，我们需要添加“扎皮尔的 Webhooks”动作；你需要选择“获取”选项。这就是每次触发(Todoist 列表中正在完成的一项)时 ping 我们的告密者 URL 的原因。

接下来，它会要求您提供一个 URL。那是你要放金色飞贼的地方，所以让我们直接到 [死人的金色飞贼](https://deadmanssnitch.com/) 来创建它。

我将我的任务命名为“从你的待办事项列表中检查一项”，并将间隔设置为每周一次，因为如果我未能完成任务，我希望每周都能收到提醒。点击“保存”。

现在，你将得到你唯一的告密者网址。

让我们复制那个 URL 并返回到 Zapier，在那里您将把 URL 粘贴到 Zap 中。

本质上，我们刚刚做的是，我们说，“好的，每次完成一个 Todoist 项目，使用 Webhooks 点击这个 URL(我们的告密者)。”如果网址每周都被点击，死者的告密者认为这是成功的。如果它没有被命中(即，我没有完成一周的至少一项)，死人的告密者会看到这一点，并会给我发电子邮件告诉我丢失的检查。

接下来，您将想要测试一切。点击“保存并继续”，扎皮尔将 ping 金色飞贼，让你知道测试是否成功。此外，在同一时间，你会收到一封电子邮件，从死者的告密者，让你知道你的告密者是正确的报告，在第一次。

我在 Zapier 设置了另一个金色飞贼，它使用 [MapMyFitness](http://www.mapmyfitness.com/my_home/) 和 Webhooks 来提醒我是否忘记每天跑步。我现在正在为马拉松训练，同时也在尝试[#连续跑](https://www.hashatit.com/hashtags/runstreak) ，所以我希望这种组合能让我保持诚实！

|集体想法

萨沙·沃尔夫毕业于卡尔文学院，获得电影研究学位。她从事过电视新闻、社交媒体、自由写作、内容营销、摄影和视频工作。高中时，她在杂货店当装袋工，并参加了地区装袋比赛。T3】

<small>*形象由*</small>[<small>*blossomstar*</small>](http://www.shutterstock.com/pic-266537561/stock-vector-business-to-do-list.html)<small>*(*</small>[<small>*Shutterstock*</small>](http://shutterstock.com)<small>*)。*</small>