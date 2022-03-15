---
layout: post
title:  "GitPages+Jekyll博客搭建"
date:   2021-10-01 20:00:00 +0530
categories: Intro
---
## 

从老早之前就一直想搞一个自己的博客，之前因为没整明白怎么搭（懒），所以一直在博客园上断断续续随便写写。到后来朋友介绍用Markdown，索性自己就在云盘上随便记些东西。时间一久零零碎碎也攒了不少，于是又想着怎么搞下博客。

搭建博客主要用了GitPages+Jekyll，GitPages主要在git上进行配置过程也比较简单。用Jekyll的话是应为它提供了很多设计好了的[主题](http://jekyllthemes.org/)，只需要下载修改下配置文件就可以使用了，不用再整什么前端页面啥的，很方便。下面简单记录一下Jekyll安装过程。

在Windows环境下的话，首先需要下载ruby（2.7.4），安装好ruby后可以通过以下指令安装bundler和jekyll

```shell
gem install jekyll bundler
```

安装好好后可以指令版本看一下是否装好。确保装好后可以去主题里挑选一个自己喜欢的主题去其git页面进行fork，我选的是***plainwhite***这一款。

fork之后可以将项目clone到本地进行修改：

_config.yaml主要修改主页的一些内容如主题源，个人简介等等

```
remote_theme: thelehhman/plainwhite-jekyll
theme: plainwhite
```

_post里是博客的主要内容，上传的文章命名格式必须是以year-month-day-title格式命名，如本文命名为2021-10-01-GitPages+Jekyll博客搭建.md

完成后提交到git，在浏览器输入kli017.github.io发现第一篇简单的博客已经发布了~
