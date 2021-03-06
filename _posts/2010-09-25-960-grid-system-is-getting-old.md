---
layout: post
title: 960px宽的网格已经过时了？
date: 2010-09-25 09:52
comments: true
categories: [CSS]

---

这是最近发表在<a href="http://www.webdesignerwall.com/">Web Design Wall</a>上的一篇文章，作者在为<a href="http://themify.me/">Themify</a>设计主题的时候摒弃了传统的960px，大胆采用了自己的978px宽的网格。初看可能会觉得这个数字比较荒谬，不过想想我们的1024px宽的屏幕也会让不熟悉计算机原理的人觉得荒谬不是么？仔细阅读文章之后我发现这个宽度十分适合国外的13像素英文字体。而这个宽度是否适合国内中文字体的布局呢？请在本文后面留言。

另外，除了翻译原文内容以外，还还翻译了四天来原文上一些有建设性的评论。

以下是译文。
<!--more-->
这几年来960px宽的网格系统（http://960.gs）一直是设计师最爱的结构和布局框架。随着屏幕分辨率越来越大，我发现960px不再适合我的需求了。20px的gutter（译者注：槽，关于网格的基本知识，见本站的另一篇文章，<a title="Permanent Link to css框架[4]-blueprint" rel="bookmark" href="http://yuguo.us/weblog/css-framework-blueprint/">css框架[4]-blueprint</a>）和940px的内容显示区对于现在的web来说有点窄了。在设计<a href="http://themify.me/">Themify</a>的时候，我发现另一个网格系统也能很好地满足我的需求。如果你从来没听说过960，我将在下文介绍它，连同我的新网格。
<h2>关于960网格系统</h2>
960gs特点如下
<ul>
	<li>总共宽度 960px</li>
	<li>12 栏，每栏 60px</li>
	<li>每栏有左右各10px边距，也就是20px的gutter</li>
	<li>内容展示区宽度为940px</li></ul>
960网格是非常好的网格系统，因为它十分灵活。它允许设计师把页面分成以下数量的网格：9 x 3, 3 x 3 x 3, 4 x 4 x 4 x 4, 10 x 2等等……960gs可能是最受欢迎的网格系统，已经在大量页面中使用了。
<h3>问题是？</h3>
960网格的问题是gutter的宽度和内容的宽度。减去960px两边的margin（两边的gutter叫做margin），实际上的内容显示区域只有940px，这在往日可能没有关系，因为那时候文字是12px的，而现在很多站点的文字是13px的（译者注，中文博客的很多站点也开始使用14px的正文）。既然文字变大了，你不认为应该增大gutter宽度和内容宽度吗？
<img class="aligncenter size-full wp-image-275" title="960gs" src="http://yuguo.us/files/2010/09/960gs.gif" alt="960gs"   /><h2>978网格</h2>
我用在<a href="http://themify.me/">Themify</a>上的网格是978px，12栏，每栏54像素，30px gutter。我发现它在1024x768px的显示器上显示十分完美。<em>去掉了左右边距</em>用来最大化内容区宽度。并且我增加了gutter的宽度到30像素，所以你的内容有更多呼吸的空间。效果如下：
<img class="aligncenter size-full wp-image-276" title="978-grid" src="http://yuguo.us/files/2010/09/978-grid.gif" alt="978-grid"   /><h2>以下是原文后的评论</h2>
（集中翻译关于960gs和978gs的评论，灰色部分为我的评论）：
<a rel="external nofollow" href="http://www.surrealtopia.com/">negativeboy</a>：或许在“创作型”项目上，960像素缺少灵活性，但对于需要在小栏目上有更多掌控的项目来说，960仍然是一个很好的选择。<span style="color: #888888;">（我想他说的是yahoo和Facebook那种类型的，而不是个人主页吧）</span><a rel="external nofollow" href="http://gr8pixel.com/">gr8pixel</a>：我个人仍倾向于960.gs。但是如果看看屏幕分辨率的统计数据，76%的用户在使用1027x768或者更噶的分辨率。65%的用户使用1280或者更高。所以，我想我们是应该跟随潮流，把我们的字体变得更大，然后开始流动布局……当然了，还有更大间距。
<a rel="external nofollow" href="http://www.chinesenewyear.me/">chinese new year</a>：去掉左右边距是一个糟糕的主意……<span style="color: #888888;">（我注意到是他的域名）</span>
anon：我一般看项目了，但我会确保条目之间gutter使用一致的宽度，另外我的最大宽度也不会超过1024px。
<a rel="external nofollow" href="http://www.twitter.com/kailashiyer">kailash</a>：我认为坚守一种网格不是一个好主意。
<a rel="external nofollow" href="http://www.refreshcreations.co.uk/">Ryan Carson</a>：Pick what suits the design, design how you want to design, it’s all fine.<span style="color: #888888;">（这个是押韵帝，我就不翻译了）</span><a rel="external nofollow" href="http://twitter.namklabs.com/">Nick</a>：哦，楼主你的意思是解决办法是增加<em>18像素</em>？这跟头发丝一样的宽度还用拿出来说？我没看出来这个解决办法有何亮点。<span style="color: #888888;">（我想你没认真读，增加的可不止是18哦，是18+20。此外作者的gutter宽度也变成了30像素，目的是更适合更大字体。）</span><a rel="external nofollow" href="http://blog.antarestrader.com/">John F. Miller</a>：是的我认为太窄了，我还认为<em>12栏是一个错误的数字</em>，我喜欢黄金比例，所以我更喜欢13栏（5|8）和25栏（8|13）。<span style="color: #888888;">（这哥们很有想法，我还点去他页面看他的设计，结果发现是个程序员，博客也很难看 :(）</span><a rel="external nofollow" href="http://www.ill-fx-designs.com/">Allen</a>：我用过960gs，现在在用24栏，已经习惯了，也不准备学习新的框架。我还是坐等你未来用978做出更多的作品吧。<span style="color: #888888;">（这应该代表很多人的心声吧）</span><a rel="external nofollow" href="http://www.imenn.com/">iMenn</a>：爱死了13像素字体和30像素宽gutter，读起来很舒服 :)
<a rel="external nofollow" href="http://prop-14.com/">Randy</a>：我也考虑过使用框架，可是我的工作都是从设计师那里取得PSD然后做成WordPress主题，很多设计师（我的意思是，<em>很多！</em>）都不知道960gs是神马，他们创作出完全自由的设计，我杯具。此外太多新手依赖CSS框架，在他们理解float:left之前。
<a rel="external nofollow" href="http://taimar.ee/">Taimar</a>：楼主，你仍然可以在960gs的栏宽和gutter的基础上增加内容快点，方法是增加栏的个数。以1280屏幕为例：

960 + 80 = 1040

960 + 2*80 = 1120

960 + 3*80 = 1200
<span style="color: #888888;">（同学算的不错，可是楼主的目的还是：1.需要支持最小1024屏幕2.增大gutter）</span>
Jib - UpShot：我正在做的一个系统很上流，是用html5做的，用户也都是设计师，他们的屏幕挺大。那些小于1024屏幕的用户也基本上是使用IE6的用户，反正无论如何他们都浏览不了什么，下面出现滚动条也没什么吧。<span style="color: #888888;">（so they don’t have sugar anyway）</span><a rel="external nofollow" href="http://leonpaternoster.com/">Leon</a>：我认为你的逻辑错了，960gs是基于这么一个事实：960像素宽的画布最适合现在的桌面显示器，960并不是根据12像素的字体来设定的，没有什么能阻止你在……比如说760像素宽的屏幕上使用13像素字。

我认为960这个数字的产生是因为它能更灵活地适应更多的设备（特别是移动设备），增加额外的38像素没什么区别。
<a rel="external nofollow" href="http://www.kamilos.net/">Kamil</a>：我使用一个1000像素的grid，它在1024的屏幕上工作良好，24像素足以容纳一个滚动条，例子：<a href="http://www.evestyle.com.pl/">http://www.evestyle.com.pl/</a> <span style="color: #888888;">（抱歉，我用Chrome模拟的1024宽屏幕显示了水平滚动条）</span>。
<a rel="external nofollow" href="http://john-m-sullivan.com/">John Sullivan</a>：希望看到流动布局的24格。<span style="color: #888888;">（可能会不稳定）</span><a rel="external nofollow" href="http://ivanasetiawan.com/">Ivana Setiawan</a>：960像素并没有“过时”，有些“过宽”的设计看起来就好像要摔在你脸上一样。
<a rel="external nofollow" href="http://www.webdesignerwall.com/trends/960-grid-system-is-getting-old/comment-page-5/www.d3sign-worx.com">Tom</a>：我想“960像素已经老了”这种言论略显误导。事实上960gs是一个相当成功的框架，这可能就是你认为的“老了”。很多人都在使用这种框架快速上手和设计，而框架作者并没有强迫你去用它。楼主你想说的意思是：<em>960gs不能满足所有的需求</em>，而设计师使用何种框架来辅助自己设计，这是设计师的自由选择。<span style="color: #888888;">（我想楼主标题在逻辑上不严谨，可能是为了吸引眼球和评论，他想表达的实际上是：Another option for bigger screen/font-size: 978 grid system）</span><a rel="external nofollow" href="http://www.redletterstrategies.com/">Red Letter</a>：有趣的文章，事实上，如果使用978像素网格+30像素gutter的话，单位空间能写的内容更少了。<span style="color: #888888;">（确实如此，不过展示更多的内容完全不是我们的目标）</span><h2>你认为呢？</h2>
留下你的评论吧。

