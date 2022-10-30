# 从 Chrome 地址栏映射任何内容

> 原文:[https://life hacker . com/map-any-from-the-chrome-address-bar-1797731855](https://lifehacker.com/map-anything-from-the-chrome-address-bar-1797731855)

在桌面上用谷歌地图查找路线有点笨拙。你必须选择出发地点、目的地和交通方式。但是如果你在 Chrome 上，你可以建立三个快捷方式来直接从地址栏获得方向，而不需要点击一下。

Watch

### **绘制任意位置的地图**

在 Chrome 中，进入“设置”，然后选择“管理搜索引擎”在“其他搜索引擎”旁边，点击“添加”像这样填写表格:

*   搜索引擎:`Google Maps`

*   关键词:`map`

*   在查询位置带有%s 的 URL:[`https://www.google.com/maps/place/%s`](https://www.google.com/maps/place/%s)

点击保存。从现在开始，你可以在地址栏中输入“地图”和一个位置，谷歌就会绘制地图。比如:`map 11 Wall St, New York, NY`:

URL 中的`%s`是您在关键字后输入的任何内容的占位符。

### **来自家的方向**

对于从你家到任何地方的路线，你也可以做同样的事情。如上添加一个新的搜索引擎，但是使用这个 URL，用你的家庭地址代替我们的示例地址:

`http://maps.google.com/maps?f=d&source=s_d&saddr=11+Wall+St,+New+York,+NY+10005&daddr=%s`

给这个搜索一个新的关键字，比如`mh`或者`maphome`。

您可以根据自己的喜好创建任意多个关键词，每个关键词指定一个不同的起点，比如您的工作或您经常旅行的任何地方。

### **回家的方向**

以上所有内容都适用，但请从以下字符串开始:

`http://maps.google.com/maps?f=d&source=s_d&saddr=%s&daddr=11+Wall+St,+New+York,+NY+10005`

### **公交/自行车/步行路线**

谷歌地图经常试图猜测你理想的交通方式。添加以下字符串之一以获得特定模式的结果:

*   驾驶:`&dirflg=d`

*   公交:`&dirflg=r`

*   骑车:`&dirflg=b`

*   行走:`&dirflg=w`

你可以在 Chrome 的地址栏中建立一系列快捷方式 ，包括专门的书签、图片搜索和特定网站搜索。坚持下去，你将永远不需要把手从键盘上拿开。