# &lt;area&gt;

### 说明
&lt;area&gt;标签在一个图片内部创建一个可点击的区域  
&lt;area&gt;标签始终嵌套在 &lt;map&gt; 标签内部。  
&lt;img&gt; 中的 usemap 属性可引用 &lt;map&gt; 中的 id 或 name 属性（由浏览器决定），所以我们需要同时向 &lt;map&gt; 添加 id 和 name 两个属性
```html
<img src="planets.gif" width="145" height="126" alt="Planets"
usemap="#planetmap">

<map name="planetmap" id="planetmap">
    <area shape="rect" coords="0,0,82,126" href="sun.htm" title="Sun">
    <area shape="circle" coords="90,58,3" href="mercur.htm" title="Mercury">
    <area shape="poly" coords="285,187,282,177,278,168,269,163,262,158" href="venus.htm" title="Venus">
</map>
```
### 属性
- shape 和 coords

```html
<area shape="rect" coords="0,0,82,126"> 创建一个矩形区域，coords属性设置值为矩形的左上角,右下角的坐标,各个坐标值之间用逗号分开
<area shape="circle" coords="90,58,3"> 创建一个圆形区域，coords属性设置值为圆心坐标及半径,前两个参数分别为圆心的横,纵坐标,第三个参数为半径
<area shape="poly" coords="285,187,282,177,278,168,269,163,262,158"> 创建一个多边形区域，coords属性设置值为多边形各项顶点的坐标值
```

- href

与&lt;a&gt;标签的href属性一样

- target

与&lt;a&gt;标签的target属性一样

- rel

与&lt;a&gt;标签的rel属性一样

- title  

与&lt;a&gt;标签的title属性一样