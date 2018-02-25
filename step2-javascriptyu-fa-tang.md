## JavaScript语法

### 本章目标：

1. 掌握JavaScript的常用基础语法
2. 掌握JavaScript基础语法学习示例，基本会使用JavaScript完成简单的网页功能



一、JS的使用

在HTML中JS有两种使用方式; 内联方式和外链接方式。

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



