# &lt;map&gt;

### 说明  
map 标签用于客户端图像映射。图像映射指带有可点击区域的一幅图像。
area 元素永远嵌套在 map 元素内部。area 元素可定义图像映射中的区域。
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
