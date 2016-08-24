# &lt;button&gt;

### 说明
&lt;button&gt; 标签定义一个按钮。和&lt;input&gt;标签创建的按钮有点类似。
在 &lt;button&gt; 元素内部，您可以放置内容，比如文本或图像。这是该元素与使用 &lt;input&gt; 元素创建的按钮之间的不同之处。

```html
<button type="button">点我!</button> 
<button type="button">
    <img src="https://img.alicdn.com/tps/TB1eREfLVXXXXaHXFXXXXXXXXXX-480-260.png" />
</button>
<input type="button" value="点我！">
```

### 属性
- type

```html
<button type="button"> 普通按钮，默认值
<button type="reset"> 表示form表单里的重置按钮
<button type="submit"> 表示form表单里的提交按钮
```