# &lt;input&gt;

### 说明
&lt;input&gt; 标签规定了用户可以在其中输入数据的输入字段。
&lt;input&gt; 元素在 &lt;form&gt; 元素中使用，用来声明允许用户输入数据的 input 控件。
输入字段可通过多种方式改变，取决于 type 属性，针对不同的type属性值，还会有其他的属性来配合使用


```html
<form action="demo_form.asp">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```

### 属性
- accept

规定通过文件上传来提交的文件的类型。 (只针对type="file")

```html
<input type="file" name="pic" accept="image/*"> 允许上传图片
<input accept="audio/*|video/*|image/*|MIME_type"> 允许上传图片，音频，视频等
```
<input type="file" name="pic" accept="image/*">

- alt

alt 属性为用户由于某些原因（比如网速太慢、src 属性中的错误、浏览器禁用图像、用户使用的是屏幕阅读器）无法查看图像时提供了替代文本。
注意：alt 属性只能与 &lt;input type="image"&gt; 配合使用。
```html
<input type="image" src="submit.gif" alt="Submit" width="48" height="48">
```
<a href="http://www.runoob.com/try/try.php?filename=tryhtml_input_alt" target="_blank">尝试</a>


- autocomplete

自动补全功能，参考form的autocomplete

```html
<form action="demo_form.html" autocomplete="on"> 这里是全局的自动补全设置
    <input type="email" name="email" autocomplete="off"> 这里可以单独对某个input设置自动补全
</form>
```

- autofocus

当页面加载时 当前的input元素自动获得焦点，只能对一个input元素进行设置

```html
<form action="demo_form.html">
  First name: <input type="text" name="fname" autofocus><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit">
</form>
```
<form action="demo_form.html">
  First name: <input type="text" name="fname" autofocus><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit">
</form>

<hr>
- checked

checked 属性规定在页面加载时应该被预先选定的 input 元素。 (只针对 type="checkbox" 或者 type="radio")

```html
<form action="demo_form.html">
    <input type="checkbox" name="vehicle" value="Bike"> I have a bike<br>
    <input type="checkbox" name="vehicle" value="Car" checked> I have a car
    <br><input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
    <input type="checkbox" name="vehicle" value="Bike"> I have a bike<br>
    <input type="checkbox" name="vehicle" value="Car" checked> I have a car
    <br><input type="submit" value="Submit">
</form>

<hr>
- disabled

disabled 属性规定应该禁用的 input 元素。被禁用的 input 元素是**无法使用和无法点击**的。  
表单中被禁用的 input 元素**不会被提交**。  
disabled 属性不适用于 &lt;input type="hidden"&gt;。


```html
<form action="demo_form.html">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname" disabled><br>
  <input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname" disabled><br>
  <input type="submit" value="Submit">
</form>

<hr>
- form

form 属性规定 input 元素所属的一个或多个表单的 id 列表，以空格分隔

```html
<form action="demo_form.html" id="form1">
First name: <input type="text" name="fname"><br>
<input type="submit" value="Submit">
</form>

Last name: <input type="text" name="lname" form="form1">  位于 form 表单外的输入字段（但仍然属于 form 表单的一部分）：
```
<hr>
- formaction & formenctype & formmethod & formtarget

这四个属性都可以覆盖form表单的action & enctype & method & target 默认设置，。(只针对 type="submit" 和 type="image")

```html
<form action="demo_form.html" method="get">
    First name: <input type="text" name="fname"><br>
    Last name: <input type="text" name="lname"><br>
    <input type="submit" value="Submit">
    <input type="submit" formmethod="post" formaction="demo_post.html" value="Submit using POST">改变了form默认的action和method
</form>
```

<hr>
- list

list 属性引用 &lt;datalist&gt; 元素，其中包含 input 元素的预定义选项。

```html
<input list="browsers">

<datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Google Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```
<input list="browsers">

<datalist id="browsers">
  <option value="Internet Explorer">
  <option value="Firefox">
  <option value="Google Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>


<hr>
- max & min

max 属性规定 input 元素的最大值。
提示：max 属性与 min 属性配合使用，可创建合法值范围。
注意：max 和 min 属性适用于以下 input 类型：number、range、date、datetime、datetime-local、month、time 和 week。

```html
<form action="demo_form.html">

  Enter a date before 1980-01-01:
  <input type="date" name="bday" max="1979-12-31"><br>

  Enter a date after 2000-01-01:
  <input type="date" name="bday" min="2000-01-02"><br>

  Quantity (between 1 and 5):
  <input type="number" name="quantity" min="1" max="5"><br>

  <input type="submit">

</form>
```
<form action="demo_form.html">

  Enter a date before 1980-01-01:
  <input type="date" name="bday" max="1979-12-31"><br>

  Enter a date after 2000-01-01:
  <input type="date" name="bday" min="2000-01-02"><br>

  Quantity (between 1 and 5):
  <input type="number" name="quantity" min="1" max="5"><br>

  <input type="submit">

</form>

<hr>
- maxlength

maxlength 属性规定 input 元素中允许的最大字符数。

```html
<form action="demo_form.html">
  Username: <input type="text" name="usrname" maxlength="10"><br>
  <input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
  Username: <input type="text" name="usrname" maxlength="10"><br>
  <input type="submit" value="Submit">
</form>

<hr>
- multiple

multiple 属性规定允许用户输入到 input 元素的多个值

```html
<form action="demo_form.html">
  Select images: <input type="file" name="img" multiple><br>
  <select multiple>
      <option value="1">看电影</option>
      <option value="2">吃饭</option>
      <option value="3">唱歌</option>
  </select>
  <input type="submit">
</form>
```
<form action="demo_form.html">
  Select images: <input type="file" name="img" multiple><br>
  <select multiple>
      <option value="1">看电影</option>
      <option value="2">吃饭</option>
      <option value="3">唱歌</option>
  </select>
  <input type="submit">
</form>

<hr>
- name

name 属性用于在表单提交后，给后台引用表单数据

```html
<form action="demo_form.html">
  Name: <input type="text" name="fullname"><br>
  Email: <input type="text" name="email"><br>
  <input type="submit" value="Submit">
</form>
```

<hr>
- pattern

pattern 属性规定用于验证 input 元素的值的正则表达式。
pattern 属性适用于下面的 input 类型：text、search、url、tel、email 和 password。
请使用全局的 title 属性来描述模式以帮助用户。

```html
<form action="demo_form.html">
    Country code: <input type="text" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
    <input type="submit">
</form>
```
<form action="demo_form.html">
    Country code: <input type="text" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
    <input type="submit">
</form>

<hr>
- placeholder

placeholder 属性规定可描述输入字段预期值的简短的提示信息（比如：一个样本值或者预期格式的短描述）。
该提示会在用户输入值之前显示在输入字段中。  
placeholder 属性适用于下面的 input 类型：text、search、url、tel、email 和 password。

```html
<form action="demo-form.php">
  <input type="text" name="fname" placeholder="First name"><br>
  <input type="text" name="lname" placeholder="Last name"><br>
  <input type="submit" value="Submit">
</form> 
```
<form action="demo-form.php">
  <input type="text" name="fname" placeholder="First name"><br>
  <input type="text" name="lname" placeholder="Last name"><br>
  <input type="submit" value="Submit">
</form> 

<hr>
- readonly

readonly 属性规定输入字段是只读的。
只读字段是不能修改的。不过，用户仍然可以使用 tab 键切换到该字段，还可以选中或拷贝其文本。
readonly 属性可以防止用户对值进行修改，直到满足某些条件为止（比如选中了一个复选框）。然后，需要使用 JavaScript 消除 readonly 值，将输入字段切换到可编辑状态。

```html
<form action="demo_form.html">
  Country: <input type="text" name="country" value="Norway" readonly><br>
  <input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
  Country: <input type="text" name="country" value="Norway" readonly><br>
  <input type="submit" value="Submit">
</form>

<hr>
- required

required 属性规定必需在提交表单之前填写输入字段。
注意：required 属性适用于下面的 input 类型：text、search、url、tel、email、password、date pickers、number、checkbox、radio 和 file。

```html
<form action="demo_form.html">
    Username: <input type="text" name="usrname" required>
    <input type="submit">
</form>
```
<form action="demo_form.html">
    Username: <input type="text" name="usrname" required>
    <input type="submit">
</form>

<hr>
- size

size 属性规定以字符数计的 input 元素的可见宽度，最好是使用css的width来定义可见宽度  
size 属性适用于下面的 input 类型：text、search、tel、url、email 和 password。
如需规定 input 元素中允许的最大字符数，使用 maxlength 属性。

```html
<form action="demo_form.html">
  Email: <input type="text" name="email" size="35"><br>
  PIN: <input type="text" name="pin" maxlength="4" size="4"><br>
  <input type="submit" value="Submit">
</form>
```
<form action="demo_form.html">
  Email: <input type="text" name="email" size="35"><br>
  PIN: <input type="text" name="pin" maxlength="4" size="4"><br>
  <input type="submit" value="Submit">
</form>

<hr>
- src

src 属性规定显示为提交按钮的图像的 URL。
src 属性对于 &lt;input type="image"&gt; 是必需的属性，且只能与 &lt;input type="image"&gt; 配合使用。

```html
<form action="demo_form.html">
  First name: <input type="text" name="fname"><br>
  <input type="image" src="submit.gif" alt="Submit">
</form>
```
<hr>
- step

step 属性规定 input 元素的合法数字间隔。
实例：如果 step="3"，则合法数字应该是 -3、0、3、6，以此类推。
step 属性可以与 max 和 min 属性配合使用，以创建合法值的范围。
step 属性适用于下面的 input 类型：number、range、date、datetime、datetime-local、month、time 和 week。

```html
<form action="demo_form.html">
    <input type="number" name="points" step="3">
    <input type="submit">
</form>
```
<form action="demo_form.html">
    <input type="number" name="points" step="3">
    <input type="submit">
</form>

<hr>
- type

type 属性规定要显示的 input 元素的类型。
默认类型是：text。
该属性不是必需的，但是我们认为您应该始终使用它。

```html
<input type="button">  定义可点击的按钮（通常与 JavaScript 一起使用来启动脚本）<br>
<input type="checkbox"> 定义复选框<br>
<input type="text"> 默认。定义一个单行的文本字段（默认宽度为 20 个字符）<br>
<input type="password"> 定义密码字段（字段中的字符会被遮蔽）。<br>
<input type="file"> 定义文件选择字段和 "浏览..." 按钮，供文件上传。<br>
<input type="hidden"> 定义隐藏输入字段，一般用来传递不需要用户自己输入的数据给后台<br>
<input type="image"> 定义图像作为提交按钮<br>
<input type="radio"> 定义单选按钮<br>
<input type="submit"> 定义提交按钮。<br>
<input type="reset"> 定义重置按钮（重置所有的表单值为默认值）<br>
以下为html5中新加入的，大部分功能比较复杂，各个浏览器对于原生的样式实现有比较大的差异，为了保持样式的统一，一般都是自己实现，不用原生的<br>
<input type="color"> 定义取色器<br>
<input type="date"> 定义 date 控件（包括年、月、日，不包括时间）。<br>
<input type="datetime"> 定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，基于 UTC 时区）。<br>
<input type="datetime-local"> 定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，不带时区）。<br>
<input type="email"> 定义用于 e-mail 地址的字段。<br>
<input type="month"> 定义 month 和 year 控件（不带时区）。<br>
<input type="number"> 定义用于输入数字的字段<br>
<input type="range"> 定义用于精确值不重要的输入数字的控件（比如 slider 控件）。<br>
<input type="search"> 定义用于输入搜索字符串的文本字段。<br>
<input type="tel">  定义用于输入电话号码的字段<br>
<input type="time">  定义用于输入时间的控件（不带时区）。<br>
<input type="url"> 定义用于输入 URL 的字段。<br>
<input type="week"> 定义 week 和 year 控件（不带时区）。<br>
```
<input type="button">  定义可点击的按钮（通常与 JavaScript 一起使用来启动脚本）<br>
<input type="checkbox"> 定义复选框<br>
<input type="text"> 默认。定义一个单行的文本字段（默认宽度为 20 个字符）<br>
<input type="password"> 定义密码字段（字段中的字符会被遮蔽）。<br>
<input type="file"> 定义文件选择字段和 "浏览..." 按钮，供文件上传。<br>
<input type="hidden"> 定义隐藏输入字段，一般用来传递不需要用户自己输入的数据给后台<br>
<input type="image"> 定义图像作为提交按钮<br>
<input type="radio"> 定义单选按钮<br>
<input type="submit"> 定义提交按钮。<br>
<input type="reset"> 定义重置按钮（重置所有的表单值为默认值）<br>
以下为html5中新加入的，大部分功能比较复杂，各个浏览器对于原生的样式实现有比较大的差异，为了保持样式的统一，一般都是自己实现，不用原生的<br>
<input type="color"> 定义取色器<br>
<input type="date"> 定义 date 控件（包括年、月、日，不包括时间）。<br>
<input type="datetime"> 定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，基于 UTC 时区）。<br>
<input type="datetime-local"> 定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，不带时区）。<br>
<input type="email"> 定义用于 e-mail 地址的字段。<br>
<input type="month"> 定义 month 和 year 控件（不带时区）。<br>
<input type="number"> 定义用于输入数字的字段<br>
<input type="range"> 定义用于精确值不重要的输入数字的控件（比如 slider 控件）。<br>
<input type="search"> 定义用于输入搜索字符串的文本字段。<br>
<input type="tel">  定义用于输入电话号码的字段<br>
<input type="time">  定义用于输入时间的控件（不带时区）。<br>
<input type="url"> 定义用于输入 URL 的字段。<br>
<input type="week"> 定义 week 和 year 控件（不带时区）。<br>


<hr>
- value

value 属性规定 input 元素的值。
value 属性对于不同 input 类型，用法也不同：
- 对于 "button"、"reset"、"submit" 类型 - 定义按钮上的文本
- 对于 "text"、"password"、"hidden" 类型 - 定义输入字段的初始（默认）值
- 对于 "checkbox"、"radio"、"image" 类型 - 定义与 input 元素相关的值，当提交表单时该值会发送到表单的 action URL。
value 属性对于 &lt;input type="checkbox"&gt; 和 &lt;input type="radio"&gt; 是必需的。
value 属性不适用于 &lt;input type="file"&gt;。
```html
<form action="demo_form.html">
  First name: <input type="text" name="fname" value="John"><br>
  Last name: <input type="text" name="lname" value="Doe"><br>
  <input type="submit" value="Submit form">
</form>
```
<form action="demo_form.html">
  First name: <input type="text" name="fname" value="John"><br>
  Last name: <input type="text" name="lname" value="Doe"><br>
  <input type="submit" value="Submit form">
</form>