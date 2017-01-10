---
title: 用hexo在github搭建个人博客
date: 2017-01-04 16:52:25
tags: [hexo,github搭建个人博客]
---
怎么搭建一个自己喜欢博客呢？这篇文章能就让你也拥有自己的个性博客，做一个合格的IT程序猿
<!--more-->
#### 准备
1、注册一个GitHub账号
2、需要验证你注册GitHub账号的邮箱
3、建立一个仓库
注意（记住建立仓库时所填写的内容！是你的帐号.github.io 这是因为github规定的格式这样才会直接讲当前仓库作为托管站点）
#### git安装
1、去官网上下载git
2、安装git（成功你会有Git Bash）
#### hexo安装
1、你的电脑先要安装nodejs，这个去官网上下载个，然后安装下
2、点开git bash 或者右键 就会有git bash here
3、安装hexo  命令 ：
  $ npm install hexo -cli -g 
4、下载hexo文件夹 放文件的路径 D:\\myblog\\hexo 
  $ hexo init  D:\\myblog\\hexo
5、安装依赖包 进入hexo文件夹的位置
  $ npm install
6、加载和启动hexo
  $ hexo g
  $ hexo s
然后你就可以看到一只地址：http://localhost:4000/ 这个是本地访问hexo生成的你的博客 默认的博客主题是landscape
个人觉得不好看，可以换主题
#### 上传你本地的博客到GitHub上
1、首先让git能链接上你的github，这个可以在网上找教程看下 
推荐:[git和github](http://www.cnblogs.com/fnng/archive/2011/08/25/2153807.html)
2、hexo文件夹中修改_config.yml配置文件
主题文件（yelee 主题文件名）

	theme: yelee

github地址（LoveChenJinwen为github的你的用户名）

	deploy:
		type: git
		repository: ssh://git@github.com/LoveChenJinwen/LoveChenJinwen.github.io  
		branch: master

3、上传你的博客
  $ hexo g
  $ hexo d
过程中没报错 那么恭喜你，你已经拥有的你的博客
#### 编辑博客
这个编辑博客用的是markdown语言，这个语言很简单 你可以看下就会编辑了
新建一篇博客
	$ hexo new “my first hexo”
在hexo文件夹中找到 my first hexo.md文件，这个文件就是编辑博客的源文件
***
** 邮箱：** * 1051165801@qq.com * 
** 微信：** * liu1051165801 *