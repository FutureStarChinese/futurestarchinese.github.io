---
layout: post
title:  "Learning HTML DAY 1"
tags:   hello diary
date:   2026-08-19 17:33:35 +0800
categories: [日志] 
---

{% highlight html %}

<!-- 声明使用html(hypertext markup language)5 doc(document)type -->
<!-- 
网络上有很多不同的文件，如果能够正确声明HTML的版本，浏览器就能正确显示网页内容。
doctype 声明是不区分大小写的，以下方式均可：
<!DOCTYPE html>
<!DOCTYPE HTML>
<!doctype html>
<!Doctype Html>

HTML5
<!DOCTYPE html>
HTML 4.01
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
XHTML 1.0
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
-->

<!DOCTYPE html>

<html>

<!-- 头部 -->

<head>
    <!-- 网页编码 中文一般 utf-8 gbk-->
    <meta charset="utf-8">

    <!-- 网页标题 -->
    <title>教程</title>

    <!-- 网页形式 用CSS实现 -->
    <style>
        body {
            /*背景颜色 色号前加# */
            background-color: #383e61;
            /*字体颜色*/
            color: white;
        }
    </style>

</head>

<!-- 网页主体部分 -->

<body>


    <!-- 标题 共6级 -->
    <h2> 标题1 </h2>


    <!-- 水平线 hr(horizontal) -->
    <hr />


    <!-- 段落 p(paragraph) -->
    <!--
    忘记使用结束标签会产生意想不到的结果和错误。
    注释: 在未来的 HTML 版本中，不允许省略结束标签。 
     -->
    <p id="paragraph1" class="paragraph1"> 段落1 </p>


    <!-- 
    当显示页面时，浏览器会移除源代码中多余的空格和空行。
    所有连续的空格或空行都会被算作一个空格。
    需要注意的是，HTML 代码中的所有连续的空行（换行）也被显示为一个空格。
    -->
    <p>
        这个段落
        在源代码 中
        包含 许多行
        但是 浏览器
        忽略了 它们。
    </p>


    <!-- 格式化标签 -->
    <p>
        <strong>strong标签作用为强调加粗</strong><br />
        <em>em(emphasized)标签作用为强调斜体</em><br />
        <b>b(bold)标签作用为加粗</b><br />
        <i>i(italic)标签作用为斜体</i><br />
        <small>small标签作用为缩小</small><br />
        DDD<sub>sub(subscript)标签作用为下标</sub><br />
        DDD<sup>sup(superscript)标签作用为上标</sup><br />
        DDD<ins>ins(insert)标签作用为插入</ins><br />
        DDD<del>del(delete)标签作用为删除字</del><br />
        <code>
            code
        </code>
        <kbd>kbd操作键盘码</kbd>
        <samp>samp sample 计算机代码样</samp>
        <var>var variety 变量</var>
    </p>

    <input type="text" onchange="alert('the value changed!')" />


    <br /> <br />


    <!-- 超链接 href(hypereference) -->
    <a style="color:pink; " href="https://futurestarchinese.github.io" title="你发现了盲点"> 链接 </a>


    <!-- 换行 br(break)  在不产生一个新段落的情况下进行换行 -->
    <br /><br />


    <!-- 图像 src(source)资源的地址 width宽度 height高度 仅指定宽度或高度自适应另一属性 -->
    <img src="./src/81163049_p0.jpg" width="300" alt="图片加载失败" />


    <br /><br />


    <video class="video" src="./src/HELLO MY TREAT.mp4" width="600" alt="视频加载失败"></video>


    <br /> <br />


    <button onclick="alert('Button clicked!')">Click Me!</button>


</body>


</html>

<!--  关于HTML
HTML 指的是超文本标记语言: HyperText Markup Language
HTML 不是一种编程语言，而是一种标记语言
标记语言是一套标记标签 (markup tag)
HTML 使用标记标签来描述网页
HTML 文档包含了HTML 标签及文本内容
HTML文档也叫做 web 页面
-->

<!-- 
HTML 标签 (HTML tag)。

HTML 标签是由尖括号包围的关键词，比如 <html>
HTML 标签通常是成对出现的，比如 <b> 和 </b> 但存在空元素 <br /> 
标签对中的第一个标签是开始标签（开放/起始标签），第二个标签是结束标签（闭合标签）

不区分大小写，但推荐：统一使用小写标签 符合 W3C 规范 提升代码可读性与一致性
-->

<!-- 
HTML 元素 语法规则

元素以开始标签开始，以结束标签结束
部分情况下，浏览器会自动补全缺失的结束标签：
虽然可以正常显示，但不推荐依赖这种行为，可能导致：

元素内容位于开始标签与结束标签之间

部分元素为空元素（empty element），没有内容
空元素通常在开始标签中自闭合（如 <br />）
<br />兼容 HTML、XHTML 和 XML 而某些情况下可以<br>

大多数元素可以包含属性（Attributes）
-->

<!-- 
HTML 属性

HTML 元素可以设置属性
属性可以在元素中添加附加信息
属性一般描述于开始标签
属性总是以名称/值对的形式出现，比如：name="value"。
属性值应该始终被包括在引号内。
双引号是最常用的，不过使用单引号也没有问题，但属性值自身含有双引号则使用单引号，含有单引号则使用双引号
-->

<!-- 
属性名	适用元素	说明
id	所有元素	为元素指定唯一的标识符。
class	所有元素	为元素指定一个或多个类名，用于 CSS 或 JavaScript 选择。
style	所有元素	直接在元素上应用 CSS 样式。
title	所有元素	为元素提供额外的提示信息，通常在鼠标悬停时显示。
data-*	所有元素	用于存储自定义数据，通常通过 JavaScript 访问。
href	<a>, <link>	指定链接的目标 URL。
src	<img>, <script>, <iframe>	指定外部资源（如图片、脚本、框架）的 URL。
alt	<img>	为图像提供替代文本，当图像无法显示时显示。
type	<input>, <button>	指定输入控件的类型（如 text, password, checkbox 等）。
value	<input>, <button>, <option>	指定元素的初始值。
disabled	表单元素	禁用元素，使其不可交互。
checked	<input type="checkbox">, <input type="radio">	指定复选框或单选按钮是否被选中。
placeholder	<input>, <textarea>	在输入框中显示提示文本。
target	<a>, <form>	指定链接或表单提交的目标窗口或框架（如 _blank 表示新标签页）。
readonly	表单元素	使输入框只读。
required	表单元素	指定输入字段为必填项。
autoplay	<audio>, <video>	自动播放媒体。
onclick	所有元素	当用户点击元素时触发 JavaScript 事件。
onmouseover	所有元素	当用户将鼠标悬停在元素上时触发 JavaScript 事件。
onchange	表单元素	当元素的值发生变化时触发 JavaScript 事件。
-->

{% endhighlight %}

regards.
<h4 align = "right">Future Star.</h4>

