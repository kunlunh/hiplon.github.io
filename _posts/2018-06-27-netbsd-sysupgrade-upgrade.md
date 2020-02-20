---
layout: post
cid: 52
title: NetBSD使用sysupgrade工具更新系统
slug: netbsd-sysupgrade-upgrade
date: 2018/06/27 19:07:00
updated: 2019/01/29 16:25:09
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Operating
  - FreeBSD
---


解决报错

> 550 netbsd-: No such file or directory.
> 
> E: Failed to determine kernel name; please set KERNEL explicitly

1.使用pkg_add工具下载sysupgrade
```bash
PKG_PATH="http://cdn.NetBSD.org/pub/pkgsrc/packages/$(uname -s)/$(uname -m)/$(uname -r|cut -f '1 2' -d.)/All/"
export PKG_PATH
pkg_add sysupgrade
```
2.修改配置文件`/usr/pkg/etc/sysupgrade.conf`
主要修改

`KERNEL=GENERIC`

3.运行更新程序sysupgrade
`sysupgrade auto ftp://ftp.netbsd.org/pub/NetBSD/NetBSD-7.1.2/amd64`