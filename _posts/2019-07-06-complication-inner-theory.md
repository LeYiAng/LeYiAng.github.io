---
layout: post
title: "编译程序的步骤 - 深入理解计算机操作系统"
description: "编译程序的底层知识"
date: 2019-07-06
tags: [Linux, gcc, c, compilation]
---

在编译一个程序时，GCC在内部会分四个步骤来做：

+ 预处理阶段 (Preprocessing Phase)
+ 编译阶段 (Compilation Phase)
+ 汇编阶段 (Assembly Phase)
+ 链接阶段 (Linking Phase)

## 预处理阶段
在本阶段GCC会解析所有以 `#` 开头的语句，如 `include` - GCC 会将 `include` 引入的代码一股脑儿的全放到代码的头部。
可用 `gcc -E filename` 查看预处理阶段的结果。
