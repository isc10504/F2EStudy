# &lt;textarea&gt;

### 说明
textarea 标签定义一个多行的文本输入控件。  
文本区域中可容纳无限数量的文本。  
可以通过 cols 和 rows 属性来规定 textarea 的尺寸大小，不过更好的办法是使用 CSS 的 height 和 width 属性。

```html
<textarea rows="10" cols="30">
我是一个文本框。 
</textarea>
```
<textarea rows="10" cols="30">
我是一个文本框。 
</textarea>

### 属性
- autofocus

页面加载完，自动获得焦点


- disabled

禁用文本区域

- maxlength

maxlength 属性规定文本区域的最大长度（以字符计）。

- name

提交表单时，数据传递给后端的名称

- placeholdere

规定一个简短的提示，描述文本区域期望的输入值

```html
<textarea placeholder="描述信息...">
</textarea>
```

<textarea placeholder="描述信息...">
</textarea>

- readonly

规定文本区域为只读

- required

规定文本区域是必需的/必填的






