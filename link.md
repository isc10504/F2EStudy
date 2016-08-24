# &lt;link&gt;

### 说明
&lt;link&gt; 标签定义文档与外部资源的关系。  
&lt;link&gt; 标签最常见的用途是链接样式表

```html
<head>
    <link rel="stylesheet" type="text/css" href="theme.css">
</head>
```

### 属性
- charset

charset 属性规定被链接文档的字符编码方式
```html
<link href="domoarigato.htm" rel="parent" charset="ISO-2022-JP">
```

- href

href 属性规定外部资源（通常是样式表文件）的位置（URL）。

- media

media 属性规定被链接文档将显示在什么设备上。
该属性通常与 CSS 样式表一起使用，用于为不同的媒介类型规定不同的样式。
media 属性接受若干个值。
```html
<link media="all"> 默认。适用于所有设备
<link media="print"> 打印预览模式/打印页面
<link media="screen"> 计算机屏幕
```
除了设备之外，还可以附加上设备的一些信息，比如宽高，分辨率等，在移动开发中非常重要，可以根据移动设备信息的不同，加载不同的css样式文件
```html
<link media="screen and (min-width:500px)"> 可显示区域的最小宽度
<link media="screen and (max-height:700px)"> 可显示区域的最大高度
<link media="screen and (aspect-ratio:16/9)"> 可显示区域的宽高比
<link media="screen and (device-width:500px)"> 显示器设备本身的宽度
<link media="screen and (device-aspect-ratio:16/9)"> 显示器设备本身的宽高比
<link media="all and (orientation: landscape)"> 显示器设备的方向，例如手机是竖着的
<link media="print and (resolution:300dpi)"> 显示器设备的像素密度
```
<hr>
- rel

rel 属性是必须的，规定当前文档与被链接文档/资源之间的关系
```html
<link rel="stylesheet"> 要导入的样式表
<link rel="icon"> 导入表示该文档的图标
<link rel="alternate"> 链接到该文档的替代版本，常用于引用备选的css样式文件
<link rel="dns-prefetch" href="http://example.com"> 规定应该对目标资源进行预先加载，会预先对example.com这个域名做解析<br>
以下不常用，看看就可以
<link rel="help">   链接到帮助文档
<link rel="license"> 链接到该文档的版权信息
<link rel="next"> 表示该文档是集合中的一部分，且集合中的下一个文档是被引用的文档
<link rel="prev"> 表示该文档是集合中的一部分，且集合中的上一个文档是被引用的文档
<link rel="search"> 链接到针对文档的搜索工具
<link rel="author"> 链接到该文档的作者
```
<hr>
- type

type 属性规定被链接文档/资源的 MIME 类型。
只有当设置了 href 属性时，才能使用该属性。
link 标签常用的 MIME 类型是 "text/css"，它规定样式表。
```html
<link rel="stylesheet" type="text/css" href="theme.css">
```
