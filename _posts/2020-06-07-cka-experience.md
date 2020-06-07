---
layout: post
title: CKA Exam 2020-06考试经验
slug: cka-experience
date: 2020/06/07 21:32:00
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Blog
  - Operating
---

最近趁打折入了CKA的考试券，从入门到考试学习了一个多星期参加了考试，最后以93%的分数通过考试，分享一下最新的情况。

首先还是说下当前Kubernetes已经基本成为业界的标准，连电信行业也引进了Container Network Function (AKA. CNF) 的做法，所以还是有必要更新一下自己的知识库。

前人已经分享了许多经验了，CKA的考试其实网上也有分享了挺多题库，但是都算比较久，所以仅供参考。我下面只说一些自己考试的一些Bibel。

<!--more-->

考试遇到的题目，这份是比较接近 [https://blog.csdn.net/zhouwenjun0820/article/details/105881669](https://blog.csdn.net/zhouwenjun0820/article/details/105881669)

考试用到的Kubernetes已经是1.18版本，其中一些创建Pod，创建Deployment的命令得要注意，例如kubectl run当前就只能创建Pod，要创建Deployment的话还是要老老实实走kubectl create deployment的命令。

而且最新的通过标准好像只要66%，所以估计通过考试问题都不大，所以参加考试的时候不用太紧张了。

待续。


