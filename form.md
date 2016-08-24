# &lt;form&gt;

### 说明
&lt;form&gt; 标签用于创建供用户输入的 HTML 表单。表单非常重要，它的几个特有属性也非常重要。

```html
<form accept-charset="utf-8" action="demo-form.php" method="get" autocomplete="on" enctype="multipart/form-data" target="_blank">
  First name:<input type="text" name="fname"><br>
  E-mail: <input type="email" name="email"><br>
  <input type="submit">
</form>
```
### 属性
- accept-charset

利用accept-charset实现在不同编码的页面里提交表单，例如当前的页面编码是utf-8，表单要提交的页面编码是gb2312，这种情况下就可以设置accept-charset="gb2312"
```html
<form accept-charset="gb2312"> 
```
- action

action 属性规定当提交表单时，向何处发送表单数据。如果action没有设置，默认是提交到当前页面本身

```html
<form action="demo_form.html" method="get">
  First name: <input type="text" name="fname"><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit" value="Submit">
</form>
```
- autocomplete

autocomplete 属性规定表单是否应该启用自动补全功能。
自动补全允许浏览器预测对字段的输入。当用户在字段开始键入时，浏览器基于之前键入过的值，应该显示出在字段中填写的选项。比如之前在一个字段输入过"abc@a.com" 这个邮箱地址，下次在这个字段里输入一个"a"，就会自动提示可以补全"abc@a.com"

```html
<form autocomplete="on">启用自动补全
<form autocomplete="off">关闭自动补全
```

- enctype

enctype 属性规定在将表单数据发送到服务器之前如何对其进行编码。只有 method="post" 时才使用 enctype 属性

```html
<form enctype="application/x-www-form-urlencoded">默认。在发送前对所有字符进行编码（将空格转换为 "+" 符号，特殊字符转换为 ASCII HEX 值）。
<form enctype="multipart/form-data">不对字符编码。当使用有文件上传控件的表单时，该值是必需的。
<form enctype="text/plain">将空格转换为 "+" 符号，但不编码特殊字符。
```

- method

method 方法规定如何发送表单数据（form-data）（表单数据会被发送到在 action 属性中规定的页面中）。
表单数据可被作为 URL 变量的形式来发送（method="get"）或者作为 HTTP post 事务的形式来发送（method="post"）  

### 关于 GET 的注释：
- 将表单数据以名称/值对的形式附加到 URL 中
- URL 的长度是有限的（大约 3000 字符）
- 绝不要使用 GET 来发送敏感数据！（在 URL 中是可见的）
- 对于用户希望加入书签的表单提交很有用
- GET 更适用于非安全数据，比如在 Google 中查询字符串

### 关于 POST 的注释：
- 将表单数据附加到 HTTP 请求的 body 内（数据不显示在 URL 中）
- 没有长度限制
- 通过 POST 提交的表单不能加入书签

```html
<form method="get"> 默认。将表单数据（form-data）以名称/值对的形式附加到 URL 中：URL?name=value&name=value。
<form method="post"> 以 HTTP post 事务的形式发送表单数据（form-data）。
```

- target

与&lt;a&gt;标签的target属性一样