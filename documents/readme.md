# 第一章 认识网页

渲染特定的编程语言 html 

## 1.1 结构 表现 行为
html 结构
css  样式 表现
javascript 活动 行为

W3C 万维网联盟

## 1.2 HTML 
- Hyptertext Markup Language 超文本标记语言
- 负责网页的结构

# 第二章 HTML 基础语法

## 2.1  认识标签

- 成对出现 <h1> </h1>
- 自结束标签 <img>

## 2.2 注释

<!-- 注释 -->

`注释不能嵌套`

## 2.3 标签中的属性

在`开始标签`中设置

```html
<h3><font color="yellow" size="3">属性</font>测试</h3>
```

属性值根据文档中写，属性值用引号，可以单引号也可双引号



## 2.4 网页的基本结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
   <title>Document</title>
</head>
<body>
    
</body>
</html>
```



## 2.5 实体

多个空格浏览器识别为一个空格

*1. 空格，连续空格*

*2. 特殊字符 大于号 小于号*

*3. 实体、转义字符*

空格 不会换行的空格： &nbsp;

```html
&nbsp;
```

小于

```html
&lt;
```

大于

```html
&gt;
```

例如：

```html
	<p>
        今天 天气 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;真不错
    </p>
    <p>
        a&lt;c&gt;b
    </p>
```

实体参考

https://www.w3school.com.cn/html/html_entities.asp

## 2.6 meta标签

给爬虫程序看的

charset 指定网页的字符集

name 指定数据的名称

content 指定数据的内容 英文逗号分隔

例如：

```html
	<meta charset="UTF-8">
    <meta name="keywords" content="HTML5,CSS">
    <meta name="description" content="这是一个非常不错的网站">
    <meta http-equiv="refresh" content="3;url=https://www.baidu.com">
```

## 2.7 语义化标签

标题标签：h1 到 h6 

p标签：段落标签 

块元素：独占一行，如 p  ，h1，blockquote

hgroup ： 标题分组

q: 引用 短 行内元素

blockquote：块元素



## 2.8 行内元素，块元素

块元素：独占一行，对网页进行布局

行内元素：对文字设置特殊效果
