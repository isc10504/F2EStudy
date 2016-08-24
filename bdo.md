# &lt;bdo&gt;

### 说明
bdo 指的是 bidi 覆盖（Bi-Directional Override）。
&lt;bdo&gt; 标签用来覆盖默认的文本方向。可以用来设置文字从右到左显示

```html
<p><bdo dir="rtl">我要买一个<bdi>mp3</bdi> 送给你。</bdo></p> 
```

bdo设置了dir属性为rtl(right to left)，里面的文字会从右到左显示，但是里面被bdi包起来的mp3还是保持从左到右显示

<a href="http://www.runoob.com/try/try.php?filename=tryhtml_bdo" target="_blank">尝试一下</a>

### 属性
- dir

```html
<bdo dir="ltr"> 文字从左到右显示，默认值
<bdo dir="rtl"> 文字从右到左显示
```