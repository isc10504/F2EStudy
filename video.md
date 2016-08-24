# &lt;video&gt;

### 说明
video 标签定义视频，比如电影片段或其他视频流。  
目前，video 元素支持三种视频格式：MP4、WebM、Ogg。  
可以在 &lt;video&gt; 和 &lt;/video&gt; 标签之间放置文本内容，这样不支持 &lt;video&gt; 元素的浏览器就可以显示出该文本内容

```html
<video width="320" height="240" controls>
    <source src="http://www.runoob.com/try/demo_source/movie.mp4" type="video/mp4">
    <source src="http://www.runoob.com/try/demo_source/movie.ogg" type="video/ogg">
    您的浏览器不支持 video 标签。
</video>
```
<video width="320" height="240" controls>
    <source src="http://www.runoob.com/try/demo_source/movie.mp4" type="video/mp4">
    <source src="http://www.runoob.com/try/demo_source/movie.ogg" type="video/ogg">
    您的浏览器不支持 video 标签。
</video>

**属性部分参见 audio**








