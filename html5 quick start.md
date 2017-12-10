# 结构元素
***
## header元素 #
header元素是一种具有引导和导航作用的结构元素，用语定义文档的页眉（介绍信息）。<br/>
Header元素通用来放置整个页面或页面内的一个内容区块的标题，可以包括网站logo图片、数据表格和搜索表单等内容。
``` html
<head>
     <h1>网页主题</h1>
</head>
```
***
## article 元素
article元素代表文档、页面或者应用程序中独立的、完整的、可以肚子被外部引用的内容。<br/>
article元素通常可以包含自己的标题，标题一般放在header元素中；还可以有注脚，注脚一般放在footer元素中。
***
## section 元素
section元素用于对网站或应用程序中页面上的内容进行分块。通常由内容和标题组成。当一个容器需要被直接定义样式或通过脚本定义行为时，推荐使用div 元素，而不是section 元素。<br/>
- **注意：<br/>**
     - section 元素不用做设置样式的页面容器，div 可以。<br/>
     - 没有标题的内容区块不适用section 元素。
***
## nav 元素
nav 元素是一个可以用作页面导航的链接组。只需要将主要的、基本的链接组放进nav 元素即可。<br/>
- **nav 元素可以用于以下几种场合：**
     - 传统导航条；
     - 侧边栏导航；
     - 页内导航；
     - 翻页操作。
```html
<nav>
 <a href=“#”>首页</a> |  <a href=“#”>新闻动态</a> |  <a href=“#”>规范标准</a> |  <a href=“#”>文章教程</a> | <a href=“#”>资源链接</a> |  <a href=“#”>常见问题</a> |  <a href=“#”>论坛交流</a> | 
</nav>
```
***
## aside 元素
aside 元素用来表示当前页或文章的附属信息部分，可以包含与当前页面或主要内容相关的引用、侧边栏、广告、导航条。可用于文章的注释、友情链接等。
***
## footer 元素
footer 元素可以作为其上层父级内容区块或是一个根区块的脚注，通常包含相关区块的脚注信息。
```html
<footer>
<div id=”r”>
          &copy; copyright 2014, my love website<br />Design: <a href=”#”>Lucy</a>
</div>
<div id=”l”>
      <a href=”#”>XHTML</a> - <a href=”#”>CSS</a>
</div>
</footer>
```
***
# 分组元素
***
## hgroup 元素
hgroup 元素是将标题及其子标题进行分组的元素。<br/>
- **使用时遵循以下条件：<br/>**
     - 有一个以上标题元素；
     - 当一个标题有副标题、其他section或者article的元数据时，建议将hgroup元素和元数据放到一个单独的header 元素容器中。

```html
<header>
   <hgroup>
       <h1>茶叶模板</h1>
       <h2>各种茶类</h2>
</hgroup>
</header>
```
***
# figcaption 和 figure
figcaption元素用于定义figure 元素的标题，该元素应该被放到figure 元素的第一个或者最后一个子元素的位置。<br/>
figure 元素指定独立的流内容，例如图像、图表、照片和代码。figure元素的内容应该与主内容无关，如果被删除，则不会对文章流产生影响。在使用figure元素时，可以通过figcaption元素添加标题。一个figure元素最多只允许放置一个figcaption元素。
***
# 文本语义元素
***
## mark 元素
mark 元素表示页面中需要突出显示或高亮显示的对于当前用户具有参考作用的一段文字。
- **通常作用在两方面：**

     -  对网页全文检索某个关键词时显示的检验结果;
     -  引用原文时，为了某种特殊目的而把原文作者没有特别重点标示的内容表示出来。
- **mark 、strong、em元素的区别：**
     - mark 元素与原文作者无关，在后来引用时添加上去的；
     - strong元素是原文作者用来强调一段文字的重要性（如警告信息）
     - em元素是作者为了突出文章重点而使用的。
***
## wbr 元素
wbr 元素指定在文本中的何处适合添加换行符,决定在此处换行。
***
# 交互元素
***
## meter 元素
meter元素是用来定义度量衡的元素。
```html
<p>
	徐海：<meter low="69" high="80" max="100" optimum="100" value="92">A</meter>
	陈露：<meter low="69" high="80" max="100" optimum="100" value="72">C</meter>
	李雪：<meter low="69" high="80" max="100" optimum="100" value="52">E</meter>
</p>
```
- **meter元素的常用属性：**
     - value：在元素中特地表现出来的实际值；
     - min：定义允许范围内的最小值，默认值为0；
     - max：定义允许范围内的最大值，默认值为1；
     - low：定义范围内的下限值；
     - high：定义范围内的上限值；
     - optimum：最佳值。
***
## progress 元素
progress元素代表一个任务的完整进度。它具有两个属性：value属性表示已经完成了多少工作量；max属性表示总共有多少工作量。两个属性只能指定为有效的浮点数，value属性的值必须大于0 ，且小于或等于max属性的值，max属性的值必须大于0。
```html
<section>
	<h1>dajihao </h1>
	<p><progress value="45" max="100"><span>45%</span></progress></p>
</section
```
***
## details 元素
details元素用于说明文档或某个细节信息的作用。<br/>
**open**属性定义details是否可见。
**summary**元素用来定义details元素的标题。  

***
# 音频和视频元素
***
## video 元素
```html
<video  src=”URL”  width=”宽度”  height=”高度”  controls  autoplay  preload  loop  poster=”URL”>
浏览器不支持video元素  //以防有些浏览器不支持video元素
</video>
```
- **Preload属性包含三个可选择的值：**
     - None：表示不进行预加载；
     - Metadata：表示只预加载媒体的元数据（媒体字节数、第一帧、播放列表和持续时间等）。
     - Auto：默认值，表示于嘉在全部视频。
***
# audio 元素
audio元素不能通过width和height来设置音频播放器的宽度和高度，需要使用CSS样式来指定。（CSS样式指定一般高度为45px）不能使用poster属性。
***
# 标准属性
***
## hidden 属性
Hidden属性是一个布尔属性，属性值为true时，元素处于不可见状态；属性值为false时，元素处于可见状态。
```html
<input type="button" id="btn" value="显示" onclick="show()" />
		<p hidden id="showp">本实力三分归元气，七分靠打拼过，四级词汇，水浒传，红楼梦，西游记，三国演义</p>
<script type="text/javascript">
			var btn=document.getElementById("btn");
			function show(){
				var p=document.getElementById("showp");
				if (btn.value=="显示") {
					btn.value="隐藏";
					p.hidden=false;
				} else{
					btn.value="显示";
					p.hidden=true;
				}
			}
</script>
```
## contenteditable 属性
contenteditable是一个布尔值，属性值设置为true时，元素被指定为允许编辑；属性值设置为false时，元素被指定为不可编辑。
***
# spellcheck 属性
spellcheck属性是一个布尔值，属性值设置为true时，会对用户输入的文本内容进行拼写和语法检查；当属性值设置为false时则不会。















