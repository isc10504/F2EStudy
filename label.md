# &lt;label&gt;

### 说明
&lt;label&gt; 标签为 input 元素定义标注（标记）。
label 元素不会向用户呈现任何特殊效果。不过，它为鼠标用户改进了可用性。如果您在 label 元素内点击文本，就会触发此控件。就是说，当用户选择该标签时，浏览器就会自动将焦点转到和标签相关的表单控件上。
&lt;label&gt; 标签的 for 属性应当与相关元素的 id 属性相同。

```html
<form action="demo_form.asp">
  <label for="male">Male</label>
  <input type="radio" name="sex" id="male" value="male"><br>
  <label for="female">Female</label>
  <input type="radio" name="sex" id="female" value="female"><br>
  <input type="submit" value="Submit">
</form>
```
<form action="demo_form.asp">
  <label for="male">Male</label>
  <input type="radio" name="sex" id="male" value="male"><br>
  <label for="female">Female</label>
  <input type="radio" name="sex" id="female" value="female"><br>
  <input type="submit" value="Submit">
</form>

### 属性
- for

for 属性规定 label 绑定的表单元素。


- form

规定 label 元素所属的一个或多个表单的 id 列表，以空格分隔。
```html
<form action="demo_form.html" id="form1">
  <input type="radio" name="sex" id="male" value="male"><br>
  <label for="female">Female</label>
  <input type="radio" name="sex" id="female" value="female">
  <input type="submit" value="Submit">
</form>

<label for="male" form="form1">Male</label> 位于 form 表单外的 <label> 元素（但仍然属于 form 表单的一部分）
```

<form action="demo_form.html" id="form1">
  <input type="radio" name="sex" id="male" value="male"><br>
  <label for="female">Female</label>
  <input type="radio" name="sex" id="female" value="female">
  <input type="submit" value="Submit">
</form>

<label for="male" form="form1">Male</label>

