# &lt;iframe&gt;

### 说明
&lt;iframe&gt; 标签规定一个内联框架。
一个内联框架被用来在当前 HTML 文档中嵌入另一个文档。


```html
<iframe src="http://www.taobao.com/"></iframe>
```

<iframe src="http://www.taobao.com/"></iframe>

### 属性
- name

name 属性规定 &lt;iframe&gt; 的名称。
&lt;iframe&gt; 元素的 name 属性作为 &lt;a&gt; 或 &lt;form&gt; 元素的 target 属性的值
```html
<iframe src="http://www.baidu.com/" name="rr"></iframe>
<a href="http://www.taobao.com/" target="rr">淘宝网</a>
```
<iframe src="http://www.baidu.com/" name="rr"></iframe>
<a href="http://www.taobao.com/" target="rr">淘宝网</a>

- sandbox

iframe经常会引入一些外部的页面，需要特别注意安全性的问题
如果指定了空字符串（sandbox=""），该属性对呈现在iframe框架中的内容启用一些额外的限制条件。
sandbox 属性的值既可以是一个空字符串（将会启用所有的限制），也可以是用空格分隔的一系列指定的字符串。
HTML 5通过sandbox属性提升iframe的安全性。sandbox属性可以防止不信任的Web页面执行某些操作。
它可以防止如下操作：
- 访问父页面的DOM（从技术角度来说，这是因为相对于父页面iframe已经成为不同的源了）
- 执行脚本
- 通过脚本嵌入自己的表单或是操纵表单
- 对cookie、本地存储或本地SQL数据库的读写

```html
<iframe sandbox=""> 启用所有限制条件
<iframe sandbox="allow-same-origin"> 允许将内容作为普通来源对待。如果未使用该关键字，嵌入的内容将被视为一个独立的源。
<iframe sandbox="allow-top-navigation"> 嵌入的页面的上下文可以导航（加载）内容到顶级的浏览上下文环境（browsing context）。如果未使用该关键字，这个操作将不可用。限制iframe嵌入的页面随意改动父级页面的URL地址
<iframe sandbox="allow-forms"> 允许表单提交。
<iframe sandbox="allow-scripts"> 允许脚本执行。
<iframe sandbox="allow-forms allow-scripts"> 允许表单提交和脚本执行。
```
<a href="http://www.w3school.com.cn/tiy/t.asp?f=html5_iframe_sandbox_form" target="_blank">尝试1</a>
<a href="http://www.w3school.com.cn/tiy/t.asp?f=html5_iframe_sandbox_origin" target="_blank">尝试2</a>



