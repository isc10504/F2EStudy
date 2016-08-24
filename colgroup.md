# &lt;colgroup&gt;

### 说明
&lt;colgroup&gt; 标签用于对表格中的列进行组合，以便对其进行格式化。
通过使用 &lt;colgroup&gt; 标签，可以向整个列应用样式，而不需要重复为每个单元格或每一行设置样式。
注释：只能在 &lt;table&gt; 元素之内，在任何一个 &lt;caption&gt; 元素之后，在任何一个 &lt;thead&gt;、&lt;tbody&gt;、&lt;tfoot&gt;、&lt;tr&gt; 元素之前使用 &lt;colgroup&gt; 标签，需要配合&lt;col&gt; 标签一起使用。

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

