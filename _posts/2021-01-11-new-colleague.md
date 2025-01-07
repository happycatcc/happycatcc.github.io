---
layout: post
title: 新年来了个新同事，我们是这样帮她onboarding的
categories: [ Working in Germany ]
author: CC猫饲养员1号

image: assets/images/new-colleague-onboarding-title.png
---

新年来了个新同事，从其他stack转过来。记录下我们是如何帮助一个对我们的stack不熟悉的新人onboarding的，希望能帮助到到新入职的朋友们呀。

> 我们小组的tech stack：Microservice （公司自己造的前端框架/JS + Node.js，SQL，Kafka），Git，CI/CD
> 其实就是个普通的用JavaScript写microservice的小组

### Brainstorming

这天的daily scrum提前结束，architect提议大家一起想一想onboarding需要做什么。我们就在一个online white board上写了一大堆posts。

![drawing](/assets/images/new-colleague-brainstorming.png)
*大概就是这样，把所有想到的东西都写上去*

比如前年从Java转Node.js的时候大家一起学的网课，一次如何从0建立新repository的pair programming，一个了解小组test strategy的session，需要一个同事帮忙授予新同事所有开发工作需要的权限。

### Prioritizing

有些topic虽然需要了解，但是用到的时候再学就好了。在我们这个小组里，对新同事来说最重要的topic是学习JavaScript，学会使用Git，理解我们的Test Strategy和Test-driven development（TDD）。

其他的Topic，比如Messaging和Kafka，可以在以后遇到的时候通过pair programming快速上手。

### Action Items

![drawing](/assets/images/new-colleague-onboarding.png)
*优先级和atcion items*

新同事在前两个月预计都不会有什么产出，但是学习也是工作的一部分嘛。
- 我们帮她在JIRA board里建立了她的学习task，方便她tracking自己的进度。
- 需要同事帮忙setup或者授予权限的地方，建立task，发送meeting request来block时间。
- 下周刚好有同事做在新的micro service里initialize messaging service的工作，block时间，和新同事一起pair programming。

### Others

小组建立两年，期间也陆续有同事加入。我们已经有了一套比较完整的wiki：如何设置IDE的plugin，什么是test strategy，大家一起学过的网课链接和介绍，去年刚刚学习messaging时候的学习笔记和录制的roll out session。

这些文档不仅能帮助新同事，在自己需要查询复习的时候，也很有帮助。