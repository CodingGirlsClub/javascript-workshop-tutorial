### 2.3 JS操作HTML元素

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
// 使用注释来阻止执行
//document.getElementById("myH1").innerHTML="Welcome to my Homepage";
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

