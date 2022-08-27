---
title: 'JavaScript: 是一种具有函数优先的轻量级，解释型或即时编译型的编程语言'
author: Binglin Li
toc: true
categories:
  - '2022'
tags:
  - javascript
date: 2022-07-31 19:10:27
---

*JavaScript 是一种全栈式的编程语言*

### 基础语法
JavaScript 是区分大小写的，并使用 Unicode 字符集，JavaScript 是大小写敏感。
ECMAScript 规定了在语句的末尾自动插入分号

{% codeblock lang:javascript %}
var aStr = "foobar";
{% endcodeblock %}

### 注释
{% codeblock lang:javascript %}
// 单行注释

/* 这是一个更长的，
   多行注释
*/

/* 然而，你不能，/* 嵌套注释 */ 语法错误 */
{% endcodeblock %}

### 声明

JavaScript 有三种声明方式。

{% codeblock lang:javascript %}

// 声明一个变量，可选初始化一个值。
var  aStr;



// 声明一个块作用域的局部变量，可选初始化一个值。
let aStr;



// 声明一个块作用域的只读常量。
const aStr = "Hello World!"

{% endcodeblock %}


### 变量的作用域
1. 全局变量
2. 常量 (Constants)

在函数之外声明的变量，叫做全局变量，因为它可被当前文档中的任何其他代码所访问。在函数内部声明的变量，叫做局部变量，因为它只能在当前函数的内部访问。

### 变量提升
JavaScript 变量的另一个不同寻常的地方是，你可以先使用变量稍后再声明变量而不会引发异常。这一概念称为变量提升；
{% codeblock lang:javascript %}
/**
 * 例子 1
 */
console.log(x === undefined); // true
var x = 3;


/**
 * 例子 2
 */
// will return a value of undefined
var myvar = "my value";

(function() {
  console.log(myvar); // undefined
  var myvar = "local value";
})();
{% endcodeblock %}

### 控制流
#### if 语句

{% codeblock lang:javascript %}
	if ( condition ) {
		block of code to be executed if the condition is true
	}
{% endcodeblock %}

#### if else 语句
{% codeblock lang:javascript %}
	if ( condition ) {
		block of code to be executed if the condition is true
	} else {
		block of code to be executed if the condition is false
	}
{% endcodeblock %}
	
#### if else if 语句

{% codeblock lang:javascript %}
	if ( condition1 ) {
		block of code to be executed if the condition is true
	} else if ( condition2 ) {
		block of code to be executed if the condition is true
	} else {
		block of code to be executed if the condition is false
	}
{% endcodeblock %}

#### switch 语句

{% codeblock lang:javascript %}
	switch (expression) {
		case label_1:
			statements_1
			[break;]
		case label_2:
			statements_2
			[break;]
		...
		default:
			statements_def
			[break;]
	}
{% endcodeblock %}

