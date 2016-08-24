# noscript
# &lt;noscript&gt;

### 说明  
noscript 元素用来定义在脚本未被执行时的替代内容（文本）。
此标签可被用于可识别 noscript 标签但无法支持其中的脚本的浏览器。
如果浏览器支持脚本，那么它不会显示出 noscript 元素中的文本。
```html
<script>
document.write("Hello World!")
</script>
<noscript>Your browser does not support JavaScript!</noscript>
```
