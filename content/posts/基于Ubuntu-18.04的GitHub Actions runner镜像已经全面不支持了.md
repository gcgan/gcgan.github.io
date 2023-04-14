---
title: "基于Ubuntu-18.04的GitHub Actions runner镜像已经全面不支持了"           # 文章标题
author: "gcgan"              # 文章作者
description : "GitHub Actions runner镜像升级"    # 文章描述信息
date: 2023-04-14            # 文章编写日期
lastmod: 2023-04-14         # 文章修改日期
tags:  ["Github", "Ubuntu"]
categories: ["信息技术"]
---
这两周发布的[GitHub](/tags/Github/) pages突然发现没有正常更新显示。查看了一下日志，发现runner报了一个错“This request was automatically failed because there were no enabled runners online to process the request for more than 1 days.”。同时有一个提示为“The ubuntu-18.04 environment is deprecated, consider switching to ubuntu-20.04(ubuntu-latest), or ubuntu-22.04 instead. For more details see https://github.com/actions/virtual-environments/issues/6002”。原来早在2022年8月2日就已经通知了[Ubuntu](/tags/Ubuntu)-18.04的启用计划，到今年4月3日就完全不支持了。

GitHub pages的这个问题的解决方案也很简单，就是修改.github/workflows目录下的deploy.yml文件，将runs-on的指修改为“[Ubuntu](/tags/Ubuntu)-20.04”或“[Ubuntu](/tags/Ubuntu)-22.04”即可。