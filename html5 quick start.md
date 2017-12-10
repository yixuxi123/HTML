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
- 注意：<br/>
1.	section 元素不用做设置样式的页面容器，div 可以。<br/>
2.	没有标题的内容区块不适用section 元素。
***
## nav 元素
nav 元素是一个可以用作页面导航的链接组。只需要将主要的、基本的链接组放进nav 元素即可。<br/>
- nav 元素可以用于以下几种场合：
1.	传统导航条；
2.	侧边栏导航；
3.	页内导航；
4.	翻页操作。
```html
<nav>
 <a href=“#”>首页</a> |  <a href=“#”>新闻动态</a> |  <a href=“#”>规范标准</a> |  <a href=“#”>文章教程</a> |  <a href=“#”>资源链接</a> |  <a href=“#”>常见问题</a> |  <a href=“#”>论坛交流</a> | 
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
hgroup 元素是将标题及其子标题进行分组的元素。
***- 使用时遵循以下条件：
1.	有一个以上标题元素；
2.	当一个标题有副标题、其他section或者article的元数据时，建议将hgroup元素和元数据放到一个单独的header 元素容器中。

```html
<header>
   <hgroup>
       <h1>茶叶模板</h1>
       <h2>各种茶类</h2>
</hgroup>
</header>
```
***
