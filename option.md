# &lt;option&gt;

### 说明

option 标签定义下拉列表中的一个选项（一个条目）。  
option 标签中的内容作为 select  的一个元素使用。  
option 标签可以在不带有任何属性的情况下使用，但是您通常需要使用 value 属性，此属性会指示出被送往服务器的内容

```html
<select>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>
```
<select>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="opel">Opel</option>
  <option value="audi">Audi</option>
</select>



### 属性
- disabled

禁用该条选项

```html
<select>
    <option value="volvo" disabled>Volvo</option>
    <option value="saab">Saab</option>
    <option value="vw">VW</option>
    <option value="audi">Audi</option>
</select>
```
<select>
    <option value="volvo" disabled>Volvo</option>
    <option value="saab">Saab</option>
    <option value="vw">VW</option>
    <option value="audi">Audi</option>
</select>

<hr>

- label

label 属性规定更短版本的选项。
下拉列表中会显示出所规定的更短版本。
```html
<select>
    <option label="Volvo">Volvo (Latin for "I roll")</option>
    <option label="Saab">Saab (Swedish Aeroplane AB)</option>
    <option label="Mercedes">Mercedes (Mercedes-Benz)</option>
    <option label="Audi">Audi (Auto Union Deutschland Ingolstadt)</option>
</select>
```
<select>
    <option label="Volvo">Volvo (Latin for "I roll")</option>
    <option label="Saab">Saab (Swedish Aeroplane AB)</option>
    <option label="Mercedes">Mercedes (Mercedes-Benz)</option>
    <option label="Audi">Audi (Auto Union Deutschland Ingolstadt)</option>
</select>

<hr>

- selected

selected 属性规定在页面加载时预先选定该选项。
被预选的选项会显示在下拉列表最前面的位置。
```html
<select>
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="vw">VW</option>
    <option value="audi" selected>Audi</option>
</select>
```
<select>
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
    <option value="vw">VW</option>
    <option value="audi" selected>Audi</option>
</select>

<hr>

- value

value 属性规定在表单被提交时被发送到服务器的值。
开始标签 &lt;option&gt; 与结束标签 &lt;/option&gt; 之间的内容是浏览器显示在下拉列表中的内容，而 value 属性中的值是表单提交时被发送到服务器的值。  
如果没有规定 value 属性，选项的值将设置为 &lt;option&gt; 与结束标签 &lt;/option&gt; 之间的内容
```html
<form action="demo_form.html">
    <select name="cars">
        <option value="volvo">Volvo XC90</option>
        <option value="saab">Saab 95</option>
        <option value="mercedes">Mercedes SLK</option>
        <option value="audi">Audi TT</option>
    </select>
    <input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
    <select name="cars">
        <option value="volvo">Volvo XC90</option>
        <option value="saab">Saab 95</option>
        <option value="mercedes">Mercedes SLK</option>
        <option value="audi">Audi TT</option>
    </select>
    <input type="submit" value="Submit">
</form>

