---
title: 生日快乐
level: HTML & CSS 1
language: zh-CN
embeds: "*.png"
materials: ["Club Leader Resources/*.*","Project Resources/*.*"]
stylesheet: web
..。

# 简介 { .intro}

本课程，我们将通过制作一张你自己设计的生日卡片来学习一些HTML与CSS的基础知识。

<div class="trinket">
  <iframe src="https://trinket.io/embed/html/e996dc0380?outputOnly=true&start=result" width="600" height="450" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
  </iframe>
  <img src="birthday-final.png">
</div>

# 步骤 1: HTML是什么? { .activity}

HTML是  __超文本标记语言__ 的英文缩写, 常用于制作网页。我们一起来看一个例子吧。

## 活动清单 { .check}

+ 你可以在Trinket网站上在线撰写HTML，地址是<a href="http://jumpto.cc/web-intro" target="_blank">jumpto.cc/web-intro</a>。如果你正在进行在线学习，也可以使用下面的嵌入版Trinket。

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/850a678202" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

+ 你可以看到，网站左半部分显示HTML代码，而右半部分则是HTML对应的网页展示。

	HTML使用 __标签__ 来构造网页，你可以在第8行看见如下的HTML代码吗？

	```
	<p>Hi. My name is Andy.</p>
	```

	`<p>`就是一种标签, p是英文中 __段落__ 的首字母. 你可以使用`<p>`来展开一个新的段落并使用`</p>`来结束一个段落。

+ 你还能发现其他标签吗？你也许看到了第9行的`<b>`, b是英文中 __粗体__ 的首字母:

	```
	<b>running</b>
	```

	更多的例子:

	+ `<html>`和`</html>`标记了HTML文档的开始与结束;
	+ `<head>`和`</head>`之间存放CSS之类的内容(我们在后面会学习的!);
	+ `<body>`和`</body>`之间存放网页的主体内容。

	![screenshot](birthday-head-body.png)

+ 将左边的HTML部分做一点改动，点击“Run”你将会看到右边的网页也变化了。

	![screenshot](birthday-edit-html.png)

+ 如果你不想保存当前改动，你可以选择菜单并点击“Reset”，试试看吧。

	![screenshot](birthday-reset.png)

## 保存你的项目 {.save}

__你不需要额外创建一个Trinket账号来保存项目！__

如果你还没有Trinket账号，点击下箭头再点击“Link”，你就可以保存一个地址供下次访问。如果你的页面内容发生了变化，相应的地址也会变化，你需要再做一次同样的操作来得到最新的地址！

![screenshot](birthday-link.png)

如果你已经创建了一个Trinket账号，保存当前页面最简单的方法就是点击页面顶端的“Remix”按钮，当前页面就保存在你的账号中了。

![screenshot](birthday-remix.png)

##挑战: 添加一段 {.challenge}
你可以在页面上已有内容的下方再添加一段文本吗？记住你可以用`<p>`和`</p>`标识新段落的起始与结束。

你的页面看起来应该是这样：

![screenshot](birthday-paragraph.png)

你能在新的段落中添加<b>粗体</b>和<u>下划线</u>的文字吗? 你可以使用`<u>`和`</u>`标签给文字添加下划线。

## 保存你的项目 {.save}

# 步骤 2: 什么是CSS？ { .activity}

CSS是英文中 __层叠样式表__ 的英文缩写, 是用于为网页添加样式使他们看起来更美观的语言。你可以在HTML文档的`<head>`部分像这样将你的页面与CSS文件链接起来:

![screenshot](birthday-css-link.png)

## 活动清单 { .check}

+ CSS中列举了特定标签的所有 __属性__ 。点击'style.css'标签看看你的网页的CSS吧。

	![screenshot](birthday-css-tab.png)

+ 找到如下代码:

	```
	p {
		color: black;
	}
	```

	这段CSS代码为段落定义了一个属性，文本颜色为黑色。

+ 将CSS中的'black'替换为'blue'，你就会发现所有段落中的文本颜色都变成蓝色了。

	![screenshot](birthday-edit-css.png)

## 保存你的项目 {.save}

##挑战: 添加更多样式 {.challenge}
你能将段落的文本颜色变为橙色吗？或者将背景改为灰色？

![screenshot](birthday-more-style.png)

## 保存你的项目 {.save}

# 步骤 3: 制作生日卡片 { .activity}

让我们利用今天学过的关于HTML和CSS的知识来制作自己的专属生日卡片吧。

## 活动清单 { .check}

+ 打开这个Trinket链接： <a href="http://jumpto.cc/web-card" target="_blank">jumpto.cc/web-card</a>，如果你是在线阅读也可以使用下面的嵌入版。

<div class="trinket">
	<iframe src="https://trinket.io/embed/html/90506676c9" width="100%" height="400" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen>
	</iframe>
</div>

如果你不能完全理解全部代码，也不用担心。毕竟这张卡片看起来很单调无聊，所以你将对HTML和CSS做一些改动。

+ 点击卡片正面的按钮，你可以看到卡片打开并显现内部的内容

	![screenshot](birthday-click.png)

+ 找到代码的第13行，就像之前的实例一样，你可以编辑HTML中的任何文字来定制你的卡片。

	![screenshot](birthday-card-html.png)

+ 你能找到机器人图片对应的HTML代码吗？（提示: 就在第16行！）将单词`robot`变为`sun`，你就会发现图片改变了！

	![screenshot](birthday-card-sun.png)

	你可以使用如下的任何一个单词`boy`、`diamond`、`dinosaur`、`flowers`、`girl`、`rainbow`、`robot`、`spaceship`、`sun`、`tea`和`trophy`。

+ 你也可以编辑生日卡片的CSS。点击“style.css”标签，最开始的代码定义了卡片`outside`部分的样式，将`background-color`改为`lightgreen`。

	![screenshot](birthday-card-outside.png)

+ 你还可以改变图片的大小。找到CSS的第29行，将外部图片的`width` and `height`改为`200px` (`px`代表像素)。

	![screenshot](birthday-card-size.png)	

+ 字体也是可以改变的。找到第24行将`font-family`改为`Comic Sans MS`，并将`font-size`改为`16pt`。

	![screenshot](birthday-card-font.png)

	你还可以使用其他字体，譬如<span style="font-family: Arial;">arial</span>、<span style="font-family: impact;">Impact</span>和<span style="font-family: tahoma;">Tahoma</span>。

## 保存你的项目 {.save}

##挑战: 制作一张个性化的卡片 {.challenge}
使用你今天学到的所有关于HTML和CSS的相关知识来完成一张个性化的卡片。可以不局限于生日卡片，想想其他场合会用到的卡片吧！

示例:

![screenshot](birthday-final.png)

## 保存你的项目 {.save}

完成你的卡片后，你可以通过链接或者电子邮件发送给其他人。

![screenshot](birthday-share.png)
