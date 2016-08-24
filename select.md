# &lt;select&gt;

### 说明
select 元素用来创建下拉列表。
select 元素中的 option 标签定义了列表中的可用选项。

```html
<select>
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
</select>
```


### 属性
- autofocus

页面加载完，自动获得焦点


- disabled

禁用下拉列表

- multiple

可选择多个选项

- name

提交表单时，数据传递给后端的名称

- required

规定用户在提交表单前必须选择一个下拉列表中的选项

- size

size 属性规定下拉列表中可见选项的数目。  
如果 size 属性的值大于 1，但是小于列表中选项的总数目，浏览器会显示出滚动条，表示可以查看更多选项。
```html
<select size="3">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
</select>
```
<select size="3">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
</select>
