# 博客管理页面

由于node_module过大，gitignore了，一些hexo依赖需要手动安装

## 初始化工作

### 拉取项目

```
git clone https://github.com/Front-lin/myblog
```

### 进入项目

```
cd myblog
```

### 安装依赖

如果条件允许
```
npm i
```

一般无翻墙需要用到cnpm

```
cnpm install
```

## 新建文章

文章在./source/_post/目录下的md文件, 文章以md形式编写

执行新建文章命令会在./source/_post/目录下创建文章名称的.md文件

```
hexo new '文章名称'
```

编写文章

```
---
title: {{ title }} # 会自动生存文章名称
date: {{ date }} # 创建日期自动生成
tags: # 可以自行选择为文章打上标签
 - 例子 # 这样是打上例子标签
categories: # 写文章分类
 - 生活  # 这样是将文章分到生活类别
---
<meta name="referrer" content="no-referrer" />  # 用于加载网络图片所用不用管
......正文.....  # 此处编写正文
```

## 添加图片

图片分为网络图片和本地图片

### 网络图片

网络插入直接在文章照md格式写

```
![](http://xxxxxx/xxx.jpg)
```

### 本地图片

在./source/_post/创建文章名相同的名字

例如文章名字是example.md，那么同样在目录下创建example文件夹用作存放图片

图片资源存放在新建的文件夹中，插入图片如下写法

```
![](example/xxx.jpg)
```


