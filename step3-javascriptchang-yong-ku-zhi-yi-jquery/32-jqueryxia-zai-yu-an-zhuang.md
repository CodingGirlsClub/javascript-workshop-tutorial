### **3.2 jQuery的下载与安装**

#### 下载

有两个版本的 jQuery 可供下载：

* Production version - 用于实际的网站中，已被精简和压缩。
* Development version - 用于测试和开发（未压缩，是可读的代码）

这两个版本都可以从[jQuery.com](http://jquery.com/download/)下载。

提示：您可以把下载文件放到与页面相同的目录中，这样更方便使用。

#### 替代方案

如果您不希望下载并存放 jQuery，那么也可以通过 CDN（内容分发网络） 引用它。

[https://cdnjs.com/libraries/jquery](https://cdnjs.com/libraries/jquery)

以上链接提供了jQuery所有的版本，目前最新版本是[3.3.1](https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.js)

#### 安装

使用 HTML 的 &lt;script&gt; 标签引用它，可以放在&lt;head&gt;或者&lt;body&gt;中。

1.下载到本地

```
<head>
<script src="jquery.js"></script>
</head>
```

2.通过CDN

```
<head>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.js"></script>
</script>
</head>
```



