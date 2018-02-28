### 3.3.1 jQuery选择器

jQuery 语法是通过选取 HTML 元素，并对选取的元素执行某些操作。

jQuery 选择器允许您对 HTML 元素组或单个元素进行操作。

jQuery 选择器基于元素的 id、类、类型、属性、属性值等"查找"（或选择）HTML 元素。 它基于已经存在的[CSS 选择器](http://www.runoob.com/cssref/css-selectors.html)，除此之外，它还有一些自定义的选择器。

jQuery 中所有选择器都以美元符号开头：$\(\)。

**基础语法：$\(selector\).action\(\)**

* 美元符号定义 jQuery
* 选择符（selector）"查询"和"查找" HTML 元素
* jQuery 的 action\(\) 执行对元素的操作

实例:

* $\(this\).hide\(\) - 隐藏当前元素

* $\("p"\).hide\(\) - 隐藏所有 &lt;p&gt; 元素  \(jQuery 元素选择器基于元素名选取元素。\)

* $\(".test"\).hide\(\) - 隐藏所有 class="test" 的 &lt;p&gt; 元素 \(jQuery 类选择器可以通过指定的 class 查找元素。\)

* $\("\#test"\).hide\(\) - 隐藏所有 id="test" 的元素 \(jQuery \#id 选择器通过 HTML 元素的 id 属性选取指定的元素。\)

```
$("p").css("background-color","red");
```

[在线试一试](http://www.w3school.com.cn/tiy/t.asp?f=jquery_css_change_p)

**文档就绪事件：**

在我们的实例中的所有 jQuery 函数位于一个 document ready 函数中：

```
$(document).ready(function(){

 //jQuery functions go here

});
```

这是为了防止文档在完全加载（就绪）之前运行 jQuery 代码，即在 DOM 加载完成后才可以对 DOM 进行操作。

如果在文档没有完全加载之前就运行函数，操作可能失败。下面是两个具体的例子：

* 试图隐藏一个不存在的元素
* 获得未完全加载的图像的大小

**提示：**简洁写法（与以上写法效果相同）:

```
$(function(){
/* jQuery functions go here */

});
```



