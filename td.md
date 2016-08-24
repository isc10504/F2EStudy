# &lt;td&gt;

### 说明
td 标签定义 HTML 表格中的标准单元格。  
HTML 表格有两种单元格类型：  
表头单元格 - 包含头部信息（由 th 元素创建）    
标准单元格 - 包含数据（由 td 元素创建）    
th 元素中的文本通常呈现为粗体并且居中。  
td 元素中的文本通常是普通的左对齐文本。    
如果需要将内容横跨多个行或列，使用 colspan 和 rowspan 属性

```html
<table>
    <tr>
        <td>Cell A</td>
        <td>Cell B</td>
    </tr>
</table>
```

### 属性
- colspan

colspan 属性定义单元格应该横跨的列数。
```html
<style>
    table{
        border-collapse: collapse;
        border-spacing: 0;
        border: 1px solid #333;
    }
</style>

<table>
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$100</td>
    </tr>
    <tr>
        <td colspan="2">Sum: $180</td>
    </tr>
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
    <tr>
        <th>Month</th>
        <th>Savings</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$100</td>
    </tr>
    <tr>
        <td colspan="2">Sum: $180</td>
    </tr>
</table>

<hr>

- rowspan

rowspan 属性定义单元格应该横跨的行数。
```html
<style>
    table{
        border-collapse: collapse;
        border-spacing: 0;
        border: 1px solid #333;
    }
</style>

<table>
    <tr>
        <th>Month</th>
        <th>Savings</th>
        <th>Savings for holiday!</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
        <td rowspan="2">$50</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$80</td>
    </tr>
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
    <tr>
        <th>Month</th>
        <th>Savings</th>
        <th>Savings for holiday!</th>
    </tr>
    <tr>
        <td>January</td>
        <td>$100</td>
        <td rowspan="2">$50</td>
    </tr>
    <tr>
        <td>February</td>
        <td>$80</td>
    </tr>
</table>





