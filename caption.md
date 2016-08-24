# &lt;caption&gt;

### 说明
&lt;caption&gt; 标签定义表格的标题。
&lt;caption&gt; 标签必须直接放置到 &lt;table&gt; 标签之后。
您只能对每个表格定义一个标题。
通常这个标题会被居中于表格之上。可以通过caption的css 属性 "text-align" 和 "caption-side" 来设置标题的对齐方式和显示位置。
。

```html
<style type="text/css">
    caption
    {
        text-align:right;  /* 默认值是 center */
        caption-side:bottom; /* 默认值是 top */
    }
</style>
<table border="1">
  <caption>每月存款</caption>
  <tr>
    <th>月份</th>
    <th>存款</th>
  </tr>
  <tr>
    <td>一月</td>
    <td>10000</td>
  </tr>
</table>
```
