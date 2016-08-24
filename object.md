# &lt;object&gt;

### 说明
 
object 标签用于嵌入对象，比如图像、音频、视频、Java applets、ActiveX、PDF 以及 Flash。    
如果浏览器不能正常解析 object 元素，就会执行位于 &lt;object&gt; 和 &lt;/object&gt; 之间的代码。通过这种方式，我们能够降级处理 。  
和embed标签类似，但embed比较旧，推荐使用object
```html
<object width="400" height="400" data="http://www.runoob.com/try/demo_source/helloworld.swf"></object>
<object data="data/test.pdf" type="application/pdf" width="300" height="200">
  alt : <a href="data/test.pdf">test.pdf</a>  当浏览器不能解析object的时候，会显示一个超链接，让用户自己下载pdf
</object>
<object data="abc.pdf" type="application/pdf">
    <embed src="abc.pdf" type="application/pdf" /> 当浏览器不能解析object的时候，会尝试embed的方式
</object>
```
<object width="400" height="400" data="http://www.runoob.com/try/demo_source/helloworld.swf"></object>
