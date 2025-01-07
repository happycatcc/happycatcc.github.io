---
layout: post
title: 德国17岁高中生制作疫苗预约爬虫网站，用户超3千万
categories: [ Life in Germany ]
author: CC猫饲养员1号

image: assets/images/impftermin.png
toc: true
---

最近德国COVID疫苗打得火热，超过40%的人口已经完成了第一针，我这种没有优先级的普通人也可以在网上刷疫苗预约了。随着政府的一系列针对打过疫苗人群的开放政策：逛宜家，在餐馆吃饭，和朋友聚会，去游泳馆，泡温泉……疫苗一针难求啊。

### 疫苗预约Automation

既然可以网上预约，那当然可以把这个过程自动化：首先想到的是Python + Selenium。GitHub搜索一下，已经有了数个star很高的Repo。
分享住在以下几个州的朋友们：BADEN-WÜRTTEMBERG，BRANDENBURG，HAMBURG，NIEDERSACHSEN，SACHSEN，SACHSEN-ANHALT，THÜRINGEN。

1. TobseF/impf-bot 
   <a class="smoothscroll" href="https://github.com/TobseF/impf-bot">github.com/TobseF/impf-bot</a> kotlin/java + Selenium
2. alfonsrv/impf-botpy
   <a class="smoothscroll" href="https://github.com/alfonsrv/impf-botpy">github.com/TobseF/impf-bot</a> Python + Selenium
3. iamnotturner/vaccipy 
   <a class="smoothscroll" href="https://github.com/iamnotturner/vaccipy">github.com/TobseF/impf-bot</a> Python + Selenium

前两个我都试用过，文档也给出了特别详细的步骤，非技术人员也能上手。甚至还给出了dockerfile，如果有闲甚至可以做到完全自动化，扔到pipeline里跑。

### 接种预约爬虫

**impfterminradar**，每隔3-5分钟call一次API，可以看到所有接种中心是否有空位。上班的时候打开网页，勾选附近的接种中心，听到铃声赶快点预约就能拿到预约疫苗的code。

网址：<a class="smoothscroll" href="https://impfterminradar.de/?state=baden_wuerttemberg">impfterminradar.de</a>

**impfterminübersicht**，这个就神奇了，除了可以看到当前哪些接种中心有空位，还可以看到每个接种中心在过去7天是什么时间放出预约的。更神奇的是，我好奇的查了下作者，居然是个17岁的德国高中生。

网址：<a class="smoothscroll" href="http://impfterminübersicht.de/">impfterminübersicht.de</a>

17岁的朱利安·安布罗齐（Julian Ambrozy）住在斯图加特附近，是一名11年级的中学生。为了帮助爷爷约到疫苗，他在复活节假期制作了这个网站。他说，“我想为祖父找到一个疫苗接种预约，有时我坐在电脑前，直到凌晨1点才能等到预约。”

<img src="{{site.baseurl}}/assets/images/impf-Julian-Ambrozy.jpg" alt="drawing"/>
*Julian Ambrozy坐在他的写字台前 @Private*

安布罗奇的问题是，巴登-符腾堡州，勃兰登堡州，汉堡，萨克森-安哈尔特州，黑森州和北莱茵-威斯特法伦州的接种中心门户网站未发布何时可以找到预约的概览，这显然是出于对疫苗接种旅游的恐惧。如果要在Impfterminservice.de页面上查找可用的预约，则需要相当多的点击和等待。

因为这个混乱的预订系统，安布罗秋在复活节假期期间编写了一个程序，该程序每隔几分钟就会读取一次接种中心网站，并一目了然地显示免费预约时间。经过30多个小时的工作，安布罗奇为他的祖父完成了impfterminübersicht网站。目前，它提供约100个疫苗接种中心的约会信息。

30多个小时的Youtube自学和编程，对安布罗奇来说非常值得，他的爷爷已经完成了第一针的接种。

安布罗奇的上一条Twitter显示，他刚刚发布了impfterminübersicht​的安卓的beta版本。而他正准备购买一台MacBook，开发iOS版本的​app。

江山代有才人出。想想我17岁的时候，高二，还在题海战术呢。

祝大家早点打完疫苗，健康的享受夏天的好时光。