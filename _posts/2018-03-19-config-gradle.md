---
layout: post
title: 'config.gradle全局配置统一管理项目依赖版本'
date: 2018-03-19
author: Zhouyuzheng
cover: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1521447977484&di=44a4719f236f207d3db2f1965a84f51f&imgtype=0&src=http%3A%2F%2Fa1.jikexueyuan.com%2Fhome%2F201512%2F31%2Fe075%2F5684922dae731.jpg'
tags: Gradle Android
---

> 当你需要统一项目依赖库版本，可通过配置全局变量来管理版本与依赖

### 一、根目录下创建config.gradle文件
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/blob/master/screenshot/gradle-config.png?row=true)

### 二、config.gradle中添加
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/blob/master/screenshot/gradle-add.png?row=true)

### 三、在根目录build.gradle中添加
apply from: 'config.gradle'
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/blob/master/screenshot/gradle-apply.png?row=true)

### 四、app或依赖库目录下的build.gradle中就可以引用全局变量了
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/blob/master/screenshot/gradle-link1.png?row=true)

![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/blob/master/screenshot/gradle-link2.png?row=true)
