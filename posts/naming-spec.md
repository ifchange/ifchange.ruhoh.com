---
title: 前端其它规范
date: '2012-11-27'
description:
categories: 前端规范
---

## 文件命名约定 
* 英文命名优先，拼音其次。
* 使用小写字母，数字和中划线组成，多个单词之间使用中划线“-”连接。
* [文件]：
  * JS/CSS文件命名建议： 名词（页面是什么）+动词（该页面是做什么的），如customer-add.css，candidate-search.js,
* [目录]：
  * 尽量使用简短的命名，不超过5个字符
  * 不要使用复数命名，采用单数格式

## 图片相关
* 图片格式仅限gif，jpg，png格式
* 对于动画类型采用gif，普通的CSS背景图采用png8，对于颜色比较丰富或者照片修饰类的采用.jpg。
* 保证视觉效果的前提下，选择文件大小最小的格式。
* 尽量避免半透明(PNG24)的图片，若使用，请注意考虑及测试IE6浏览器。
* 运用CSS Sprite集中各类小图标，按照图片类型进行合并，并保存主要的源文件至PSD目录。
* 图片命名建议：类型+具体说明，如icon-user，icon-addv，icon-next，btn-save，btn-cancel，bg-body，bg-block，arrow-down.png，arrow-down-big.png等
