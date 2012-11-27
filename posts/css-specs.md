---
title: CSS代码规范
date: '2012-11-26'
description: CSS前端代码规范
categories: 前端规范
---

**Version:** 1.0

**Last Modified:** 10:58 上午 星期二, 十一月 27, 2012

- 文件编码统一使用不带BOM头的UTF-8编码。
- 为防止文件合并及编码问题，避免在样式定义中出现中文，如定义中文字体时尽量采用英文名（如黑体用SimHei，微软雅黑用Microsoft Yahei，宋体用SimSun）。
- 使用4个空格缩进代码。
- 每个属性规则独占一行且缩进对齐。
- 属性值后都要有“;”结尾。
- 属性名冒号后加一个空白字符。
- 属性名和属性值一律采用小写（严禁出现如FONT-SIZE:10px的书写格式）。
- 删除行尾多余的空格。
- 尽量为ID/Class取通用且有意义（能描述模块的含义）的名字，严禁出现以下样式相关的名称（位置，颜色，尺寸等），如redfont，greenbox，leftborder，bigBarNavigation，w255，h350，10px等
- Class命名一律采用小写字符，不使用除破折号“-”之外的特殊字符，多单词组合用破折号“-”分开（如.page-nav，.main-wrap等）。
- 除了作为JS钩子元素或者全局唯一独立模块外，最好不要用ID，确保在任何一个页面不会出现ID的重复。
- JS钩子的ID一律采用“J\_xxx”的方式定义，多单词组合用驼峰式命名（如J\_toggler，J\_siteNav，J\_searchForm），不要在CSS文件中对ID命名定义样式。
- 非必要情况下，ID和Class的命名尽量简短。
- 如果使用CSS3的属性，如果有必要加入浏览器前缀，则按照-webkit-/-moz-/-ms-/-o-/std的顺序进行添加，标准属性写在最后，并且属性名称要对齐。
- 省略URI外的引号（如background-image: url(../test.jpg)）。
- 省略0后面的单位，非0情况下必须加上单位（如padding: 0; margin: 0; width: 100px）。
- 省略0开头小数点前面的0（如padding: .5em，opacity: .8）。
- 16进制尽量采用3位（如用#fff代替#ffffff，#ffcc00代替#fc0）。
- 避免使用CSS“Hacks”。
- 在一些模块和特定页面代码中，避免编写 **可能** 影响全局的css声明，尽量继承其父级class/id名称，如（避免重定义body{},*{}，避免.hd{xxx}，采用.site-nav .hd{}）
- 尽量避免使用!important，尽量采用复杂的CSS继承规则实现。
- 对于页面的小图标，尽量采用CSS Sprite方式进行合并使用。
- CSS背景图的定义要加上时间戳，每次更新图片时同步更新背景图的时间戳（如background-image: url(../test.jpg?t=20121127)）。
- 保证选择器准确匹配到元素的前提下，尽量保持选择器的层级，建议不超过4级（如.site-nav ul li a span.num可简化为.site-nav li .num）
- 尽量能缩写的属性定义尽量缩写（如margin-top:5px;margin-bottom: 10px;margin-left:3px;margin-right:3px可缩写为margin: 5px 3px 10px）。
- CSS编写应该按模块编写，模块内每个元素的定义都在继承该模块最外层元素的Class。
  如（.site-nav{}，.site-nav li{}，.site-nav li a{}）
- 通用模块的定义可参考以下方式定义：
 - 容器采用mod-xxx（mod-可以省略）。
 - 容器的head，body，foot分别用 xxx-hd，xxx-bd，xxx-ft等。
    <pre>`<div class="news">
            <div class="news-hd"></div>
            <div class="news-bd"></div>
            <div class="news-ft"></div>
    </div>`</pre>
- 模块一定要加头尾注释，细节定义可以适当加注释。
    <pre>`<!-- news begin -->
    .mod-news {}
    .mod-news .news-hd{}
    .mod-news .news-bd{}
    <!-- news end -->`</pre>
- 常用的一些css命名
 - 容器：wrap，wrapper，container
 - 导航：nav，mainnav（主导航），subnav（子导航）
 - 页眉：header
 - 主题区域：main
 - 内容区：content
 - 页脚：footer
 - 侧栏：sidebar
 - 网站标志：logo
 - 菜单：menu，mainmenu（主菜单），submenu（子菜单）
 - 面包屑：breadcrumb
 - 搜索：search
 - 当前：current，cur
 - 激活：active，selected
 - 列表信息：list，list-news，list-articles
 - 提示：tip
 - 消息：msg
 - 服务：service
 - 热门：hot
 - 下载：download
 - 状态:status，state
 - 按钮：btn-show, btn-close
 - 图标：icon-manager, icon-user
 - 版权信息：copyright
 - 指南：guide
 - 登录，注册：login，register