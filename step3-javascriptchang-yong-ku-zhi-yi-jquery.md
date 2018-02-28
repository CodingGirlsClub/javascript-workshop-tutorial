### 3. JavaScript常用库之一jQuery

jQuery 是一个 JavaScript 库。 

jQuery 极大地简化了 JavaScript 编程。

```
<html>
<head>
<script type="text/javascript" src="jquery.js"></script>
<script type="text/javascript">
$(document).ready(function(){
  $("p").click(function(){
  $(this).hide();
  });
});
</script>
</head>

<body>
<p>If you click on me, I will disappear.</p>
</body>

</html> 
```

在线试一试









