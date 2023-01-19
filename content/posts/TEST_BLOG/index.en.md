
---
weight: 1
title: "TEST_BLOG"
date: 2023-01-18T02:48:04+08:00
lastmod: 2023-01-18T02:48:04+08:00
draft: false
author: "wjg"
authorLink: "https://dillonzq.com"
description: "网站开发阶段的信息"
tags: ["test"]
categories: ["test"]
images: []
resources:
- name: "featured-image"
  src: "featured-image.jpg"
enableEmoji: true
toc:
  auto: false
twemoji: false
lightgallery: true
---

网站开发阶段的信息 :joy: 
:heart_eyes:

<!--more-->

## 已经实现的功能 {#test-done}
***

### 1 网站基础设置
  * 更改网站名称为WJGGAN'S SITE
  * 更改网站简介和图标

### 2 作者设置

```
# Author config
# 作者配置  
[author]
  name = "WangJiagan"
  email = "wangjiaGGan@163.com"
  link = ""
```

### 3 导航栏设置
{{< admonition >}}
在构建网站时, 你可以使用 `--theme` 选项设置主题. 但是, 我建议你修改配置文件 (**config.toml**) 将本主题设置为默认主题.
{{< /admonition >}}

### 4 图片实现
尝试通过微博图床的方式实现，在本地*hugo server*运行时可以实现图片的加载，但发布到网站中便无法实现，可能由于使用
netlify发布无法载入图片。
直接将图片存储到本地文件夹中再git到github上也并不麻烦，所以采取这样的方式也不失为一个很好的选择。

### 5 git流程
```bash
git init 
git add .
git commit -m "commit messages"
git push
```

***
## 未实现的功能 {#test-no}

### 1 网站图标（LOGO）
   
### 2 Emoji
去露营啦! :tent: 很快就回来.

真开心! :joy:
Emoji 无法使用，config文件中的enableEmoji 已经开启为true 但为啥无法使用？？？？！！！！