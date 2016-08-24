# &lt;script&gt;

### 说明
script 标签用于定义客户端脚本，比如 JavaScript。  
script 元素既可包含脚本语句，也可以通过 "src" 属性指向外部脚本文件。  



如果使用 "src" 属性，则 script 元素内部的脚本不会被执行，应该保持内部是空的  

有多种执行外部脚本的方法：
- 如果 async="async"：脚本相对于页面的其余部分异步地执行（当页面继续进行解析时，脚本将被执行）
- 如果不使用 async 且 defer="defer"：脚本将在页面完成解析时执行
- 如果既不使用 async 也不使用 defer：在浏览器继续解析页面之前，立即读取并执行脚本

### 属性
- charset

charset 属性规定引入的js代码的字符编码方式
```html
<script src="myscripts.js" charset="utf-8"></script>
```






