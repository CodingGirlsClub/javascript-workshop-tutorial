### 3.3.2 jQuery 事件

jQuery 是为事件处理特别设计的。

#### 什么是事件？

页面对不同访问者的响应叫做事件。

事件处理程序指的是当 HTML 中发生某些事件时所调用的方法。

实例：

* 在元素上移动鼠标。
* 选取单选按钮
* 点击元素

在事件中经常使用术语"触发"（或"激发"）例如： "当您按下按键时触发 keypress 事件"。

常见 DOM 事件：

| 鼠标事件 | 键盘事件 | 表单事件 | 文档/窗口事件 |
| :--- | :--- | :--- | :--- |
| [click](http://www.runoob.com/jquery/event-click.html) | [keypress](http://www.runoob.com/jquery/event-keypress.html) | [submit](http://www.runoob.com/jquery/event-submit.html) | [load](http://www.runoob.com/jquery/event-load.html) |
| [dblclick](http://www.runoob.com/jquery/event-dblclick.html) | [keydown](http://www.runoob.com/jquery/event-keydown.html) | [change](http://www.runoob.com/jquery/event-change.html) | [resize](http://www.runoob.com/jquery/event-resize.html) |
| [mouseenter](http://www.runoob.com/jquery/event-mouseenter.html) | [keyup](http://www.runoob.com/jquery/event-keyup.html) | [focus](http://www.runoob.com/jquery/event-focus.html) | [scroll](http://www.runoob.com/jquery/event-scroll.html) |
| [mouseleave](http://www.runoob.com/jquery/event-mouseleave.html) |  | [blur](http://www.runoob.com/jquery/event-blur.html) | [unload](http://www.runoob.com/jquery/event-unload.html) |

## jQuery 事件方法语法

在 jQuery 中，大多数 DOM 事件都有一个等效的 jQuery 方法。

页面中指定一个点击事件：

```
$("p").click();
```

下一步是定义什么时间触发事件。您可以通过一个事件函数实现：

```
$("p").click(function(){
    // 动作触发后执行的代码!!
});
```

* 常用的jQuery事件方法的说明与示例详见[http://www.runoob.com/jquery/jquery-events.html](http://www.runoob.com/jquery/jquery-events.html)
* jQuery还能实现隐藏、显示、切换，滑动，淡入淡出，以及动画等效果；详细的说明和示例详见[http://www.runoob.com/jquery/jquery-hide-show.html](http://www.runoob.com/jquery/jquery-hide-show.html)
* jQuery操作HTML元素和属性详细的说明和示例详见http://www.runoob.com/jquery/jquery-dom-get.html



