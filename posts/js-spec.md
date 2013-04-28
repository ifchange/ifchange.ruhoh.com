---
title: JavaScript编码规范
date: '2012-11-28'
description:
categories: 前端规范
---

**Last Modified：** 2013-04-28 13:17:54

## 代码风格
* 采用四个空格进行缩进。
* windows换行符
* 开始的花括号不换行，跟在函数名或者条件判断后面。
    <pre>`if (a > b)
    {
        ....
    }
    function()
    {
        ....
    }
    // 应写为：
    if(a > b){
        ....
    }
    function(){
        ....
    }
`</pre>
* 一行代码的长度最好不超过80个字符，当一条语句过长时可以进行换行拆分，一般在标点符号后面拆分，比如逗号，加号等。
* 等号/条件判断符前后，逗号，JSON冒号后面，三元语句的?/:前后，if条件语句中的分号后面，都要加空格。
    <pre>`var name = 'john';
    var arr = [1, 2, 3, 4];
    var obj = {a: 1, b: 2, c: 3};
    name == 'john' ? 1 : 2;
    function foo(a, b, c){
        if(var i = 0; i < 10; i++){
            ...
        }
    }`</pre>
* 使用引号的地方，优先考虑使用单引号代替双引号。
* 使用三元运算符“?:”代替简单的if/else语句。
    <pre>`if(a > 10){
        b = 1;
    }else{
        b = 2;
    }
    //可优化为：
    b = (a > 10 ? 1 : 2);`</pre>
* 编写规范且有意义注释。
  * 类的构造函数，重要的方法/属性/内部变量要写上注释
  * 代码中参考第三方代码段时要写上注释且注明参考源
  * 对于一些容易误解的写法加上注释
  * 用注释分割一些过长的代码，按功能或逻辑来划分
  * 注释标识符与注释内容要用一个空格分割，如// xxx，/* xx */
* 每个JS文件应该封装在一个闭包内，并且在闭包的头尾加上分号，参考下面的代码或者采用AMD/CMD规范。
    <pre>`;(function($, window, undefined){
        ....
    })(jQuery, window);`</pre>

## 语法规则
* 每条语句必须都有分号结尾，除了for, function, if, switch, try, while。
* 不要省略花括号“{}”，除非是在同一行中。
* 避免数组及json中额外的逗号。如：var arr = [1,2,3,], obj={a:1,b:2,}。
* for-in循环体中必须用hasOwnProperty方法检查成员是否为自身成员。避免来自原型链上的污染。
* 使用严格的条件判断符。用===代替==，用!==代替!=。
* 下面类型的对象不建议用new构造：new Number，new String，new Boolean，new Object(用{}代替)，new Array(用[]代替)。
* 引用对象成员用obj.prop1代替obj["prop1"]，除非属性名是变量。
* 使用前置的+把字符串转换为数字（特别是在读取页面表单数据进行运算时）。
* 不要在if/while的条件判断中进行赋值。
    <pre>`var a;
    if(a = b / 2){...}
    // 应该改为
    var a = b / 2;
    if(a){...}
    `</pre>
* 不要使用with；除了用于解析序列化串外不要使用eval。
* 不要在块语句内定义函数。

## 变量声明
* 所有变量在使用前都要先用var声明，避免导致意外的隐式全局变量的出现。
* 变量定义要放置在函数或者方法的开头部分，一次性定义完，一般把不初始化值的放在前面，初始化值的放在后面，赋值的变量声明一般每行一个。
    <pre>`var var end, unit,
	tween = this.createTween( prop, value ),
	parts = rfxnum.exec( value ),
	target = tween.cur(),
	start = +target || 0,
	scale = 1,
	maxIterations = 20; 
    `</pre>
* 尽量减少全局变量，特别应该严禁隐式的全局变量（如方法内不用var声明的变量）。

## 命名规则
* 创建一个类的构造器首字母大写的驼峰式命名，如Dialog，WidgetSuggest。
* 变量及类的方法或属性采用首字母小写的驼峰式命名，如init，bindEvent，updatePosition。
* 类的私有变量或者属性采用下划线开头，如\_current、\_defaultConfig。
* 常量命名全部大写，多个单词之间用下划线“_”分隔，如TXT_LOADING，DOM_CACHE。
* 用“动词-形容词-名词”格式来命名程序和函数。
* 变量名要足够长(描述意义完整)，尽量短(选择简短或者有效的缩写或单词)，有意义(选择意义准确的单词)。

## 其它建议
* 避免使用JS直接修改元素的样式，应该转换为操作其ClassName，样式的问题应该交给class来管理。
* 避免使用复杂的html字符串拼接，一者比较难看，二者容易出错。应该转化为html模版的方式处理，对于特别复杂的html块，可改为用ajax加载外部模版。
* 可以在一些简短的代码中使用二元操作符&&，||代替简单的条件语句。
    <pre>`if(b != false){a = b}else{a = 10}
    // 可优化为
    a = b || 10;
    `</pre>
* 对于一些有具体含义的状态/类型的值（如操作类型），不要直接用数字，而应该定义一个常量代替。
    <pre>`function doSomething(val){
        if(val == 1){
           add();
        }else if(val == 2){
           del();
        }
        if(val == 1){
            others();
        }
    }
    // 优化为
    function doSomething(val){
        var ADD = 1;
        var DEL = 2;
        if(val == ADD){
           add();
        }else if(val == DEL){
           del();
        }
        if(val == ADD){
            others();
        }
    }
`</pre>
