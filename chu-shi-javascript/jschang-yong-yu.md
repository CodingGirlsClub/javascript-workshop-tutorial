### 1.1 JavaScript（简称JS）常用术语

* #### JS数据类型

  字符串（String）、数字\(Number\)、布尔\(Boolean\)、数组\(Array\)、对象\(Object\)、空（Null）、未定义（Undefined）。

* #### JS变量

  ECMAScript 中的变量是用 var 运算符（variable 的缩写）加变量名定义的。

  变量的数据类型拥有动态能力，它的类型取决于当前值的数据类型。

* #### JS运算符

  JS运算符分为JS算术运算符和JS赋值运算符。

  ##### JS算术运算符：用于执行变量与/或值之间的算术运算。

| **运算符** | **描述** | **例子** | **结果** |
| :---: | :---: | :---: | :---: |
| + | 加 | x=y+2 | x=7 |
| - | 减 | x=y-2 | x=3 |
| \* | 乘 | x=y\*2 | x=10 |
| / | 除 | x=y/2 | x=2.5 |
| % | 求余数 \(保留整数\) | x=y%2 | x=1 |
| ++ | 累加 | x=++y | x=6 |
| -- | 递减 | x=--y | x=4 |

##### JS赋值运算符：用于给 JS 变量赋值。

| **运算符** | **例子** | **等价于** | **结果** |
| :---: | :---: | :---: | :---: |
| = | x=y |  | x=5 |
| += | x+=y | x=x+y | x=15 |
| -= | x-=y | x=x-y | x=5 |
| \*= | x\*=y | x=x\*y | x=50 |
| /= | x/=y | x=x/y | x=2 |
| %= | x%=y | x=x%y | x=0 |

* #### JS表达式

JS表达式是由运算元和运算符\\(可选\\)构成，并产生运算结果的语法结构。

以下在ES5中被称为**基本表达式（Primary Expression）**

* this、null、arguments等内置的关键字
* 变量。即一个已声明的标识符
* 字面量。仅包括数字字面量、布尔值字面量、字符串字面量、正则字面量
* 分组表达式，即用来表示立刻进行计算的

这类表达式是原子表达式**，是无法再分解的表达式。**

除基本表达式以外，还有由多个原子表达式组合成一个表达式，称为**复杂表达式。**

* #### JS语句

JS 语句向浏览器发出的命令。语句的作用是告诉浏览器该做什么。通常我们在每条可执行的语句结尾添加分号。

* #### JS函数

JS函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。

* #### JS对象

JS 对象是拥有属性\(变量\)和方法\(函数\)的数据。

* #### JS关键字

  ECMA-262 定义了 ECMAScript 支持的一套_关键字（keyword）_。 这些关键字标识了 ECMAScript 语句的开头和/或结尾。根据规定，关键字是保留的，不能用作变量名或函数名。CMAScript 关键字的完整列表：

```
break
case
catch
continue
default
delete
do
else
finally
for
function
if
in
instanceof
new
return
switch
this
throw
try
typeof
var
void
while
with
```

* #### HTML DOM\(Document Object Model 文档对象模型\)

当网页被加载时，浏览器会创建页面的文档对象模型，**HTML DOM**模型被构造为**对象**的树：

![](/assets/HTMLDOM.png)

* #### BOM \(Browser Object Model 浏览器对象模型\)

浏览器对象模型 \(BOM\) 使 JavaScript 有与浏览器"对话"的能力。

* #### Window 对象

所有浏览器都支持 window 对象。它表示浏览器窗口。

所有 JavaScript 全局对象、函数以及变量均自动成为 window 对象的成员。

全局变量是 window 对象的属性。

全局函数是 window 对象的方法。

甚至 HTML DOM 的 document 也是 window 对象的属性之一：

* #### JS 框架（库）

JavaScript 高级程序设计（特别是对浏览器差异的复杂处理），通常很困难也很耗时。

为了应对这些调整，许多的**JavaScript \(helper\)**库应运而生。这些 JavaScript 库常被称为**JavaScript 框架**。

在本教程中，我们将了解到一些广受欢迎的 JavaScript 框架 jQuery。有兴趣也可以自己去了解一下目前最流行的一些框架，比如Vue, React等。所有这些框架都提供针对常见 JavaScript 任务的函数，包括动画、DOM 操作以及 Ajax 处理等。

