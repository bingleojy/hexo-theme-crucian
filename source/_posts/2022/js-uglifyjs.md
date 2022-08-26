---
title: 'JavaScript: UglifyJS 是一个用 JavaScript 编写的 JavaScript 压缩器/压缩器'
author: Binglin Li
toc: true
categories:
  - '2022'
tags:
  - js-uglifyjs
date: 2022-08-24 00:34:33
---


#### 它还包含允许自动使用 JavaScript 代码的工具：

1. 从 JavaScript 代码生成抽象语法树 (AST)的解析器。
2. 从 AST 输出 JavaScript 代码的代码生成器，还提供获取 源映射的选项。
3. 压缩器（优化器） ——它使用转换器 API 将 AST 优化为更小的。
4. A mangler — 将局部变量的名称简化为（通常）单字母。
5. 范围分析器，它是一种工具，可通过有关定义/引用变量的位置等信息来扩充 AST。
6. Tree walker——一个简单的 API，允许你在 AST 中的每个节点上做一些事情。
7. 树转换器——另一个用于转换树的 API。
