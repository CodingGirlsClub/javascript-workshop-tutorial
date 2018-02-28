### 3.1 jQuery是什么

jQuery 是一个跨浏览器的 JavaScript 库， 极大地简化了 JavaScript 编程。例如JavaScript 访问某个 HTML 元素，以下是JavaScript原生实现代码：

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

JavaScript 访问某个 HTML 元素，以下是JQuery实现代码：

```
<!DOCTYPE html>
<html>
<body>

<h1></h1>

<p id="demo">My First Paragraph.</p>

<script>
// 通过指定的 id 来访问 HTML 元素，并改变其内容
$('#demo').html('My First JavaScript');
</script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.js"></script>
</body>
</html>
```



