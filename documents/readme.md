# 第1章 认识网页

渲染特定的编程语言 html 

## 1.1 结构 表现 行为
html 结构
css  样式 表现
javascript 活动 行为

W3C 万维网联盟

## 1.2 HTML 
- Hyptertext Markup Language 超文本标记语言
- 负责网页的结构

# 第2章 HTML 基础语法

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

## 2.7 语义化标签 tag

标题标签：h1 到 h6 

p标签：段落标签 

块元素：独占一行，如 p  ，h1，blockquote

hgroup ： 标题分组

q: 引用 短 行内元素

blockquote：块元素



## 2.8 行内元素，块元素

块元素：独占一行，对网页进行布局

行内元素：对文字设置特殊效果



## 2.9 结构化语义标签 tag

header

main 主体

footer 可以在一些标签内，如article

nav 导航

aside 和主题相关的，侧边栏，解释说明

article 文章

section

div

span

## 2.10 列表

```html
    <!-- 
        1. 有序列表 ol
        2. 无序列表 ul
        3. 下拉菜单 dl
    -->
    <ul>
        <li>1</li>
        <li>2</li>
    </ul>
    <ol>
        <li>aaron</li>
        <li>jack</li>
    </ol>
    <dl>
        <dt>结构</dt>
        <dd>1. 结构表示网页的结构</dd>
        <dd>2. 结构表示网页的结构</dd>
    </dl>
```

列表之间可以互相嵌套

## 2.11 超链接

使用 a 标签表示超链接

行内元素，可以嵌套除它以外的任何元素

href 属性

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- 
        1. 可以是外部网页的连接
        2. 可以是内部的目标路径
    -->
    <a href="https://www.starvistar.com">星原览胜</a>
    <br>
    <a href="demo.html">inner</a>
</body>
</html>
```

## 2.12 相对路径

相对路径，当前页面相对另一个的路径

./meta.html

../code/meta.html

## 2.13 超链接属性

target 

lorem 快捷生成文字

alt + shift + 下  copy



javascript:;

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <!-- 
        1. _self 自己
        2. _blank 新标签页打开

        id 属性 每个标签都可加id属性,都是字母开头
    -->
    <a href="https://www.starvistar.com" target="_self">starvistar</a>
    <a href="#bottom">去底部</a>
    <a href="#p3">去第三个自然段</a>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Adipisci vero quam amet at voluptates! Et dolorem
        laboriosam tenetur sequi ipsum reprehenderit fugit blanditiis doloribus, ad dignissimos quos neque reiciendis
        tempora.</p>

    <a href="#" id="bottom">回到顶部</a>
    <a href="javascript:;">什么也不会发生</a>
</body>

</html>
```

## 2.14 图片标签

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img src="../images/1.jpg">
</body>
</html>
```

alt 会在图片无法加载时显示

width 

height

如果只改了高或者长度，它会等比例缩放，一般不建议修改大小	

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <img src="../images/1.jpg" width="500" height="500" alt="风景">
</body>
</html>
```

图片格式

- jpg 颜色丰富，不支持透明效果，不支持动图

- jpeg

- gif  支持动图，简单透明

- png 支持颜色丰富，支持复杂透明，不支持动图 用的最多

- webp 兼容性差

- base64 需要和网页一起加载的图片

**效果一样，用小的**

## 2.15 内联框架

iframe

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- 
        内联框架：用于向当前页面中引入一个其他页面
        src 指定要引入页面的路径
        frameborder 指定内联框架的边框
    -->
    <iframe src="https://www.starvistar.com" width="800" height="600" frameborder="0"></iframe>
</body>
</html>
```

## 2.16 音视频

video

audio

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <!-- 
        audio 标签 引入音频文件,默认情况不允许用户控制播放停止
        属性：
            controls 是否允许用户控制播放
            autoplay 是否自动播放 大部分浏览器不会自动播放
    -->
    <!-- <audio src="../source/1.mp3" controls></audio> -->
    <audio controls>
        对不起，您的浏览器不支持升级浏览器
        <source src="../source/1.mp3">
        <source src="../source/1.ogg">
        <embed src="../source/1.mp3" type="audio/mp3" width="" height=""> 
        <!-- 第一个不起作用就找第二个 -->
    </audio>
    <!-- <embed src="../source/1.mp3" type="audio/mp3" width=> -->
    <!-- 
        video 和audio使用类似
        webm 格式    
    -->
    
    <video src="../source/1.mp4" controls></video>

</body> 
</html>
```

# 第3章 CSS基础语法

## 3.1 CSS位置

第一种：标签内部，内联样式

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <!-- 
        css 简介：层叠样式表，设置网页中元素的样式        
    -->
    <!--
    第一种： 标签内部 ，内联样式
    -->
    <p style="color: red; font-size: 60px;">少小离家老大回</p>

    <p style="color: blue; font-size: 40px;">今天天气真不错</p>


</body>

</html>
```

第二种： 单独一个style标签在head里，内部标签， 只能对一个网页起作用。

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- 
        第二种：内部样式表 
        修改一处即可全部修改
    -->
    <style>
        p{color: yellow;}
    </style>
</head>

<body>
    <!-- 
        css 简介：层叠样式表，设置网页中元素的样式        
    -->
    <!--
    第一种： 标签内部 ，内联样式
    -->
    <p style="color: red; font-size: 60px;">少小离家老大回</p>

    <p style="color: blue; font-size: 40px;">今天天气真不错</p>

    <p>style 标签</p>

</body>

</html>
```

第三种(**最佳使用方式**)：外部样式表，多个网页中使用，需要link标签使用，可以使用浏览器缓存机制，提高加载速度

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- 
        第二种：内部样式表 
        修改一处即可全部修改
    -->
    <!-- <style>
        p{color: yellow;}
    </style> -->
    <!-- 
        第三种： 外部样式表 
    -->
    <link rel="stylesheet" href="./style.css">
</head>

<body>
    <!-- 
        css 简介：层叠样式表，设置网页中元素的样式        
    -->
    <!--
    第一种： 标签内部 ，内联样式
    -->
    <p style="color: red; font-size: 60px;">少小离家老大回</p>

    <p style="color: blue; font-size: 40px;">今天天气真不错</p>

    <p>style 标签</p>

</body>

</html>
```

```css
p{
    color: rebeccapurple;
    font-size: 20px;
}
```

## 3.2 CSS语法

注释

```css
/* CSS注释实例 */
```

选择器，声明块

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- 在style标签里遵循css语法，注释也不一样 -->
    <style>
        /* 
            CSS注释实例 
            CSS基本语法
                选择器 声明块

            选择器

            声明块：名值对结构
        
        */
        p{
            color: rebeccapurple;
            font-size: 40px;
        }
    </style>
</head>
<body>
    <p>今天天气真不错</p>
</body>
</html>
```

## 3.3 常用选择器

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            元素选择器
        */
        h1{
            color: red;
        }
        p{
            color: black;
        }
        /* 
            id选择器 #id
        */
        #red{
            color: red;
        }
        /* 
            类选择器 .class 多个class使用空格隔开
        */
        .blue{
            color: aqua;
        }
        .abc{
            font-size: 30px;
        }
        /* 
            通配选择器 *
        */
        *{
            color:black;
        }
    </style>
</head>
<body>
    <h1>标题</h1>
    <p>第一段</p>
    <p class="blue abc">第二段</p>
    <p id="red">第三段</p>
    <p class="blue">第四段</p>
</body>
</html>
```

## 3.4 复合选择器

交集选择器 选择器1选择器2

并集选择器  逗号分隔，相当于或

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .red{
            color: red;
        }
        /* 
            复合选择器，交集选择器，同时满足
            语法：选择器1选择器2
            注意：元素选择器开头
        */
        div.red{
            font-size: 30px;
        }
        /* 
            并集选择器 同时选择
            语法：逗号分隔，逗号相当于或
        */
        h1,span{
            color: green;
        }
    </style>
</head>
<body>
    <div class="red">我是div</div>
    <p class="red">我是p</p>
    <h1>标题</h1>
    <span>span</span>
</body>
</html>
```

## 3.5 关系选择器

子元素选择器    父元素 > 子元素

后代选择器   祖先 后代

兄弟选择器  兄 + 紧挨着的第   兄 ~ 弟弟们

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            父元素
            子元素
            祖先元素，间接包含
                - 直接或间接包含
            后代元素
                - 直接或间接
            兄弟元素
                - 拥有相同父元素
        */
        /* 
            为div子元素span设置
            子元素选择器
            语法：父元素 > span
        */
        /* div > span{
            color: orange;
        } */
        /* 
            后代元素选择器
            语法：祖先 后代
        */
        /* div span{
            color: orange
        } */
        /* div > p > span{
            color: red;
        } */

        /* 
            兄弟选择器
            语法：前一个 + 下一个 影响紧挨着的弟弟
            注意：紧挨着，隔了一个元素就选不到

            语法：兄 ~ 第 影响所有弟弟
        */
        p + span{
            color: red;
        }
    </style>
</head>
<body>
    <div>
        我是div
        <p>
            我是div中的p元素
            <span>我是p中的span</span>
        </p>
        <span>我是div中的的span</span>
    </div>
</body>
</html>
```

## 3.6 属性选择器

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            第一种：[属性名]
            第二种：[属性名=属性值]
            第三种：[属性名^=属性值] 以属性值开头的元素
            第四种：[属性名$=属性值] 以属性值结尾的元素
            第五种：[属性名*=属性值] 含有属性值的元素
        */
        p[title^=abc]{
            color: red;
        }
        p[title$=cat]{
            color: orange;
        }
    </style>
</head>
<body>
    <p title="abc">第一段</p>
    <p title="abcedfcat">第一段</p>
    <p title="cat">第一段</p>
    <p>第一段</p>
    <p>第一段</p>
    <p>第一段</p>
</body>
</html>
```

## 3.7 伪类选择器

伪类 带一个冒号

伪元素 带两个冒号

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            ul中第一个li设置为红色
        */
        /* 
            伪类：不存在的类，描述元素的特殊状态
            如：点击，第一个子元素，鼠标移入
            - 一般使用冒号开头
            -   子元素
                :first-child
                :last-child
                :nth-child(3)
                :nth-child(n) 全选中
                :nth-child(2n) 或 even 偶数位元素
                :nth-child(2n+1) 或 odd 奇数位元素
            - 依据所有元素排序
            - 同类子元素(和上面的区别，只找相同类型)
                :first-of-type
            - :not() 否定伪类
                将复合的元素从选择器排除
                ul > li:not(:nth-child(3)){
        */
        /* ul > li:first-child{
            color: red;
        }
        ul > li:last-child{
            color: red;
        } */
        ul > li:not(:nth-child(3)){
            color: blue;
        }
    </style>
</head>
<body>
    <ul>
        <li>第1个</li>
        <li class="first">第2个</li>
        <li>第3个</li>
        <li>第4个</li>
        <li>第5个</li>
    </ul>
</body>
</html>
```

## 3.8 超连接的伪类

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            1.访问过
            2.没访问过
        */
        /* 没访问 */
        a:link{
            color: red;
            font-size: 40px;
        }
        /* 
            由于隐私的原因，在visited中只能改颜色
        */
        /* 访问过 */
        a:visited{
            color: orange;
            font-size: 40px;
        }
        /* 鼠标移入 */
        a:hover{
            color: aqua;
        }
        /* 点击时 */
        a:active{
            color: yellowgreen;
        }
    </style>
</head>
<body>
    <a href="https://www.starvistar.com">SVS</a>
    <br>
    <a href="https://www.starvistar123.com">SVS</a>
</body>
</html>
```

## 3.9 伪元素

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=p, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            伪元素：页面中一些特殊的不真实存在的元素
            ::first-letter 第一个字母
            ::first-line 第一行
            ::selection 选中的内容
            ::after 元素的最后
            ::before 元素的开始
                - before 和 after必须结合content属性使用
        */
        p::first-letter{
            font-size: 40px;
        }
        p::first-line{
            background-color: yellow;
        }
        div::before{
            content: 'abc';
            color: red;
        }
    </style>
</head>
<body>
    <div>hello how are you</div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempore voluptatibus repellat dolores sed ex iste illo? A non odit iure alias iusto itaque, vel eius esse aliquam commodi ipsa blanditiis?</p>
</body>
</html>
```

## 3.10 继承

后代元素应用样式，如 p元素中的span

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            样式的继承，后代元素
            并不是所有的元素都会被继承，比如背景，布局相关
        */
        body{
            font-size: 12px;
        }
        p{
            color: red;
        }
    </style>
</head>
<body>
    <p>
        我是一个p元素
        <span>我是p元素中的span</span>
    </p>
</body>
</html>
```

## 3.11 选择器的权重

样式不生效时，思考下权重

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            选择器的权重
            内联样式 1000        1 0 0 0 
            id选择器 100         0 1 0 0
            类/伪类选择器 10     0 0 1 0  
            元素选择器 1         0 0 0 1
            通配选择器 0
            继承没有优先级
            !important 1000

            比较优先级时需要将所有的选择器优先级进行相加计算
            分组选择器是单独计算的
            选择器的累加不会超过最大的数量级，不进位
            !important 开发中慎用，优先级最高
        */
        div{
            color: red !important;
        }
        .red{
            color: yellow;
        }
        *{
            color: blue;
        }

    </style>
</head>
<body>
    <!-- <div id="red" class="red" style="background-color: skyblue;">我是一个div</div> -->
    <div id="red" class="red">我是一个div</div>

</body>
</html>
```

## 3.12 像素和百分比（单位）

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            px 像素
            % 百分比
            vw 窗口宽度的百分比
            vh 窗口高度的百分比
            vmin 窗口最小宽度的百分比
            vmax 窗口最大宽度的百分比
            em 相对自身元素 字体大小计算 font-size
            rem 相对根元素  如html
        */
        html{
            font-size: 10px;
        }
        .box1{
            width: 100px;
            height: 100px;
            background-color: red;
        }
        .box2{
            width: 50%;
            height: 50%;
            background-color: blue;
        }
        .box3{
            width: 50vw;
            height: 50vh;
            background-color: yellow;
        }
        .box4{
            font-size: 5px;
            width: 50em;
            height: 50em;
            background-color: green;
        }
        .box5{
            width: 50rem;
            height: 50rem;
            background-color: pink;
        }
    </style>
</head>
<body>
    <div class="box1">
        <div class="box2"></div>
    </div>
    <div class="box3"></div>
    <div class="box4"></div>
    <div class="box5"></div>
</body>
</html>
```

## 3.13 颜色

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* 
            红绿蓝
            rgba(红,绿,蓝,.5) .5半透明 0表示完全透明
            十六进制 #aabbcc
            HSL色值 hsl(色调,饱和度,亮度)
        */
        .box1{
            width: 100px;
            height: 100px;
            background-color: rgb(255, 0, 0);
        }
    </style>
</head>
<body>
    <div class="box1"></div>
</body>
</html>
```

