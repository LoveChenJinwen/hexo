---
title: nodejs自学教程
date: 2017-01-05 11:16:25
tags: [nodejs初级]
---
Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行环境。Node.js 使用了一个事件驱动、非阻塞式 I/O 的模型，使其轻量又高效。Node.js 的包管理器 npm，是全球最大的开源库生态系统。
Node.js 适合的场景：JSON APIs，准实时应用系统，单页面、多Ajax请求应用。一个语言或者框架都有适合的场景和不适合的场景，所以作为一个开发者应该数据至少目前比较流行的框架。
<!--more-->
#### 1、nodejs安装
nodejs安装有三种方式：
1）通过安装包安装   推荐用适合windows安装
2）通过源码编译安装
3）在 Linux 下可以通过 yum|apt-get 安装   （就是源码安装）
#### 2、npm
NPM是随同NodeJS一起安装的包管理工具，能解决NodeJS代码部署上的很多问题：
允许用户从NPM服务器下载别人编写的第三方包到本地使用。
允许用户从NPM服务器下载并安装别人编写的命令行程序到本地使用。
允许用户将自己编写的包或命令行程序上传到NPM服务器供别人使用。

	npm -v 查看npm版本
	npm install <Module Name> 安装模块
	npm install express  本地安装web框架模块express
	npm install express -g  全局安装web框架模块express
	npm uninstall express 卸载模块
	npm update express 更新模块
	npm search express 搜索模块
	
express 是nodejs一个web框架模块，比较火的web框架
#### 3、pm2
pm2是node的进程管理工具，可以利用它来简化很多node应用管理的繁琐任务，如性能监控、自动重启、负载均衡等，而且使用非常简单。
	
	npm install -g pm2  全局安装
	pm2 start app.js   启动（方式很多）
pm2其他命令可以去官网上查看
[nodejs官网](http://nodejs.cn/)
[pm2官网](http://pm2.keymetrics.io)

***
** 邮箱：** * 1051165801@qq.com * 
** 微信：** * liu1051165801 *