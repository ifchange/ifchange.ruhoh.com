---
title: Easyhunter UI设计规范与约定
date: '2012-12-07'
description:
categories: 其它规范
---
<style>
	.color-block{width:30px;margin:0 5px;height: 16px;vertical-align:middle;display:inline-block;border:1px solid #666}
</style>

> **全局约定变量：**  
>
<span style="background:#498cf7;" class="color-block"></span>【linkcolor】#498cf7  
<span style="background:#ff6938;" class="color-block"></span>【orangecolor】#ff6938  
<span style="background:#8cc818;" class="color-block"></span>【greencolor】#8cc818  
<span style="background:#599BD5;" class="color-block"></span>【bluecolor】#599BD5  
<span style="background:#ca213e;" class="color-block"></span>【redcolor】#ca213e  
<span style="background:#c5c5c5;" class="color-block"></span>【graycolor】#c5c5c5  
<span style="background:#878787;" class="color-block"></span>【darkgraycolor】#878787  
<span style="background:#f0f0f0;" class="color-block"></span>【graybg】#f0f0f0  

## 表单 ##
### 标签 ###
- label要与对应的表单关联，点击label要使对应的表单获取焦点
- label用粗体文字，后面不添加冒号
- 对于必填项，在label后显示星号（红色(#f00)，向上偏移0.4em，距左侧文字2px）
- 垂直布局：左侧与其表单项对齐；水平布局：顶到最左侧。

### 按钮 ###
- 页面按钮使用手型光标(cursor:pointer)
- 按钮不使用圆角
- 表单提交按钮：
 - 默认：灰色背景，白色文字，居中显示
 - Hover：**页面对应的主题色作为背景色，其它不变**
- 大按钮（standard-button）：微软雅黑，字体大小18px，行高50px
- 小按钮(small-button)：padding: 6px 8px，字体大小12px，加粗，字体simsun

### 表单项 ###
- txtInput/select/textarea：四周5px的内边距，1px的浅灰色(graycolor)边框/3px圆角，深灰色(darkgraycolor)不加粗文字
- txtInput/select：高度为30px(height:18px + border: 2px + padding: 10px);对应的Label一般也是30px(height:21px + padding-top:9px)

### 错误提示 ###
- 采用红色字体
- 显示在表单域的下面，左侧对齐
- *将表单label文字标红， 或者将边框标红*

## 标题 ##
- 模块大标题(列表标题，添加/查看详情的标题模块)
 - 高度28px，左侧8px宽矩形条，1px的底部边框，默认文字和矩形条及边框都为浅灰色（graycolor）
 - 列表页：如果有自定义列功能，左侧矩形条为链接，可以单击弹出自定义列等设置页面，**hover变色(页面主题色)**

## 表格 ##
- 表头行与数据行高度都为30px(height:20px + padding:10px)

## 页面 ##
- 添加/编辑页面
 - 整个页面背景色为浅灰背景色(graybg),背景垂直铺满所有可用区域
 - **标题：字体和左侧矩形条，底部边框颜色默认为主题色**
- 详情页面
 - 整个页面背景图片统一,背景垂直铺满所有可用区域
 - **标题：字体和左侧矩形条，底部边框颜色默认为主题色**