# &lt;a&gt;

### 说明
&lt;a&gt;标签定义一个超链接，用于在一个指定的窗口中打开一个指定的页面
```html
<a href="http://www.taobao.com/" target="_blank" title="淘啊淘，淘你喜欢！">淘宝网</a>
```
<a href="http://www.taobao.com/" target="_blank" title="淘啊淘，淘你喜欢！" rel="nofollow">淘宝网</a>

### 属性
- href

```html
<a href="http://www.taobao.com/"> 要打开页面的URL地址
<a href="#rr"> 快速跳转到页面内部id是"rr"的元素位置
```

- target

```html
<a target="_self"> 在当前窗口打开指定页面，默认值
<a target="_blank"> 在一个新的窗口中打开指定页面
<a target="_parent"> 当出现页面嵌套时，在父级窗口中打开指定页面，如果没有页面嵌套，则等于_self
<a target="_top"> 当出现页面嵌套时，在最外层窗口中打开指定页面，如果没有页面嵌套，则等于_self
<a target="rr"> 在一个名字为"rr"的窗口中打开指定页面，如果此窗口不存在，则会先新建一个名字为"rr"的窗口
```
- rel

```html
<a rel="nofollow"> 规定当前页面与超链接指向的页面 之间的关系，最常用的一个值nofollow，告诉搜索引擎的爬虫，不要继续抓取这个超链接指向的页面
```


- title  

设置超链接的提示信息，当鼠标移到超链接上，并且停留一段时间，提示信息就会显示