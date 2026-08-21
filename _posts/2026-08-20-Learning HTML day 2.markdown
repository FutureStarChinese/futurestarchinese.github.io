---
layout: post
title:  "Learning HTML DAY 2"
tags:   HTML 
date:   2026-08-20 22:51:35 +0800
categories: [日志] 
---



### html表单

``` html

<!DOCTYPE html>

<html>

<head>
    <title>html表格</title>
    <meta charset="utf-8" />
    <style>
        body {
            background-color: #383e61;
            color: white;
        }
    </style>

</head>

<body>

    <h2>html表单</h2>
    <hr />
    <!-- form表单是一个包含表单元素的区域，允许用户输入数据 -->
    <!-- action属性指定表单提交后跳转的URL method属性指定提交方法 post提交给服务器 get存储在url内并跳转url /?page=1 用于存储不重要的信息 -->
    <!-- 示例：?firstname=1&lastname=2&password=3&gender=male&subscribe=subscrible&hobbies=reading&hobbies=traveling&hobbies=sports -->
    <form name="signup" action="html图像.html" method="get">
        <!-- fieldset用于对表单元素进行分组，使用外框包含起来 -->
        <fieldset>
            <!-- legend用于为fieldset提供标题 -->
            <legend>注册表单</legend>
            <!-- input通过指定type属性来定义不同的输入类型 name属性用于标识表单元素 value属性用于指定默认值 -->
            <!-- text类型为正常的文本输入 -->
            First name:<input type="text" name="firstname" required autocomplete="given-name"><br>

            <!-- datalist用于提供下拉选项(类似于浏览器提供，非强制) id必须和input标签的list属性对应 -->
            <datalist id="lastname">
                <option value="Zhang">
                <option value="Li">
                <option value="Wang">
            </datalist>

            Last name:<input type="text" name="lastname" required autocomplete="family-name" list="lastname"><br>

            <!-- select类型用于下拉菜单 -->
            age range:<select name="age" required>
                <!-- optgroup类型用于组合选项 -->
                <optgroup label="under 18">
                    <!-- option类型用于创建选项 -->
                    <option value="0-18">0-18</option>
                </optgroup>
                <optgroup label="18-50">
                    <option value="19-30" selected>19-30</option>
                    <option value="31-50">31-50</option>
                </optgroup>
                <optgroup label="51+">
                    <option value="51+">51+</option>
                </optgroup>
            </select><br>

            age:0<input type="range" name="age" min="0" max="100" required autocomplete="off">100<br>

            <!-- password类型用于输入密码，输入内容会被隐藏 -->
            Password:<input type="password" name="password" required autocomplete="new-password" value="123456"><br>

            <!-- radio类型用于单选按钮，name相同的单选按钮只能选择一个，value属性用于指定选中时的值 -->
            Gender:<input type="radio" name="gender" value="male" autocomplete="sex"> Male
            <input type="radio" name="gender" value="female" autocomplete="sex"> Female<br>

            <!-- checkbox类型用于复选框，name相同的复选框可以选择多个，value属性用于指定选中时的值 -->
            Subscribe:<input type="checkbox" name="subscribe" value="subscrible" checked> Yes<br>
            Hobbies:<input type="checkbox" name="hobbies" value="reading" autocomplete="hobby"> Reading
            <input type="checkbox" name="hobbies" value="traveling" autocomplete="hobby"> Traveling
            <input type="checkbox" name="hobbies" value="sports" autocomplete="hobby"> Sports<br>

            <!-- textarea类型用于文本框 多行 其中文本不会省略空格 -->
            Other message you want to tell us:<br />
            <textarea name="message" rows="5" cols="40"> 文本框 </textarea><br />

            <!-- submit类型用于提交表单，提交完成后会依照action动作执行文件，value值用于指定按钮上显示的文本 -->
            <input type="submit" value="Submit">

            <!-- button类型用于创建按钮 -->
            <input type="button" value="Cancel">

            <!-- reset类型用于重置表单 -->
            <input type="reset" value="Reset">
        </fieldset>
    </form>

</body>

<!-- 
selected属性用于<select>标签指定默认选中的选项
required属性用于<input>标签指定必填项
checked属性用于<input>标签指定默认选中的复选框或单选框
autocomplete属性用于<input>标签指定是否启用自动完成功能
    on开启自动完成功能，off关闭自动完成功能，
    name自动填写姓名，given-name自动填写名字，
    family-name自动填写姓氏，
    mail自动填写邮箱，
    username自动填写用户名，
    new-password自动填写新密码，c
    current-password自动填写当前密码
-->

</html>

```

### html表格

``` html
<!DOCTYPE html>

<html>

<head>
    <title>html表格</title>
    <meta charset="utf-8" />
    <style>
        body {
            background-color: #383e61;
            color: white;
        }
    </style>
</head>

<body>

    <h2>表格</h2>
    <hr>
    <!-- 表格以<table>开始 属性border边界 cellspacing单元格间距 cellpadding单元格填充 -->
    <table border="1" cellspacing="5" cellpadding="5">
        <!-- caption(说明文字)表示表格标题 -->
        <caption>学生信息表</caption>
        <colgroup>
            <!-- col表示列 可以指定样式 通过span批量指定列 -->
            <col span="2" style="background-color: #ff0000">
            <col span="2" style="background-color: #ff00f7">
        </colgroup>
        <!-- thead表示表格头部，可以不指定，指定时通常和tbody、tfoot一起使用 -->
        <thead>
            <!-- tr表示table row 一行表格 -->
            <tr>
                <th>姓名</th>
                <th>年龄</th>
                <th>城市</th>
                <th>居住地</th>
            </tr>
        </thead>
        <!-- tbody表示表格主体，可以不指定，指定时通常和thead、tfoot一起使用 -->
        <tbody>
            <tr>
                <!-- td表示table data单元格 -->
                <td>张三</td>
                <!-- rowspan="2" row span 表示单元格跨越两行 -->
                <td rowspan="2">25</td>
                <!-- colspan="2" column span 表示单元格跨越两列 -->
                <td colspan="2">北京</td>
            </tr>
            <tr>
                <td>李四</td>
                <!-- 列跨度自动省略掉 -->
                <td>上海</td>
                <td>北京</td>
            </tr>
        </tbody>
        <!-- tfoot表示表格尾部，可以不指定，指定时通常和thead、tbody一起使用 -->
        <tfoot>
            <tr>
                <td colspan="4" style="background-color: #383e61;">表格尾部</td>
            </tr>
        </tfoot>

    </table>


</body>

</html>

```


### html框架
``` html
<!DOCTYPE html>

<html>

<head>
    <title>html框架</title>
    <meta charset="utf-8" />
    <style>
        body {
            background-color: #383e61;
            color: white;
        }
    </style>
</head>

<body>

    <h2>html框架</h2>
    <hr />
    <!-- <iframe> 标签用于在当前页面中嵌入另一个页面，src 属性指定要嵌入的页面的 URL -->
    <!-- width指定宽度，height指定高度，可以按照比例指定 -->
    <!-- frameborder指定是否含有边框 -->
    <iframe src="html表单.html" width="60%" height="500 px" frameborder="0" name="iframe_a"></iframe>


    <br />
    <!-- 与超链接的配合 a target-> iframe name -->
    <a href="html表格.html" target="iframe_a">跳转到表格</a>

    <br /><br />
    <iframe src="https://futurestarchinese.github.io/" width="100%" height="1000px" frameborder="0"
        name="iframe_b"></iframe>

</body>

</html>
```

### html图像

``` html
<!DOCTYPE html>

<html>

<head>
    <title>html表格</title>
    <meta charset="utf-8" />
    <style>
        body {
            background-color: #383e61;
            color: white;
        }
    </style>
</head>

<body>
    <h2>html图像</h2>
    <hr />
    <!-- <img> 标签用于插入图像，src 属性指定图像的路径，alt 属性指定图像无法加载时的替代文本 -->
    <!-- width表示宽度 height表示高度 单一指定属性时另外一属性会自动调整 -->
    <img src="./src/81163049_p0.jpg" alt="图片1" width="200" />
    <img src="./src/81163049_p0.jpg" alt="图片2" height="200" />
    <img src="./src/81163049_p0.jpg" alt="图片3" width="200" height="200" />
</body>


</html>
```

regards.
<h4 align = "right">Future Star.</h4>

