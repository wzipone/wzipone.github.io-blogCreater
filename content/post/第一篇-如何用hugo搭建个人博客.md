---
title: "第一篇 如何用hugo搭建个人博客"
date: 2020-02-06T21:41:36+08:00
draft: fasle
---

# 如何用 hugo 搭建个人博客

## 第一步：安装Hugo
 
Mac 安装方式
1. brew install hugo
2. hugo version

Windows 安装方式
1. 在[Hugo releases页面](https://github.com/gohugoio/hugo/releases)下载压缩包
2. 解压，将解压后 hugo.exe 放入 D:\software\hugo\hugo.exe
3. 将 D:\software\hugo 加入path
4. 重启终端，运行 hugo version 查看版本

## 第二步：快速搭建博客

根据文档，快速开始
1. 进入[Hugo官网](https://gohugo.io)，点击 Quick Start 快速开始
2. 从 Step 2 开始，按照提示一步一步抄代码，直到 Step 7
3. Step 2 ：建议根文件夹名称为 GitHub用户名.github.io-blogCreater
4. Step 5 : 执行完成后，打开[http://localhost:1313/](http://localhost:1313/)就可以看到博客的本地预览（tips：）
5. Step 7 : 执行完会生成一个 public 目录，这就是我们的博客站点

tips：
1. 使用 hugo server -D 可以预览草稿，hugo server 可以与看非草稿
2. 直接双击打开 public.index.html 不能预览，因为此处不能使用文件协议预览，需要何使用 hugo server 预览

## 第三步：如何让别人能够看到自己的博客

使用 GitHub Pages：
可以预览Html 不能预览mark down
需要预览markdown 直接打开github

GitHub 上建立个人仓库
1. 仓库名为：自己的GitHub用户名.github.io
2. 创建的时候不要勾选其他选择，写好仓库名后直接点创建

本地仓库操作
1. 在本地仓库创建.gitignore 文件，并将/public/写入
2. 进入public目录
   1. git init
   2. git add .
   3. git commit -m 第一次部署
3. 关联远程仓库
   1. git remote add origin 远程仓库位置
   2. git push -u origin master
   3. 建议直接在 Github 的远程仓库上直接复制这两段命令执行
4. 开打远程仓库的 settings 找到 GitHub Pages 可以看到 Your site is published at https://xxxxxx.github.io/ 点击联接就可以看到自己的博客了

   
