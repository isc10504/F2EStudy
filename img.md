# &lt;img&gt;

### 说明
&lt;img&gt; 标签定义 HTML 页面中的图像。
&lt;img&gt; 标签有两个必需的属性：src 和 alt。
注释：从技术上讲，图像并不会插入 HTML 页面中，而是链接到 HTML 页面上。&lt;img&gt; 标签的作用是为被引用的图像创建占位符，img是可替换元素


```html
<img src="smiley.gif" alt="Smiley face" height="42" width="42">
```

### 属性
- alt

alt是对图片内容的描述，当图片不能显示的时候，会显示alt，盲人阅读器也会读取alt属性的值

- src

图片的URL地址

- usemap

usemap 属性将图片定义为客户端图片映射（图片映射指的是带有可点击区域的图片）

```html
<img src="planets.gif" width="145" height="126" alt="Planets" usemap="#planetmap">

<map name="planetmap">
  <area shape="rect" coords="0,0,82,126" href="sun.htm" title="Sun">
  <area shape="circle" coords="90,58,3" href="mercur.htm" title="Mercury">
  <area shape="circle" coords="124,58,8" href="venus.htm" title="Venus">
</map>
```

- ismap

ismap 属性是一个布尔属性。
ismap 属性将图像定义为服务器端图像映射（图像映射指的是带有可点击区域的图像）。
当点击一个服务器端图像映射时，点击坐标会以 URL 查询字符串的形式发送到服务器。
注意：只有当 &lt;img&gt; 元素属于带有有效 href 属性的 &lt;a&gt; 元素的后代时，才允许使用 ismap 属性。

```html
<a href="demo_form.html">
    <img src="w3html.gif" alt="W3CSchool.cc" ismap>
</a>
```
<a href="http://www.runoob.com/try/try.php?filename=tryhtml_img_ismap" target="_blank">尝试</a>
