### 3.3.3 jQueryAjax

AJAX 是与服务器交换数据的技术，它在不重载全部页面的情况下，实现了对部分网页的更新。

[在线点击按钮，通过 jQuery AJAX 改变这段文本。](http://www.w3school.com.cn/tiy/t.asp?f=jquery_ajax_load)

```
<!DOCTYPE html>
<html>
<head>
<script src="/jquery/jquery-1.11.1.min.js">
</script>
<script>
$(document).ready(function(){
  $("#btn1").click(function(){
    $('#test').load('/example/jquery/demo_test.txt');
  })
})
</script>
</head>

<body>

<h3 id="test">请点击下面的按钮，通过 jQuery AJAX 改变这段文本。</h3>
<button id="btn1" type="button">获得外部的内容</button>

</body>
</html>
```

#### 什么是 AJAX？

AJAX = 异步 JavaScript 和 XML（Asynchronous JavaScript and XML）。

简短地说，在不重载整个网页的情况下，AJAX 通过后台加载数据，并在网页上进行显示。

使用 AJAX 的应用程序案例：yy.com等几乎所有的网站。

#### 关于 jQuery 与 AJAX

jQuery 提供多个与 AJAX 有关的方法。

通过 jQuery AJAX 方法，您能够使用 HTTP Get 和 HTTP Post 从远程服务器上请求文本、HTML、XML 或 JSON - 同时您能够把这些外部数据直接载入网页的被选元素中。

#### jQuery load\(\) 方法

jQuery load\(\) 方法是简单但强大的 AJAX 方法。

load\(\) 方法从服务器加载数据，并把返回的数据放入被选元素中。

**语法:**

```
$(selector).load(URL,data,callback);
```

必需的URL参数规定您希望加载的 URL。

可选的data参数规定与请求一同发送的查询字符串键/值对集合。

可选的callback参数是 load\(\) 方法完成后所执行的函数名称。

这是示例文件（"demo\_test.txt"）的内容：

```
<h2>jQuery AJAX 是个非常棒的功能！</h2>
<p id="p1">这是段落的一些文本。</p>
```

下面的例子会把文件 "demo\_test.txt" 的内容加载到指定的 &lt;div&gt; 元素中：

```
$("#div1").load("demo_test.txt");
```

也可以把 jQuery 选择器添加到 URL 参数。

下面的例子把 "demo\_test.txt" 文件中 id="p1" 的元素的内容，加载到指定的 &lt;div&gt; 元素中：

```
$("#div1").load("demo_test.txt #p1");
```

可选的 callback 参数规定当 load\(\) 方法完成后所要允许的回调函数。回调函数可以设置不同的参数：

* responseTxt
  * 包含调用成功时的结果内容
* statusTXT
  * 包含调用的状态
* xhr
  * 包含 XMLHttpRequest 对象

下面的例子会在 load\(\) 方法完成后显示一个提示框。如果 load\(\) 方法已成功，则显示"外部内容加载成功！"，而如果失败，则显示错误消息：

```
$("button").click(function(){
  $("#div1").load("demo_test.txt",function(responseTxt,statusTxt,xhr){
    if(statusTxt=="success")
      alert("外部内容加载成功!");
    if(statusTxt=="error")
      alert("Error: "+xhr.status+": "+xhr.statusText);
  });
});
```

#### HTTP 请求：GET vs. POST

jQuery get\(\) 和 post\(\) 方法用于通过 HTTP GET 或 POST 请求从服务器请求数据。

两种在客户端和服务器端进行请求-响应的常用方法是：GET 和 POST。

* _GET_
  * 从指定的资源请求数据
* _POST_
  * 向指定的资源提交要处理的数据

GET 基本上用于从服务器获得（取回）数据。注释：GET 方法可能返回缓存数据。

POST 也可用于从服务器获取数据。不过，POST 方法不会缓存数据，并且常用于连同请求一起发送数据。

#### jQuery $.get\(\) 方法

$.get\(\) 方法通过 HTTP GET 请求从服务器上请求数据。

#### 语法：

```
$.get(URL,callback);
```

必需的URL参数规定您希望请求的 URL。

可选的callback参数是请求成功后所执行的函数名。

下面的例子使用 $.get\(\) 方法从服务器上的一个文件中取回数据：

```
$("button").click(function(){
  $.get("demo_test.json",function(data,status){
    alert("数据: " + data.test + "\n状态: " + status);
  });
});
```

$.get\(\) 的第一个参数是我们希望请求的 URL（"demo\_test.json"）。

第二个参数是回调函数。第一个回调参数存有被请求页面的内容，第二个回调参数存有请求的状态。

**提示：**这个JSON 文件 \("demo\_test.json"\) 类似这样：

```
{"test": "这是个从JSON文件中读取的数据。"}
```











