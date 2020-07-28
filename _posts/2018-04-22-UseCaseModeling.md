---
layout:     post
title:      用例建模
subtitle:   实践3
date:       2018-04-22
author:     Hanxu
header-img: img/post-bg-desk.jpg
catalog: true
tags:
    - 系统分析与设计
---

> 第六周

本周学习了用例建模实践相关的知识，以下是第六周的作业内容。

***

# 用例建模-实践3

## 用例建模

- a. 阅读 Asg_RH 文档，绘制用例图。按 Task1 要求，请使用工具 UMLet，截图格式务必是 png 并控制尺寸

![task1](/img/2018-04-22/task1.png)

- b. 选择你熟悉的定旅馆在线服务系统（或移动 APP），如绘制用例图。并满足以下要求：
    - 对比 Asg_RH 用例图，请用色彩标注出创新用例或子用例
    - 尽可能识别外部系统，并用色彩标注新的外部系统和服务
    
![qunaer](/img/2018-04-22/qunaer.png)

- c. 对比两个时代、不同地区产品的用例图，总结在项目早期，发现创新的思路与方法
    
    在项目早期，对已有并可应用的现代科学技术手段做一个总结调研，尝试将它们和项目的需求相结合，利用成熟完善性能可靠的外部系统加强系统的功能。
    在去哪儿网站中，就应用了比较成熟的两种系统：定位系统和评价系统。

- d. 请使用 SCRUM 方法，在（任务b）用例图基础上，编制某定旅馆开发的需求 （backlog）

|ID |Name               |Imp|Est|How to demo|Notes|
|---|-------------------|---|---|---|---|
|1  |Search Hotel       |8  |5  |Type in the destination city, select the check in date, select the check out date, submit the request, choose group buying, use automatic positioning, search by types.|Design appropriate interfaces between different systems|
|2  |Choose Hotel       |4  |7  |The traveler should select a hotel, and submit reservation request| check the correctness of the request |
|3  |Choose Room type   |5  |3  |Specify required rooms and the number of adults and children in each room| check the correctness of the request |
|4  |Confirm Reservation|9  |4  |The traveler provide personal information, choose a method for payment, secure the reservation |Once the payment is made, “Reserve Hotel” will email the customer the confirmation of the payment and the reservation|

## 业务建模
- a. 在（任务b）基础上，用活动图建模找酒店用例。简述利用流程图发现子用例的方法。

![hotelactivity](/img/2018-04-22/hotelactivity.png)

- b. 选择你身边的银行 ATM，用活动图描绘取款业务流程。

![bank](/img/2018-04-22/bank.png)

- c. 查找淘宝退货业务官方文档，使用多泳道图，表达客户、淘宝网、淘宝商家服务系统、商家等用户和系统协同完成退货业务的过程。分析客户要完成退货业务，在淘宝网上需要实现哪些系统用例。

![taobao](/img/2018-04-22/taobao.png)

## 用例文本编写

 在大作业基础上，分析三种用例文本的优点和缺点。

 用例能够以不同形式化程度或格式进行编写，主要分三种常用形式：摘要、非正式、详述。

### 摘要

简洁的一段式概要，通常用于主成功场景。

- 优点

    十分简洁，在早期需求分析过程中，可以用几分钟进行编写便于快速了解主题和范围。

- 缺点

    不能展示出具体的细节。

### 非正式

非正式的段落格式。用几个段落覆盖不同场景。

- 优点

    适用于早期需求分析，编写简单。

- 缺点

    不能展示出具体的细节。


### 详述

详细编写所有步骤及各种变化，同时具有补充部分，如前置条件和成功保证。

- 优点

    详述用例是结构化的，它展示了更多的细节并且更为深入。有利于对具有重要架构意义的用例或场景进行设计或编程。

- 缺点

    实现起来比较复杂。（在迭代和进化式UP需求分析中的第一次需求讨论会中只要求以这种形式编写10%的关键用例。）
