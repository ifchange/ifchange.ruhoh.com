---
title: HTML代码规范
date: '2012-11-27'
description:
categories: 前端规范
---

**LastModified:** 2013-04-28 13:10:34

## 基础规范
* 采用不带BOM头的UTF-8编码

## 风格规范
* 缩进4个空格，每个子元素都相对父元素进行缩进
* 每个块元素(div/p/blockquote...)，列表元素(ul/ol/li/dl/dt..)，表格元素(table/tbody/th/tr/td...)都独占一行。
* html标签和属性采用小写字符
* 合理嵌套标签，确保标签一定匹配，避免未关闭标记的现象（采用合理的缩进+编辑器一般可以有效避免）。
* 删除行尾的空格

## 代码规范
* 使用HTML5标准的文档类型
* 标签语义话，根据标签语义去使用它们，不要全篇div或者采用不合语义的HTML标记。
* 在样式表和脚本标签中省略type属性（如`<script></script>`，`<style></style>`）。
* 对模块的html代码头尾加上注释。如
    <pre>`<!-- news begin -->
    <div class="mod-news">
    	......
    </div>
    <!-- news end -->`</pre>
* 必须为表单项（如radio,checkbox等）的描述文本添加label标签且通过id关联。
* 重要的图片元素要加上alt属性，写上该图片所代表的内容。对于标题等元素内容可能被截断的情况下，用title属性写上完整内容。
* 需要为html属性定义一些自定义属性与JS交互时，采用html5的“data-”方式（只能用小写字母，多个单词之间用破折号“-”分开）定义， 避免采用其它定义方式
  （如避免`<div initState="show" data:link="a"></div>`，改用`<div data-init-state="show" data-link="a"></div>`）。
* CSS引入一般放置在页面的head区域中(延迟展示的模块的CSS可延迟加载或者放到页面底部)，JS文件一般放置到页面底部。
