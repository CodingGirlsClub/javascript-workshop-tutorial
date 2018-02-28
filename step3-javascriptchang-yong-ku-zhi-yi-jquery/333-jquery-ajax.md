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



