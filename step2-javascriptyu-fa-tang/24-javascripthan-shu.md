### 2.4 JavaScript函数

函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。

```
<!DOCTYPE html>
<html>
<head>
<script>
function myFunction(){
    alert("Hello World!");  // JS语句
}
</script>
</head>

<body>
<button onclick="myFunction()">Try it</button>
</body>
</html>
```

## JavaScript 函数语法

函数就是包裹在花括号中的代码块，前面使用了关键词 function：

```
function functionname(){
   //执行代码
}
```

当调用该函数时，会执行函数内的代码。

可以在某事件发生时直接调用函数（比如当用户点击按钮时），并且可由 JavaScript 在任何位置进行调用。

**注意：JavaScript 对大小写敏感。关键词 function 必须是小写的，并且必须以与函数名称相同的大小写来调用函数。**

#### 带有返回值，带参数的函数

在调用函数时，您可以向其传递值，这些值被称为参数。

这些参数可以在函数中使用。

您可以发送任意多的参数，由逗号 \(,\) 分隔，

有时，我们会希望函数将值返回调用它的地方。

通过使用 return 语句就可以实现。

在使用 return 语句时，函数会停止执行，并返回指定的值。

#### 语法

```
myFunction(argument1,argument2){
    // 代码
}
```

示例如下：

```
function myFunction(x, y){
    var z=5; // var 声明JS变量
    return x + y + z; // x + y + z 是JS表达式，return语句的返回时是表达式的计算结果 
}
```



继续了解JavaScript 的事件，作用域，条件语句，循环语句，请前往：http://www.runoob.com/js/js-functions.html



