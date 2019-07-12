---
title: '第3期:(3)hexo部署多设备同步管理'
date: 2019-07-02 18:15:54
categories: 
    - Hexo
tags:
    - 7月
---

### 一、hexo部署多设备同步管理

对于很多已经把项目部署到github来说已经可以发表文章了，但是想要执行多台电脑同时写文章并且操作还是有很多坑，看了网上很多文章总结下来的，一些坑

#### 环境配置

* 安装 hexo
* 安装 Node
* 安装 git

这个不废话直接跳过

#### 创建分支

这个其实就是咱们正常使用github创建项目的流程了，首先咱们要确定的是就是要有两个分支，**master** 和 **hexo**,

* <font color="#d93a49" face="hexo"> **hexo** </font>生成的静态博客文件都是上传到GitHub上的, 且默认放在<font color="#d93a49" face="master"> **master** </font>分支上, 而一些相关的配置文件都在本地,所以首先我们要创建**hexo**分支并且设置**hexo**为默认分支(更换电脑是直接 <font color="#d93a49" face="master"> **git clone hexo** </font>)

* 切换到该**hexo分支**，并在该仓库->Settings->Branches->Default branch中将默认分支设为hexo，save保存

### 二、上传hexo源文件到服务器

#### 克隆hexo分支

* 在**hexo**分支创建完成以后，克隆**hexo**到本地，然后在命令行中执行,查看新建的分支为hexo

```
    $ git branch
    *hexo
```

#### 上传部署文件

* 将本地博客的部署文件（Hexo目录下的全部文件）全部拷贝进刚clone的文件目录中去，需要将插件重新安装一遍

```
    npm install hexo-generator-index --save
    npm install hexo-generator-archive --save
    npm install hexo-generator-category --save
    npm install hexo-generator-tag --save
    npm install hexo-server --save
    npm install hexo-deployer-git --save
    npm install hexo-deployer-heroku --save
    npm install hexo-deployer-rsync --save
    npm install hexo-deployer-openshift --save
    npm install hexo-renderer-marked@0.2 --save
    npm install hexo-renderer-stylus@0.2 --save
    npm install hexo-generator-feed@1 --save
    npm install hexo-generator-sitemap@1 --save
    npm install hexo-generator-search --save
    npm install hexo-generator-searchdb --save
```
* 最后文件全部提交到**Hexo**分支
* 提交时注意事项 如果themes目录中主题中含有主题的.git文件，直接删除
* 最后用终端或者管理工具将所有文件提交到hexo分支


* **另外需要说明的是同步到其他电脑时需要将新电脑的生成的ssh key添加到GitHub账户上**
> master分支和hexo分支各自保存着一个版本，master分支用于保存博客静态资源，提供博客页面供人访问；hexo分支用于备份博客部署文件，供自己维护更新，两者在一个GitHub仓库内也不会有任何冲突

{% link 本文参考出处 https://www.jianshu.com/p/0558c041e56d [external] [title] %}








