---
layout: post
cid: 67
title: proxmox notes
slug: proxmox-notes
date: 2018/08/26 09:17:00
updated: 2019/02/26 09:19:23
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Virtualization
  - Proxmox
---


`/etc/apt/sources.list`

```bash
deb http://mirrors.tuna.tsinghua.edu.cn/debian buster main contrib
deb http://mirrors.tuna.tsinghua.edu.cn/debian sid main
deb http://mirrors.tuna.tsinghua.edu.cn/debian experimental main contrib non-free

deb http://mirrors.tuna.tsinghua.edu.cn/debian buster-updates main contrib
deb http://mirrors.ustc.edu.cn/proxmox/debian/pve buster pve-no-subscription

# security updates
deb http://security.debian.org buster/updates main contrib
```
