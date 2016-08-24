# &lt;canvas&gt;

### 说明
&lt;canvas&gt; 标签通过脚本（通常是 JavaScript）来绘制图形（比如图表和其他图像）。
&lt;canvas&gt; 标签只是图形容器，您必须使用脚本来绘制图形。

```html
<canvas id="myCanvas"></canvas>

<script type="text/javascript">
    var canvas=document.getElementById('myCanvas');
    var ctx=canvas.getContext('2d');
    ctx.fillStyle='#FF0000';
    ctx.fillRect(0,0,80,100);
</script>
```
<a href="http://www.runoob.com/try/try.php?filename=tryhtml5_canvas" target="_blank">尝试一下</a>
