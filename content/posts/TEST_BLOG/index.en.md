
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
基本写作功能已经实现
可以开始写东西了！
不方便的再慢慢调试吧
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
git push  -u origin master
```
{{< admonition failure"报错1">}}
! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/WJGGan/loveit.git'
{{< /admonition >}}

{{< admonition success"解决">}}
**原因：** 远程库与本地库不一致造成的，在hint中也有提示把远程库同步到本地库就可以了
```
git pull
```
{{< /admonition >}}

{{< admonition failure"报错2">}}
fatal: unable to access 'https://github.com/WJGGan/loveit.git/': Recv failure: Connection was reset
{{< /admonition >}}

{{< admonition success"解决">}}

**原因：** 一般是这是因为服务器的SSL证书没有经过第三方机构的签署,解除ssl验证后，再次git即可
```
git config --global http.sslVerify "false"
```
{{< /admonition >}}

在vscode中也可以直接git很方便
**步骤：**
* 1更改文件
* 2打开vscode左侧的源代码管理
* 3点击+号暂存更改
* 4输入commit信息点击提交即可
* 5push(推送)
{{< admonition tip"步骤">}}

* 1更改文件
* 2打开vscode左侧的源代码管理
* 3点击+号暂存更改
* 4输入commit信息点击提交即可
* 5push(推送)

{{< /admonition>}}
### 5 横幅
{{< admonition >}}
一个 **注意** 横幅
{{< /admonition >}}

{{< admonition abstract >}}
一个 **摘要** 横幅
abstract
{{< /admonition >}}

{{< admonition info >}}
一个 **信息** 横幅
info
{{< /admonition >}}

{{< admonition tip >}}
一个 **技巧** 横幅
 tip
{{< /admonition >}}

{{< admonition success >}}
一个 **成功** 横幅
success
{{< /admonition >}}

{{< admonition question >}}
一个 **问题** 横幅
question
{{< /admonition >}}

{{< admonition warning >}}
一个 **警告** 横幅
warning
{{< /admonition >}}

{{< admonition failure >}}
一个 **失败** 横幅
failure
{{< /admonition >}}

{{< admonition danger >}}
一个 **危险** 横幅
danger
{{< /admonition >}}

{{< admonition bug >}}
一个 **Bug** 横幅
bug
{{< /admonition >}}

{{< admonition example >}}
一个 **示例** 横幅
example
{{< /admonition >}}

{{< admonition quote >}}
一个 **引用** 横幅
quote
{{< /admonition >}}
***
## 未实现的功能 {#test-no}

### 1 ~~网站图标（LOGO）~~
   
### 2 Emoji
去露营啦! :tent: 很快就回来.
真开心! :joy:
Emoji 无法使用，config文件中的enableEmoji 
已经开启为true 但为啥无法使用？？？？！！！！
没有Emoji少了狠多乐趣


## 3代码~~隐藏~~和复制
估计是配置文件的问题
隐藏问题可以使用横幅嵌套代码实现
应该也很少会贴代码 
zz