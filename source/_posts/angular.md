---
title:  angular环境搭建!
tags: angular
---
# 快速开始

### 1.安装[nodejs](https://nodejs.org/en/download/)
首先要安装nodejs，如果你的电脑已经装过了，最好确认是比较新的版本，否则可能会出问题。 
没有安装的直接去nodejs官网下载nodejs安装。安装过程很简单，官网有教程。

下载地址：[https://nodejs.org/en/download](https://nodejs.org/en/download/)

安装完成后，windows+R 输入cmd，打开命令
输入 **node -v** 看看安装版本 

### 2.安装cnmp
由于Angular CLi的一些资源被墙掉了，所以这里我们使用淘宝的镜像去下载安装，否则会很慢并且很容易出问题。

 淘宝镜像网址：[https://npm.taobao.org/](https://npm.taobao.org/)
 
 #### 使用node npm命令安装
``` bash
npm install -g cnpm –registry=https://registry.npm.taobao.org
```
之后安装angular cli的时候我们就用**cnpm**命令即可。包括其他被墙的资源也可以用cnmp去下载安装！

### 3.安装Angular Cli

之前电脑上如果安装过angular cli老版本的话建议先卸载，然后重新安装
#### 卸载老版本：
``` bash
npm uninstall -g angular-cli 
```
#### 卸载新版本：
``` bash
npm uninstall -g @angular/cli
```
#### 清除下缓存 ：
``` bash
npm cache clean
```
更多信息: [服务器](https://hexo.io/docs/server.html)

#### 然后开始安装，记住，最好用**cnpm**

``` bash
cnpm install -g @angular/cli@latest
```

安装完成后输入 **ng help** 查看是否安装成功 


# angular 搭建项目

### 1.搭建项目框架
安装完命令行工具后我们就可以创建Angular项目了。 
首先，切换到项目的存放目录，我的是在桌面的angularDemo文件夹下 
输入:
``` bash
ng new [projectName] 
```
projectName就是你的项目名称，例如，我创建一个aution项目

然后耐心等待，这里会下载很多东西，所以不要着急

这就表示创建完成了
### 1.运行项目
首先切换至项目目录，然后执行**ng serve**命令
在项目目录输入：
 ``` bash
ng serve
 ```
 
 出现上图所示表示项目运行成功了。默认是运行在4200端口上的。
  
 打开浏览器，输入**localhost:4200**即可访问。

 大功告成！一个Angular的项目就创建好了

