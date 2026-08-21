---
layout: post
title:  "Learning HTML DAY 3"
tags:   HTML 
date:   2026-08-21 11:46:35 +0800
categories: [日志] 
---



### html颜色
``` html
<!DOCTYPE html>

<html>

  

<head>

    <title>html颜色</title>

    <meta charset="utf-8" />

</head>

  

<body>

  

    <h2>html颜色</h2>

    <hr />

  

    <!-- html颜色由#开头的十六进制值表示 分别表示红、绿、蓝（RGB）三个颜色分量 -->

    <div style="background:#000000; height: 10px;"></div>

    <div style="background:#080000; height: 10px;"></div>

    <div style="background:#100000; height: 10px;"></div>

    <div style="background:#180000; height: 10px;"></div>

    <div style="background:#200000; height: 10px;"></div>

    <div style="background:#280000; height: 10px;"></div>

    <div style="background:#300000; height: 10px;"></div>

    <div style="background:#380000; height: 10px;"></div>

    <div style="background:#400000; height: 10px;"></div>

    <div style="background:#480000; height: 10px;"></div>

    <div style="background:#500000; height: 10px;"></div>

    <div style="background:#580000; height: 10px;"></div>

    <div style="background:#600000; height: 10px;"></div>

    <div style="background:#680000; height: 10px;"></div>

    <div style="background:#700000; height: 10px;"></div>

    <div style="background:#780000; height: 10px;"></div>

    <div style="background:#800000; height: 10px;"></div>

    <div style="background:#880000; height: 10px;"></div>

    <div style="background:#900000; height: 10px;"></div>

    <div style="background:#980000; height: 10px;"></div>

    <div style="background:#A00000; height: 10px;"></div>

    <div style="background:#A80000; height: 10px;"></div>

    <div style="background:#B00000; height: 10px;"></div>

    <div style="background:#B80000; height: 10px;"></div>

    <div style="background:#C00000; height: 10px;"></div>

    <div style="background:#C80000; height: 10px;"></div>

    <div style="background:#D00000; height: 10px;"></div>

    <div style="background:#D80000; height: 10px;"></div>

    <div style="background:#E00000; height: 10px;"></div>

    <div style="background:#E80000; height: 10px;"></div>

    <div style="background:#F00000; height: 10px;"></div>

    <div style="background:#F80000; height: 10px;"></div>

    <div style="background:#FF0000; height: 10px;"></div>

  

    <hr />

    <div style="background:#000000; height: 10px;"></div>

    <div style="background:#FF0000; height: 10px;"></div>

    <div style="background:#00FF00; height: 10px;"></div>

    <div style="background:#0000FF; height: 10px;"></div>

    <div style="background:#FFFF00; height: 10px;"></div>

    <div style="background:#00FFFF; height: 10px;"></div>

    <div style="background:#FF00FF; height: 10px;"></div>

    <div style="background:#FFFFFF; height: 10px;"></div>

  

    <!-- 灰度颜色 -->

    <hr />

    <div style="background:#000000; height: 10px;"></div>

    <div style="background:#111111; height: 10px;"></div>

    <div style="background:#222222; height: 10px;"></div>

    <div style="background:#333333; height: 10px;"></div>

    <div style="background:#444444; height: 10px;"></div>

    <div style="background:#555555; height: 10px;"></div>

    <div style="background:#666666; height: 10px;"></div>

    <div style="background:#777777; height: 10px;"></div>

    <div style="background:#888888; height: 10px;"></div>

    <div style="background:#999999; height: 10px;"></div>

    <div style="background:#AAAAAA; height: 10px;"></div>

    <div style="background:#BBBBBB; height: 10px;"></div>

    <div style="background:#CCCCCC; height: 10px;"></div>

    <div style="background:#DDDDDD; height: 10px;"></div>

    <div style="background:#EEEEEE; height: 10px;"></div>

    <div style="background:#FFFFFF; height: 10px;"></div>

  

    <!-- 当大多数计算机仅支持 256 种颜色的时候，一系列 216 种 Web 安全色作为 Web 标准被建议使用。 -->

    <!-- RGB每个通道有6个级别 (0, 33, 66, 99, CC, FF) -->

    <!-- 因此，6 x 6 x 6 = 216 种颜色 -->

  

    <!-- html标准颜色名 17+124 -->

    <hr />

    <div style="background:black; height: 10px;"></div>

    <div style="background:blue; height: 10px;"></div>

    <div style="background:aqua; height: 10px;"></div>

    <div style="background:Fuchsia; height: 10px;"></div>

    <div style="background:gray; height: 10px;"></div>

    <div style="background:green; height: 10px;"></div>

    <div style="background:lime; height: 10px;"></div>

    <div style="background:maroon; height: 10px;"></div>

    <div style="background:navy; height: 10px;"></div>

    <div style="background:olive; height: 10px;"></div>

    <div style="background:purple; height: 10px;"></div>

    <div style="background:red; height: 10px;"></div>

    <div style="background:silver; height: 10px;"></div>

    <div style="background:teal; height: 10px;"></div>

    <div style="background:white; height: 10px;"></div>

    <div style="background:yellow; height: 10px;"></div>

  
  

</body>

  

</html>
```

### html实体字符
``` html
<!DOCTYPE html>

<html>

  

<head>

    <title>html实体字符</title>

    <meta charset="utf-8" />

    <style>

        body {

            background-color: #383e61;

            color: white;

        }

    </style>

</head>

  

<body>

  

    <h2>html实体字符</h2>

    <hr />

    <!-- html实体字符用于表示特殊字符 &名称; &#数字（支持更好）; -->

    <!-- &lt; &#060(&#60)  表示小于号 less than < -->

    <!-- &gt; &#062  表示大于号 greater than > -->

    <!-- &amp; &#038  表示和号 ampersand & -->

    <!-- &quot; &#034  表示双引号 quotation mark " -->

    <!-- &apos; &#039  表示单引号 apostrophe ' -->

    <!-- &nbsp; &#160  表示空格 non-breaking space -->

    <p>&lt;div&gt;这是一个div元素&lt;/div&gt;</p>

    <p>&lt;p&gt;这是一个段落元素&lt;/p&gt;</p>

    <p>&lt;a href=&quot;#&quot;&gt;这是一个链接&lt;/a&gt;</p>

    <p>&lt;br /&gt;这是一个换行符</p>

    <p>&lt;hr /&gt;这是一个水平线</p>

    <p>&lt;!-- 这是一个注释 --&gt;</p>

  

    <!-- 结合音标符 尖音符 抑音符 -->

    <p>a&#768; 这是一个带有尖音符的a</p>

    <p>a&#769; 这是一个带有抑音符的a</p>

    <p>a&#770; 这是一个带有的a</p>

    <p>a&#771; 这是一个带有的a</p>

  

    <!-- 货币 -->

    <p>&#36; &dollar; 这是一个美元符号</p>

    <p>&#165; &yen; 这是一个日元符号</p>

    <p>&#8364; &euro; 这是一个欧元符号</p>

  

    <!-- 其它常用实体字符 -->

    <p>&#169; &copy; 这是一个版权符号</p>

    <p>&#174; &reg; 这是一个注册商标符号</p>

    <p>&#8482; &trade; 这是一个商标符号</p>

  

</body>

  

</html>
```

html布局
``` html

<!DOCTYPE html>

  

<html>

  

<head>

  

    <title>HTML布局</title>

    <meta charset="UTF-8">

    <style>

        body {

            background-color: #383e61;

            color: white;

        }

    </style>

  

</head>

  

<body>

  

    <h2>HTML布局</h2>

  

    <!-- div division 区块元素（单独占行） 用于将元素组合起来 -->

    <!-- span 内联元素 （不单独占行） 也用于将元素组合起来 -->

    <div id="container" style="width: 100%;">

  

        <div id="header" style="background-color: orange; color: blue;">

            <!-- margin-bottom属性用于设置元素下方的外边距 -->

            <h1 style="margin-bottom:0;">头部</h1>

        </div>

  

        <!-- float属性用于设置元素的浮动 -->

        <div id="menu" style="background-color: black;color: white; float: left; width: 20% ; height: 1000px; ">

            <h2 align="center">菜单</h2>

            菜单1<br>菜单2<br>菜单3<br>菜单4<br>菜单5<br>菜单6<br>菜单7<br>菜单8<br>菜单9<br>菜单10

        </div>

  

        <div id="content" style="background-color: green; color: white; float: left; width: 80% ; height: 1000px; ">

            <h2 align="center">内容</h2>

            <p>内容</p>

        </div>

  

        <!-- clear属性用于清除浮动 -->

        <div id="footer" style="background-color: red; color: white; clear: both;">

            <h2 align="center">底部</h2>

  

        </div>

  

    </div>

  

</body>

  
  
  

</html>
```


regards.
<h4 align = "right">Future Star.</h4>

