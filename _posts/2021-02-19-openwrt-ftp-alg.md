---
layout: post
title: 原版OpenWRT启用FTP ALG功能
slug: openwrt-ftp-alg
date: 2021/02/19 19:01:00
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Linux
  - Operating
  - Networking
---

本文主要介绍原版OpenWRT系统使用FTP ALG功能。

<!--more-->

安装对应kerner mod
```bash
root@OpenWrt:~# opkg install kmod-nf-nathelper-extra
root@OpenWrt:~# opkg install kmod-nf-ipvs-ftp
```

启用对应配置
```bash
root@OpenWrt:~# cat /etc/sysctl.d/11-nf-conntrack.conf 
net.netfilter.nf_conntrack_helper=1
```