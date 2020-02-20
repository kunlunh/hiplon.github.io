---
layout: post
cid: 65
title: OPNsense 内置Netflow工作不正常或者获取不到数据
slug: OPNsense-netflow-problem
date: 2018/11/19 09:46:00
updated: 2019/01/29 16:22:13
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Operating
  - FreeBSD
---


flowd_aggregate服务没有工作，或者报表没有数据 
此情况一般为日志缓存有问题，需要手动清缓存
命令如下 

```bash
rm /var/log/flowd.log*
rm /var/netflow/*.sqlite
```