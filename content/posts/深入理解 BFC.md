---
title: "深入理解 BFC"
date: 2021-01-21T23:44:09+08:00
draft: true，
description: "这次来说说面试常问的 BFC"
tags: ["CSS"]
---

## 什么是 BFC(Block fomatting context)
  - 它是页面中的一块渲染区域，有一套渲染规则，它决定了子元素如何定位以及和其他元素的关系
  - 通俗地说，BFC 是一个容器，用来管理块级元素
## 如何创建 BFC
  - 根元素（<`html`>）
  - 浮动元素（元素的 float 不是 none）
  - 绝对定位元素（元素的 position 为 absolute 或 fixed）
  - 行内块元素（元素的 display 为 inline-block）
  - 表格单元格（元素的 display 为 table-cell，HTML 表格单元格默认为该值）
  - 表格标题（元素的 display 为 table-caption，HTML 表格标题默认为该值）
  - 匿名表格单元格元素（元素的 display 为 table、table-row、 table-row-group、table-header-group、- table-footer-group（分别是 HTML table、row、tbody、thead、tfoot 的默认属性）或 inline-table）
  - overflow 计算值 (Computed) 不为 visible 的块元素
  - display 值为 flow-root 的元素
  - contain 值为 layout、content 或 paint 的元素
  - 弹性元素（display 为 flex 或 inline-flex 元素的直接子元素）
  - 网格元素（display 为 grid 或 inline-grid 元素的直接子元素）
  - 多列容器（元素的 column-count 或 column-width 不为 auto，包括 column-count 为 1）
## BFC 布局规则
  - BFC 的区域不会与 float box 重叠
  - 计算 BFC 的高度时，浮动元素也参与计算
  - BFC 就是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素。反之也如此
## BFC 有哪些特性
  - 阻止垂直外边距折叠
  - BFC 不会重叠浮动元素
  - 可以清除浮动
#### [DEMO](https://codepen.io/coolfe/pen/WNGWRQQ)
###  参考链接
  - https://github.com/ljianshu/Blog/issues/15
  - https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Block_formatting_context


