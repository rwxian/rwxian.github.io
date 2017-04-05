---
title: ubuntu系统boot分区空间不足
date: 2017-03-28 12:48:05
tags: 菜鸟修炼
---
经常遇到boot空间不足的情况，原来是因为linux更新了新的内核，而旧内核还在，boot分区越来越小导致的。解决方法就是删除旧内核。
- 使用命令dpkg --get-selections | grep linux来查看一下安装了那些内核。
- 列出的内核中，带image的就是旧的内核，如果后面跟install代表已安装，如果是deinnstall就是未安装的。
- 使用uname -a来看看系统启用的是那个版本的内核
- 然后就可以用sudo apt remove+旧内核版本号来删除旧内核了，boot空间就腾出来了。