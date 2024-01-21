---
title: "如何在云服务器上装 Arch Linux"
slug: "vps2arch"
date: 2020-06-09T15:31:00.000Z
categories:
- 技术
tags:
- Arch Linux
- 云服务器
aliases: /Tutorial/vps2arch.html
---

*这篇文章讲了如何在云服务器上安装一个 Arch Linux，不推荐没有 Linux 操作经验的用户使用 Arch Linux。*
*友情警告：重装系统会**抹掉**云服务器的**硬盘**，请先备份好所有重要数据！*

<!--more-->

### 前言
  - 本文适用于 Arch Linux 用户，小白有可能不适合阅读本文。
  - 警告: 本文介绍的脚本在运行时将会**格式化**硬盘，请提前**备份重要数据**后继续操作。
----------

### 工具
  - vps2arch
    - [Gitlab 官方介绍][1]
    - [ArchWiki(中文页) 介绍页][2]
    - [ArchWiki(英文页) 介绍页][3]

### 后续更新
  - 推荐使用由 Arch Linux TU (Trust User) **Felix Yan** 大佬维护的 [vps2arch][4]
----------

### 使用方法
#### 1. 下载脚本文件
```shell
wget https://felixc.at/vps2arch
```
#### 2. 赋予执行权限
```shell
chmod +x vps2arch
```
#### 3. 执行脚本文件
```shell
./vps2arch -m [镜像源]
```
#### 例如:
```shell
wget https://felixc.at/vps2arch
chmod +x vps2arch
./vps2arch -m https://mirrors.bfsu.edu.cn/archlinux/
```


  [1]: https://gitlab.com/drizzt/vps2arch
  [2]: https://wiki.archlinux.org/index.php/Install_Arch_Linux_from_existing_Linux_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)#%E4%BB%8E%E4%B8%80%E4%B8%AA%E4%B8%BB%E6%9C%BA%E8%BF%90%E8%A1%8C%E5%8F%A6%E4%B8%80%E4%B8%AALinux%E5%8F%91%E8%A1%8C%E7%89%88
  [3]: https://wiki.archlinux.org/index.php/Install_Arch_Linux_from_existing_Linux#From_a_host_running_another_Linux_distribution
  [4]: https://github.com/felixonmars/vps2arch/
