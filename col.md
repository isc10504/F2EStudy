# &lt;col&gt;

### 说明
&lt;col&gt; 标签规定了 &lt;colgroup&gt; 元素内部的每一列的列属性。
通过使用 &lt;col&gt; 标签，可以向整个列应用样式，而不需要重复为每个单元格或每一行设置样式。

```html
<table border="1">
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>ISBN</th>
    <th>Title</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>3476896</td>
    <td>My first HTML</td>
    <td>$53</td>
  </tr>
</table>
```
<a href="http://www.runoob.com/try/try.php?filename=tryhtml_col_test" target="_blank">尝试一下</a>

### 属性
- span

```html
<col span="2"> 规定 <col> 元素应该横跨的列数
```
