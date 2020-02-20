---
layout: post
cid: 42
title: 将FreeBSD由stable分支转到release分支的方法
slug: freebsd-to-release
date: 2017/03/24 09:30:00
updated: 2019/01/29 16:30:04
status: publish
author: HKL
categories: 
  - 默认分类
tags: 
  - Operating
  - FreeBSD
  - Firefox
---


最近在用FreeBSD系统搭建一些实验环境，遇到了在某国内云服务平台提供的FreeBSD旧版本镜像不能升级的情况，
主要原因就是通过`freebsd-update`命令升级系统是只支持release版本的FreeBSD，而服务商的提供的基础镜像是stable版本的，
参考了官方论坛和一些资料，通过`setenv UNAME_r "10.3-RELEASE"`将版本设定成最近的一个release版本,然后再通过

`freebsd-update fetch`

`freebsd-update install`

命令成功将其升级到最新的release版本,之后就可以通过系统的命令进行其他的更新了。