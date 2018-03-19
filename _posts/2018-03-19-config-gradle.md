---
layout: post
title: 'config.gradle全局配置统一管理项目依赖版本'
date: 2018-03-19
author: Zhouyuzheng
cover: ''
tags: Gradle Android
---

当你需要统一项目依赖库版本，可通过配置全局变量来管理版本与依赖
### 一、根目录下创建config.gradle文件
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/tree/master/screenshot/gradle-config.png)

### 二、config.gradle中添加
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/tree/master/screenshot/gradle-add.png)

### 三、在根目录build.gradle中添加
apply from: 'config.gradle'
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/tree/master/screenshot/gradle-apply.png)

### 四、app或依赖库目录下的build.gradle中就可以引用全局变量了
![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/tree/master/screenshot/gradle-link1.png)

![](https://github.com/zhouyuzheng/zhouyuzheng.github.io/tree/master/screenshot/gradle-link2.png)