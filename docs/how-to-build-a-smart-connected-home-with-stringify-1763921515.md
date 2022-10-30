# 如何用 Stringify 打造智能互联家居

> 原文：<https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515>

投资智能互联设备(如 Wi-FI 变色灯泡、可上网的电源板和 Fitbits 等可穿戴设备)的问题是，你需要一打应用程序来满足所有需求。 [Stringify](https://www.stringify.com/the-app/) 是一个 iPhone 应用程序(Android 即将推出)，它将所有这些连接在一起。想象一下:用一个应用程序来管理它们，用一个应用程序来自动化它们。下面是如何设置它。

Watch

### Stringify 是如何工作的

如果所有这些关于“自动化”的谈论听起来很熟悉，那是因为 Stringify 类似于我们喜欢的另一个服务，[If This Then](https://ifttt.com/)。可以把 Stringify 看作是 IFTTT 的一个更加可定制的版本，更像是， *If This，This，This，Then That。它的目的有两个:管理智能电器和互联网连接的设备，并自动让它们做你想让它们做的任何事情。*

Stringify 支持大量不同的服务和物理设备，所有的 [你都可以在应用的下载页面](https://itunes.apple.com/us/app/stringify/id1012539039?mt=8) 找到。你可能认识[Fitbit](https://www.fitbit.com/)[Philips Hue 灯泡](http://www2.meethue.com/en-us/about-hue/what-hue-does/?&origin=|mckv|s6gmIoLVP_dc&pcrid=78454519236|plid|&gclid=Cj0KEQiAsP-2BRCFl4Lb2NTJttEBEiQAmj2tbS8lXZSYKEn4dBy6IEnv27Ojs6C5P2Pt0Ztatx8EBW8aAmX18P8HAQ)[Nest devices](https://nest.com/)[net atmo devices](https://www.netatmo.com/)，以及类似 [Google Drive](https://www.google.com/drive/) 、RSS feeds、 [Reddit](https://www.reddit.com/) 、[Slack【t3t 我个人测试 Stringify 用的是一个](https://slack.com/) [亚马逊 Echo](http://www.amazon.com/gp/product/B00X4WHP5E/ref=ods_xs_ae_shurl?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515&asc_source=&hvadid=84472872905&hvdev=c&hvexid=&hvnetw=g&hvpone=&hvpos=1t1&hvptwo=&hvqmt=b&hvrand=15142381587517795018&ref=pd_sl_202q10xm53_b&tag=kinjalifehackerlink-20) ， [LIFX 灯泡](http://www.amazon.com/LIFX-Original-Multicolor-Adjustable-Dimmable/dp/B00EJ9FY2C?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515&asc_source=&tag=kinjalifehackerlink-20) ，一个 [自动](http://lifehacker.com/automatic-tracks-your-driving-and-your-car-to-save-you-1453393979) 车载适配器，[Misfit flash link](http://www.amazon.com/Misfit-Wearables-Activity-Tracker-Button/dp/B011HT9AEY/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515&asc_source=&ie=UTF8&keywords=misfit flash link&qid=1457546314&sr=8-1&tag=kinjalifehackerlink-20)，一个 [古怪的 Pivot Power Genius](http://www.amazon.com/Quirky-PPVG-WH01-Pivot-Power-Genius/dp/B00GN92MC6/ref=sr_1_1?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515&asc_source=&ie=UTF8&keywords=pivot genius&qid=1457546351&sr=8-1&tag=kinjalifehackerlink-20) 插线板。你拥有的联网设备种类越多，Stringify 就越有用。

在 Stringify 中，每个设备都有两种能力:一个触发器或一个动作。触发器是启动自动化过程的规则。一个动作是，嗯，触发后发生的事情。您可以设置 Stringify，以便多个参数触发一个动作，或者多个动作被触发。这真的取决于你，如果这听起来超级简单，那是因为它是。

例如，你可以设置它，这样当你下午 5 点后到家时，你的 Wi-Fi 灯就会打开，你的 Nest 恒温器就会启动，一个连接的电源板会触发你的电水壶烧水喝下午茶。当然，这有点荒谬，但它使自动化所有那些愚蠢的连接设备变得容易得多，而且令人惊讶地有趣。在他们自己的本地应用或工具中，没有任何编程规则。在这篇文章的最后，我将通过更多的例子来说明你可以用 Stringify 做什么，但是让我们先来完成你的第一个“流”

### 第一步:将所有设备连接到 Stringify

让我们从使用任何这样的应用程序的最乏味、最糟糕的部分开始:批准和设置你的设备。首先，下载 [Stringify app](https://itunes.apple.com/us/app/stringify/id1012539039?mt=8) 并创建账户。接下来，您需要验证您拥有的每台设备。这意味着你必须在每一个你想访问的服务或连接的设备上登录你的帐户。如果你有很多这样的密码，这可能需要一段时间，所以坐下来，打开你的密码管理器，开始使用吧。

1.  点击“事物”选项卡。
2.  点击新建。
3.  在列表中搜索您想要添加的设备或服务。找到后，点击它。
4.  轻按“连接”(您也可以轻按“可用的触发器和操作”来查看 Stringify 在设置之前能够在设备上控制什么)。
5.  如果您连接了一个设备，您将前进到鉴定页面。键入您的设备或服务的用户名和密码以进行身份验证。

现在，您的设备或服务处于 Stringify 中。继续对您想要连接的所有东西重复此过程。

### 第二步:创造你的第一个“心流”

一旦你所有的设备都设置好了，是时候创建你的第一个“流”了流是 Stringify 的自动化规则集。再次，思考“如果这个和这个，那么那个和那个。”

让我们创建一个示例流，如果我在一天中的某个时间点没有达到我的活动目标，它就会关闭我的电视。规则很简单:如果我在家，到下午 6 点我还没有达到每天的活动目标，那么就关掉电视的插座。我知道这很苛刻，但你必须做你必须做的事情来激励你去锻炼，对吗？

1.  在 Stringify 的主屏幕上，点击流量>新建。在这里，欢迎您的是主流程设计屏幕，称为画布。点击“+”添加一些设备。
2.  在“选择项目”菜单中，点击您想要包含在流程中的所有设备或参数，完成后点击“添加”。对于我的例子，我正在使用位置(通过我的手机上的 GPS 定位我的物理位置)， [Misfit Flash Link](http://www.amazon.com/Misfit-Wearables-Activity-Tracker-Button/dp/B011HT9AEY?asc_campaign=InlineText&asc_refurl=https://lifehacker.com/how-to-build-a-smart-connected-home-with-stringify-1763921515&asc_source=&tag=kinjalifehackerlink-20) 健身追踪器，以及 [Pivot Power Genius](https://www.quirky.com/invent/243972) 电源板。
3.  您添加的所有项目现在都在屏幕底部的面板中，点击、按住并拖动它们，以大致的使用顺序将它们移动到画布上的圆圈中。把触发器放在左边，动作放在右边。在我的例子中，位置和不匹配在一列，电源在第二列。

一旦画布设置完毕，您需要配置每个参数。

### 第三步:设置你的触发器和动作

将每个项目拖到画布后，您会注意到一个旋转的齿轮图标。这意味着在您可以使用该项目之前，需要设置某种类型的参数。请记住，每个项目只能做两件事之一:触发某事或执行一个动作。例如，如果您使用位置触发器，您需要选择哪个位置触发动作。下面是设置参数的方法:

1.  用旋转齿轮图标点击其中一个图标。在本例中，让我们点击 Pivot 图标来设置流程中的操作。
2.  点击要启用的触发器或操作。对于枢轴，我将它设置为“关闭插座 1”，因为这是电视的电源。
3.  对画布上的所有项目重复这个过程。

回到我的例子，我这样设置它:

*   地点:如果我在一个地点(家)。
*   不适应:如果每日目标在下午 6 点前没有实现
*   Pivot Power Genius:关闭插座 1(电视)

您可以在这里尝试许多不同的参数，所以在设置这些参数时，请不要着急，这样您就可以确切地了解每款设备的功能。

### 第四步:把所有东西连接起来，打开所有东西

一旦为流程中的所有设备或服务设置了所有参数，就该将所有内容链接在一起了。要将触发器链接到动作，只需将手指从触发器拖动到动作。

当您有多个触发器或多个操作时，事情会变得有点复杂。例如，在我们的例子中，我们希望在行动发生之前满足两个参数:我需要在家*和*我需要错过我的活动目标。为此，将手指从一个触发器(在我们的示例中，这是位置触发器)拖动到动作(枢轴)并放开。如果连接成功，您会看到一个黄色链接图标出现。如果没有，链接图标是红色的，这意味着某处有冲突。如果一切正常，那么将手指从第二个触发器(在我们的例子中是 Misfit)拖动到刚刚出现的链接图标。这将两个触发器联系在一起。您可以重复这个基本过程，将任何操作或触发器链接在一起。

创建完所有链接后，点击顶部的框来命名您的流，然后点击启用流框来启用它。恭喜你！你刚刚完成了你的第一个流程。

### 有用流程的一些附加示例

好了，我们已经完成了用一组非常基本的参数创建一个简单流程的过程。但是，就像 IFTTT 一样，你能用它做什么真的只受你想象力的限制。Stringify 在他们的网站 上列出了许多想法，让你的头脑风暴活跃起来，但这里有一些我个人最喜欢的。

*   [**在黑暗中，照亮道路**](https://www.stringify.com/flowideas/when-in-dark-light-up-the-way/) :设置一个支持的运动探测器，在夜间寻找运动。当它感觉到什么时，你的灯就会变暗。这对于那些深夜去浴室或客厅检查你是否锁门的人来说是很棒的，在那里你不想因为把灯开到最大亮度而被弄瞎。
*   " [**锻炼**](https://www.stringify.com/flowideas/workout/) :"这使用亚马逊的 Alexa 作为触发器，所以当你说，" Alexa，告诉 Stringify 运行锻炼"，你的家庭健身房就会亮起，音乐开始播放，你的锻炼记录在谷歌日历中。然后，定时器被设置为一个小时。一小时后，一切都会关闭。
*   [**离家上班**](https://www.stringify.com/flowideas/leaving-home-for-work/) :这是我见过最疯狂(但还是有用)的一个。它是这样设置的，当你在工作日的早上 7 点到 8 点之间离开房子时，所有的插座都会关闭，两种不同品牌的灯都会关闭，任何音乐都会暂停，一组调光开关也会关闭。当这一切都完成后，你会收到一个通知，告诉你你的“房子被关闭。”
*   [**易醒**](https://www.stringify.com/flowideas/easy-wake-up/) :此流好饮茶。当工作日的早上 5:45 时，一个支持的灯泡慢慢变暗，连接到电热水壶的 Pivot Power Genius 插座开始为您的晨杯烧水。

当然，这里有数不清的其他变化，如果你改变时间或更换特定设备，其中一些甚至可以用于其他目的。慢慢来，尝试各种设置，尝试不同的动作。你永远不知道，你可能真的会为你已经拥有的设备找到完美的“智能家居”组合。

[Open *kinja-labs.com*](http://kinja-labs.com/related-widget/?posts=510246491,1640844965,1660175128&title=Connect It All)

* * *

<small>*联系作者在*</small>[<small></small>](mailto:thorin@lifehacker.com)*<small>*。*T15】</small>*