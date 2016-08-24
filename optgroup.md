# &lt;optgroup&gt;

### 说明
 
optgroup 标签经常用于把相关的选项组合在一起。
如果你有很多的选项组合, 你可以使用optgroup 标签能够很简单的将相关选项组合在一起

```html
<select>
  <optgroup label="Swedish Cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>
```
<select>
  <optgroup label="Swedish Cars">
    <option value="volvo">Volvo</option>
    <option value="saab">Saab</option>
  </optgroup>
  <optgroup label="German Cars">
    <option value="mercedes">Mercedes</option>
    <option value="audi">Audi</option>
  </optgroup>
</select>



### 属性
- disabled

禁用该选项组

```html
<select>
    <optgroup label="German Cars" disabled>
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </optgroup>
    <optgroup label="German Cars">
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </optgroup>
</select>
```
<select>
    <optgroup label="German Cars" disabled>
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </optgroup>
    <optgroup label="German Cars">
        <option value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </optgroup>
</select>

<hr>

- label

label 属性为选项组规定描述标签



