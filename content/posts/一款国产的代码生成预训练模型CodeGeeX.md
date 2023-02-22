---
title: "一款国产的代码生成预训练模型CodeGeeX"           # 文章标题
author: "gcgan"              # 文章作者
description : "一款国产的代码生成预训练模型"    # 文章描述信息
date: 2023-02-22            # 文章编写日期
lastmod: 2023-02-22         # 文章修改日期
tags:  ["人工智能","工具"]
categories: ["人工智能"]
---

## 什么是CodeGeeX？

[官方网站](https://models.aminer.cn/codegeex/zh-CN)的描述是这样的
> CodeGeeX是一个具有130亿参数的多编程语言代码生成预训练模型。CodeGeeX采用华为[MindSpore](https://www.mindspore.cn/)框架实现，在[鹏程实验室](https://pcl.ac.cn/)的1536个国产昇腾910 AI处理器上训练而成。

## CodeGeeX能做什么？

1. **精度代码生成**：支持生成Python、C++、Java、JavaScript、Go、Rust等多种主流编程语言的代码。
2. **跨语言代码翻译**：支持代码片段在不同编程语言间进行自动翻译转换，翻译结果正确率高。
3. **自动编程插件**：CodeGeeX插件现已上架[VSCode插件](https://marketplace.visualstudio.com/items?itemName=aminer.codegeex)和[jetbrains插件](https://plugins.jetbrains.com/plugin/20587-codegeex)。用户可以通过其强大的少样本生成能力，自定义代码生成风格和能力，更好辅助代码编写。插件下载
4. **模型跨平台开源**: 所有[代码和模型权重](https://github.com/THUDM/CodeGeeX)开源开放，用作研究用途。

## 试用情况
从我实验的情况来看，实现一些简单的算法没有任何问题,用来解leecode也可以起到很大的助力。在vscode的插件上，他有三种模式，你可以根据不同场景起到不同作用，隐匿模式可以当成是一个强大的自动完成工具，交互模式（ Control+Enter）可以当成有个AI结对编程人员，Prompt模式可以帮你解释、总结已有的代码。

没安装相应插件，[也可以在这里先试用一下](https://models.aminer.cn/codegeex/zh-CN/playground)