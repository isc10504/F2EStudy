# &lt;base&gt;

### 说明
&lt;base&gt;标签为页面上的所有的相对链接规定默认 URL前缀 和默认目标。
在一个文档中，最多能使用一个 &lt;base&gt; 标签。&lt;base&gt; 标签必须位于 &lt;head&gt; 标签内部。
```html
<head>
    <base href="http://www.taobao.com/images/" target="_blank">
</head>

<body>
    <img src="stickman.gif" width="24" height="39" alt="Stickman">
    <a href="http://www.taobao.com/">淘宝网</a>
</body>
```



### 属性
- href

相对链接的URL前缀

- target

与&lt;a&gt;标签的target属性一样
