# &lt;audio&gt;

### 说明
&lt;audio&gt;标签定义音频，比如音乐或其他音频流。  
目前支持的3种文件格式：MP3、Wav、Ogg。
```html
<audio controls autoplay loop muted preload="none">
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  您的浏览器不支持 audio 元素。
</audio>
```
<a href="http://www.runoob.com/try/try.php?filename=tryhtml5_audio_preload" target="_blank">尝试一下</a>


### 属性
- autoplay

```html
<audio autoplay="autoplay"> 音频会自动播放
<audio autoplay> 由于autoplay属性只有一个同名的属性值，所以可以省略掉属性值
```

- controls

```html
<audio controls> 向用户显示音频控件（比如播放/暂停按钮）
```

- loop

```html
<audio loop> 音频会循环播放
```

- muted

```html
<audio muted> 静音
```

- preload

```html
<audio preload="auto"> 当页面加载后载入整个音频
<audio preload="meta"> 当页面加载后只载入元数据，比如音频的时长
<audio preload="none"> 当页面加载后不载入音频
```
