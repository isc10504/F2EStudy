# &lt;tbody&gt;

### 说明
tbody 标签用于组合 HTML 表格的主体内容。  
tbody 元素应该与 thead 及 tfoot 元素结合起来使用，用来规定表格的各个部分（主体、表头、页脚）。  
通过使用这些元素，使浏览器有能力支持独立于表格表头和表格页脚的表格主体滚动。当包含多个页面的长的表格被打印时，表格的表头和页脚可被打印在包含表格数据的每张页面上。  
tbody 标签必须被用在以下情境中：作为 table 元素的子元素，出现在 caption、colgroup 和 thead 元素之后。
tbody 元素内部必须包含一个或者多个 tr 标签。  
thead、tbody 和 tfoot 元素默认不会影响表格的布局。

```html
<style>
    table{
        border-collapse: collapse;
        border-spacing: 0;
        border: 1px solid #333;
    }
</style>

<table>
    <thead>
        <tr>
            <th>Month</th>
            <th>Savings</th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <td>Sum</td>
            <td>$180</td>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <td>January</td>
            <td>$100</td>
        </tr>
        <tr>
            <td>February</td>
            <td>$80</td>
        </tr>
    </tbody>
</table>
```
<style>
    table{
        border-collapse: collapse;
        border-spacing: 0;
        border: 1px solid #333;
    }
</style>

<table>
    <thead>
        <tr>
            <th>Month</th>
            <th>Savings</th>
        </tr>
    </thead>
    <tfoot>
        <tr>
            <td>Sum</td>
            <td>$180</td>
        </tr>
    </tfoot>
    <tbody>
        <tr>
            <td>January</td>
            <td>$100</td>
        </tr>
        <tr>
            <td>February</td>
            <td>$80</td>
        </tr>
    </tbody>
</table>







