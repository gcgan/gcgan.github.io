---
title: "Hello Althttpd"           # 文章标题
author: "gcgan"              # 文章作者
description : "Althttpd 是一个非常小巧的Web服务器，力求简单、安全和低资源使用。他的作者是Richard Hipp，Richard Hipp也是SQLite的作者，SQLite的官网正是运行在Althttpd上。"    # 文章描述信息
date: 2021-08-24            # 文章编写日期
lastmod: 2021-08-24         # 文章修改日期
tags:  ["Althttpd", "Web服务器"]
categories: ["信息技术"]

---

## Althttpd是什么
[Althttpd](https://sqlite.org/althttpd/doc/trunk/althttpd.md) 是一个非常小巧的Web服务器，力求简单、安全和低资源使用。他的作者是[Richard Hipp](https://github.com/drhsqlite)，Richard Hipp也是[SQLite](https://sqlite.org/)的作者，SQLite的官网正是运行在Althttpd上。

<!--more-->

## Althttpd有多小
Althttpd只有一个文件[althttpd.c](https://sqlite.org/althttpd/file?name=althttpd.c&ci=tip),这个文件一共只有2593行（对应的nginx代码有173139行，不含注释和空行），用cloc分析的数据如下：

| Language | files | blank | comment | code |
| :---: | :---: | :---: | :---: | :---: |
| C | 1 | 101 | 593 | 1899 |

## 本地运行Althttpd
1. 下载源代码：
```shell
wget https://sqlite.org/althttpd/raw/3bd58672947cb446f72bc64471db63d525f949f6a258b89875436f992ebea39c?at=althttpd.c -O ./althttp.c
```

2. 编译安装：
```shell
gcc -Os -o /usr/bin/althttpd althttpd.c
```

3. 准备测试内容
```shell
mkdir ~/www
cd ~/www
echo "Hello Althttpd" > index.html
```

4. 启动Althttp服务
```shell
althttpd -root ~/www -port 8080
```

5. 在浏览器中进行[测试验证](http://localhost:8080/)。
