---
title: "微软Edge默认“在浏览器中打开 Office 文件”可能存在的信息安全问题"           # 文章标题
author: "gcgan"              # 文章作者
description : "微软Edge默认“在浏览器中打开 Office 文件”，对信息安全要求高的公司或个人可能存在风险，建议修改默认配置，让文件下载到本地使用。"    # 文章描述信息
date: 2021-03-13            # 文章编写日期
lastmod: 2021-03-13         # 文章修改日期
tags:  ["微软,Edge,信息安全,office"]
categories: ["信息安全"]
---
今天在网上查资料的时候，发现当我下载一个Word文档(Excel、PPT都有类似的问题)的时候，微软Edge的默认选项是在线打开，而不是直接下载这个文件到本地。默认使用这个[地址](https://view.officeapps.live.com/op/view.aspx?src=)+下载文件的地址打开，如下图：
![默认在线打开](../../static/images/edge/%E9%BB%98%E8%AE%A4%E6%89%93%E5%BC%80.png)

这可能会有两个风险，我没法验证：
1. 你的文件下载记录，可能被微软保存；
2. 甚至你下载的文件内容，也可能被微软记录。

作为一个本地都只用wps，而不用微软office的人，这种风险不能接受。可以通过修改Edge的默认设置来禁用这种打开方式，具体操作可以按下图提示的3步来完成：
![修改设置](../../static/images/edge/%E4%BF%AE%E6%94%B9%E8%AE%BE%E7%BD%AE.png)

完成这个设置之后，Edge默认会通过下载到本地的方式来处理Office能处理的文件。