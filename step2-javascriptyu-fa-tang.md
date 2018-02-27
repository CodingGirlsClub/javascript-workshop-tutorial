## JavaScript语法

### 本章目标：

1. 掌握JavaScript的常用基础语法
2. 掌握JavaScript基础语法学习示例，基本会使用JavaScript完成简单的网页功能

### 一、JS的使用

在HTML中插入JS使用&lt;script&gt;标签，有两种使用方式; 内联方式和外链接方式。

内联方式的JS必须位于**&lt;script&gt; **与** &lt;/script&gt; **标签之间。可以被放置在 HTML 页面的 &lt;body&gt; 和 &lt;head&gt; 部分中。**&lt;script&gt; **与** &lt;/script&gt;** 告诉浏览器在何处开始和结束，**&lt;script&gt; **与** &lt;/script&gt; **之间的代码就是JS脚本。

```
<!DOCTYPE html>
<html>
<head>
  <script>
    alert("My First JavaScript");
  </script>
</head>
<body>
  <script>
    document.write("<h1>This is a heading</h1>");
    document.write("<p>This is a paragraph</p>");
 </script>
</body>
</html>
```

外链接方式是直接通过**&lt;script src="文件后缀以.js结尾的文件地址或者链接"&gt; &lt;/script&gt;**的方式，可以被放置在 HTML 页面的 &lt;body&gt; 和 &lt;head&gt; 部分中。

```
<!DOCTYPE html>
<html>
<head>
  <script src="myScript.js"></script>
</head>
<body>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.js"></script>
</body>
</html>
```

### 二、JS有效代码与 JS注释

JS代码包含有效的执行语句和注部分。JS不会执行注释。

我们可以添加注释来对 JS进行解释提高代码的可读性。

JS代码的注释有行内注释（//）和注释块（/\* 注释内容 \*/）。

单行注释以 // 开头，// 只能在一行中，只有一行中的第一个//有效，第一个//后面的所有本行内的内容均为注释信息。

/\* 注释内容 \*/ 可以跨行，以/\*开始，以\*/结束。

```
<script>
// 这是行内注释
alert("My First JavaScript"); //有效代码
/*
这是注释块，
可多行
*/
</script>
```

### 三、JS操作HTML元素

JavaScript 通常用于操作 HTML 元素。

如需从 JavaScript 访问某个 HTML 元素，您可以使用 document.getElementById\(id\) 方法。

通常使用 "id" 属性来标识 HTML 元素，示例如下：

```
<!DOCTYPE html>
<html>
<body>

<h1></h1>

<p id="demo">My First Paragraph.</p>

<script>
// 通过指定的 id 来访问 HTML 元素，并改变其内容
document.getElementById("demo").innerHTML="My First JavaScript";
</script>

</body>
</html>
```

[在线试一试](http://www.w3school.com.cn/tiy/t.asp?f=js_dom)

又如需要向HTML输出内容，示例如下：

```
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>

<script>
// 向HTML输出内容
document.write("<p>My First JavaScript</p>");
</script>

</body>
</html>
```

[在线试一试](http://www.w3school.com.cn/tiy/t.asp?f=js_write)

**注意： document.write\(\) 仅仅向文档输出写内容。如果在html文档已完成加载后执行 document.write，整个 HTML 页面\(包括原来已经显示在HTML上的内容\)都将被覆盖。**









