---
layout: post
title:  "Learning CSS DAY 1"
tags:   HELLO CSS
date:   2026-08-21 13:55:35 +0800
categories: [日志] 
---

### css简介

<hr>

CSS 指层叠样式表 Cascading Style Sheets

  

#### css规则

``` css

h1 {

    color:red;

    text-align:center;

}

```

格式：选择器{属性:值;} <br/>

**不要忘记大括号、冒号、分号**

  

#### css注释

``` css

/* */

```

css注释以`/*`开始 以`*/`结束

  

### css选择器

<hr>

  

#### css id选择器

``` css

#para1

{

    color: red;

    text-align:left;

}

```

id选择器以`#`开头，和html文件中的id对应<br>

id是唯一的

  

#### css class选择器

``` css

.center{text-align:center;}

p.center{text-align:center;}

```

class选择器为`.` 与html文件中的class对应 可以在`.`前指定选择的标签<br>

class不是唯一的

  

### css创建

<hr>

  

#### 外部样式表

需要html文件内用`<link>`连接

``` html

<link rel="stylesheet" type="text/css" href="style.css">

```

  

#### 内部样式表

需要在html文件内创建

``` html

<!DOCTYPE html>

<html>

<head>

    <style>

        p{

            background-color:red;

        }

    </style>

</head>

</html>

```

  

#### 内联样式

在html标签中用style属性创建

``` html

<a href="www.bilibili.com" style="color:red;"> bilibili </a>

```

  

#### 多重样式的顺序

当样式在某一级样式表中唯一存在时，使用唯一的样式<br>

当不唯一存在时

```

（内联样式）Inline style > （内部样式）Internal style sheet >（外部样式）External style sheet > 浏览器默认样式

```

regards.
<h4 align = "right">Future Star.</h4>

