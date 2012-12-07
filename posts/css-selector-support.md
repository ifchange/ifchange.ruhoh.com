---
title: CSS选择器的浏览器支持
date: '2012-12-07'
description:
categories: 参考资料
---
<link rel="stylesheet" href="http://labs.qianduan.net/css-selector/style/fancybox.css" />
<style>
table.testOverview{margin:10px 0;padding:0;border-collapse:collapse;border:0;font-size:12px;}
table.testOverview caption{text-align:left;margin:10px 0 0;padding:0;font-weight:bold;text-transform:uppercase;font-size:14px}
table.testOverview thead th,table.testOverview tfoot th,table.testOverview foot th{text-align:center;background:#333;border:1px solid #333;color:#eee;padding:3px 5px}
table.testOverview foot th{border-bottom:1px solid #000;}
table.testOverview thead th{ vertical-align: bottom}
table.testOverview tbody th{text-align:left;padding:0;background:#eee;border:1px solid #000}
table.testOverview tbody th.specHeader{text-align:center;text-transform:uppercase}
table.testOverview td{text-align:center;padding:2px 3px;border:1px solid #000;width:90px;text-transform:uppercase}
table.testOverview th a{display:block;padding:4px;text-decoration:underline;color:blue}
table.testOverview th a:visited{color:purple}
table.testOverview th a:hover{background:#eee;text-decoration:none}
.fullSupport{background:green;color:#fff}
.partialSupport{background:#f60;color:#fff}
.noSupport{background:red;color:#fff}
.buggySupport{background:purple;color:#fff}
ol,ul{ margin-left:2em;}
ol li{ list-style-type:decimal}
ul li{ list-style-type: square}
</style>
<script src="http://labs.qianduan.net/css-selector/js/jquery.js"></script>
<script src="http://labs.qianduan.net/css-selector/js/jquery.fancybox.js"></script>
<script src="http://labs.qianduan.net/css-selector/js/jquery.easing.1.3.js"></script>
<script src="/assets/twitter/javascripts/page/css-selector-support.js"></script>
<p>下面是一系列关于最流行的浏览器对<abbr title="级联样式表(Cascading Style Sheets)">CSS</abbr>选择器和伪选择器的支持情况的测试。该测试包括从过去美好的<strong>CSS1</strong>到当前时髦的<strong>CSS3</strong>最基本的东西。如果你想了解关于CSS的选择器的更多内容，<a href="http://www.w3.org/TR/2005/WD-css3-selectors-20051215/" title="W3C Working Draft 15 December 2005" target="_blank">W3C官方文档绝对是个好地方</a>!</p>
<table summary="CSS 1 selectors" class="testOverview" border="1" cellspacing="0">
    <caption>
    CSS 1
    </caption>
    <thead>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/element.html" title="E" class="iframe">E</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/descendant.html" title="E F" class="iframe">E F</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/link.html" title=":link" class="iframe">:link</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/active.html" title="E:active" class="iframe">E:active</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/link.html" title=":visited" class="iframe">:visited</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/firstline.html" title="E:first-line" class="iframe">E:first-line</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/firstletter.html" title="E:first-line" class="iframe">E:first-letter</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/class.html" title="E.classname" class="iframe">E.classname</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/id.html" title="E#id" class="iframe">E#id</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/classname.html" title="E.classname.classname" class="iframe">.classname.classname</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
    </tbody>
</table>
<table summary="CSS 2.1 selectors" class="testOverview" border="1" cellspacing="0">
    <caption>
    CSS 2.1
    </caption>
    <thead>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/star.html" title="*" class="iframe">*</a></th>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/directchild.html" title="E &gt; F" class="iframe">E &gt; F</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/firstchild.html" title="E:first-child" class="iframe">E:first-child</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/hover.html" title="E:hover" class="iframe">E:hover</a></th>
            <td class="partialSupport"><span>Partial (1)</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/focus.html" title="E:focus" class="iframe">E:focus</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/preceding.html" title="E + F" class="iframe">E + F</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr.html" title="E[attr]" class="iframe">E[attr]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name.html" title="E[attr='name']" class="iframe">E[attr="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name_contains.html" title="E[attr~='name']" class="iframe">E[attr~="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/before.html" title="E:before" class="iframe">E:before</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/after.html" title="E:after" class="iframe">E:after</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
    </tbody>
</table>
<table summary="CSS 3 selectors" class="testOverview" border="1" cellspacing="0">
    <caption>
    CSS 3
    </caption>
    <thead>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <th>↓选择器/浏览器→</th>
            <th scope="col"><strong title="Internet Explorer 6.0.3790.1830">IE6</strong></th>
            <th scope="col"><strong title="Internet Explorer 7.0.5730.13">IE7</strong></th>
            <th scope="col"><strong title="Internet Explorer 8.0.6001.18702">IE8</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 2.0.0.14">FF 2</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.0.6">FF 3</strong></th>
            <th scope="col"><strong title="Mozilla Firefox 3.5">FF 3.5</strong></th>
            <th scope="col"><strong title="Safari 3.0">Safari 3.0</strong></th>
            <th scope="col"><strong title="Safari 3.2+">Safari 3.2+</strong></th>
            <th scope="col"><strong title="Chrome 2.0.172.39">Chrome 2</strong></th>
            <th scope="col"><strong title="Opera 9.64">Opera</strong></th>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/preceding2.html" title="E ~ F" class="iframe">E ~ F</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name_begins_part.html" title="E[attr^='name']" class="iframe">E[attr^="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name_ends_part.html" title="E[attr$='name']" class="iframe">E[attr$="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name_contains_star.html" title="E[attr *='name']" class="iframe">E[attr *="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/attr_name_begins.html" title="E[attr|='name']" class="iframe">E[attr|="name"]</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/root.html" title="E:root" class="iframe">E:root</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/nthoftype.html" title="E:nth-of-type" class="iframe">E:nth-of-type</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/nth_last_oftype.html" title="E:nth-last-of-type" class="iframe">E:nth-last-of-type</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/firstoftype.html" title="E:first-of-type" class="iframe">E:first-of-type</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="partialSupport">Yes</td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/lastoftype.html" title="E:last-of-type" class="iframe">E:last-of-type</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/onlyoftype.html" title="E:only-of-type" class="iframe">E:only-of-type</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/onlychild.html" title="E:only-child" class="iframe">E:only-child</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/lastchild.html" title="E:last-child" class="iframe">E:last-child</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/nthchild.html" title="E:nth-child" class="iframe">E:nth-child</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/nth_last_child.html" title="E:nth-last-child" class="iframe">E:nth-last-child</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/empty.html" title="E:empty" class="iframe">E:empty</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="buggySupport"><span>Buggy (2)</span></td>
            <td class="fullSupport"><span>Yes (3)</span></td>
            <td class="buggySupport"><span>Buggy (2)</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/target.html" title="E:target" class="iframe">E:target</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/checked.html" title="E:checked" class="iframe">E:checked</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/selection.html" title="E:selection" class="iframe">E:selection</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/enabled.html" title="E:enabled" class="iframe">E:enabled</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
        <tr>
            <th scope="row"><a href="http://labs.qianduan.net/css-selector/examples/enabled.html" title="E:disabled" class="iframe">E:disabled</a></th>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="noSupport"><span>No</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
            <td class="fullSupport"><span>Yes</span></td>
        </tr>
    </tbody>
</table>
<ol>
    <li>:hover 在IE6中只有<code>a</code>元素可用。</li>
    <li>E:empty 貌似在webkit核心浏览器中有些小bug。</li>
    <li>如果这个bug依然存在，不太确定如何测试。</li>
    <li>IE6不支持.class1{}.class2{}双类选择器。</li>
</ol>
<h3>IE8注意事项：</h3>
<ul>
    <li>E[attr]选择器在值为空的时候或者写错的时候，将不会生效；</li>
    <li>IE8支持CSS2.1的所有属性，支持伪类，但是不支持伪元素。</li>
</ul>
<h3>IE8中的IE7兼容模式</h3>
<ul>
    <li>E[attr] 和IE8一样，值为空或写错的时候，无效；</li>
    <li>E[attr~=val]这里唯一需要注意的是，属性的值，区分大小写；</li>
    <li>E[attr|=val]IE7有一些大小写敏感的问题，但是通常可以正常使用；</li>
    <li>:first-child IE7 会将一个注释或者文字节点当成first-child，而不是只有元素才是“子”元素。所以，如果在第一个子元素前有注释或文字，IE7会匹配之而不是去匹配第一个子元素。</li>
</ul>
<h3>Safari/Chrome</h3>
<ul>
    <li>Safari3.2(事实上可以追溯到3.1)以上的版本已经完全的支持所有CSS选择器了。</li>
    <li>Safari3.0基本上对CSS 2的选择器支持很好，但不支持CSS3大部分新增的选择器，而且对属性选择器的支持<strong>不是很完整</strong>。</li>
    <li>iPhone中的Safari有3.0和3.2两个版本，对CSS的支持情况与PC/Mac版的支持情况一致。</li>
    <li>Android系统自带的浏览器基本上也是基于webkit核心的，其对于CSS选择器的支持情况待测。</li>
</ul>
