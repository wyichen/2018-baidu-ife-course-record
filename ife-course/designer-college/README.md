# 设计学院学习文件夹

## No.1 - 制作一个简单的菜单动画效果

> 原本想开始 MVVM 学院的，发现连入门都困难，算了，还是从简单的开始。'

### 今天做一个简单的动画效果。

[Demo](code/NO01/index.html)

## No.2 - 初步接触 CSS 2D 变形

这两天一边看张鑫旭大神的《CSS 世界》，一边学着动画。动画这一块真心看的头疼，几个变形的关键字还好，自己写出来看看效果就还算深有体会，后面那个 matrix 真的是要把头往墙上撞的呀，好吧，我承认没读完大学的。看了张鑫旭的文章，看不太懂，最后只能开始谷歌大法，最后还是没有弄得很动，只能算是粗略的理解吧，不过倒是有意外收获
[CSS Animations Series](https://www.youtube.com/playlist?list=PLqGj3iMvMa4LvJ8VctoXnPI0dtE40wfid)
youtube 上一个讲 css 动画的视频，那哥们讲的太欢乐了，如果有正好学习到动画的可以看看，唯一的缺点就是英文一句也没听懂，好在牛逼的 youtube 可以自动生成字幕和自动翻译，让我这样的文盲也能看懂视频。

回到任务，要百分之百还原设计稿，卡在了最后一个盒子上，psd 上说是包含以上所有属性，把所有属性放上去，死活就是不一样。刚开始在想是不是图画错了，后来想到是包含所有属性，而没有说属性的值要全部一样。于是开始调各种角度，试了一会儿放弃了，角度怎么弄也弄不到一样的。只能基础 ps 复制大法了，最后直接复制图层的 css 属性，把变形的值复制过来，最后加上平移，算是完了。只是用的 martix，不知道算不算数...

[Demo](code/NO02/index.html)

## No.3 - CSS transition 和 CSS transform 配合制作动画

在`使用 CSS 伪元素触发过渡效果`这个目标中纠结了一会,然后回头想，是不是应该指的的就是hover，任务应该是`使用 CSS 伪类触发过渡效果`，只是写错了写成伪元素了，一定是这样没错的`-_-|||`，嗯，终于把自己说服了。

[Demo](code/NO03/index.html)

## No.4 - 3D 空间的卡片翻转动效

刚开始用的是90度角，会动画的时候会有一个时间两张图片都出现，后来试了下让第二张的执行时间延迟到第一张执行完，这样鼠标移入的动画正常了，但是移出的时候，因为第二张的延迟导致等第二张执行完时，第一张早就执行完了。后来把demo视频放慢看了几遍，才想明白，第二张图片不应该竖着在哪里等着的，应该是跟第一张反着，这样第一张转到90度的时候，正好第二张也变成90度，完成一个交替，然后第二张显示，第一转到背面。加上`backface-visibility:hidden;`就可以让转到背面的图片不显示了。

[Demo](code/NO04/index.html)

## No.5 - 纯 CSS 制作绕中轴旋转的立方体

[Demo](code/NO05/index.html)

## No.6 - 利用 CSS animation 制作一个炫酷的 Slider

[Demo](code/NO06/index.html)

## No.7 - 使用 animate.css 实现一个优雅的登录框

[Demo](code/NO07/index.html)

## No.8 - 把 AE 动画转换成 Web 原生动画

[Demo](code/NO08/index.html)