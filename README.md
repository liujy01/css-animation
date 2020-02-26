# CSS的常用套路
1. 交错动画
---
有时候，我们需要给多个元素添加同一个动画，播放后，不难发现它们会一起运动，一起结束，这样就会显得很平淡无奇。

那么如何将动画变得稍微有趣一点呢？很简单，既然它们都是同一时刻开始运动的，那么让它们不在同一时刻运动不就可以了吗。如何让它们不在同一时刻运动呢？注意到CSS动画有延迟（delay）这一属性。

举个栗子，比如有十个元素播放十个动画，将第二个元素的动画播放时间设定为比第一个元素晚0.5秒（也就是将延迟设为0.5秒），其他元素以此类推，这样它们就会错开来，形成一种独特的视觉效果。

这就是所谓的交错动画：通过设置不同的延迟时间，达到动画交错播放的效果。

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/640.gif)](https://liujy01.github.io/css-animation/demo/jcdh.html)

> Demo :(https://liujy01.github.io/css-animation/demo/jcdh.html)

2. 用JS分割文本
---
还有一种经常用到的玩法：用JS将句子或单词分割成字母，并给每个字母加上不同延时的动画，同样也很华丽。

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/641.gif)](https://liujy01.github.io/css-animation/demo/jsfg1.html)
> Demo :(https://liujy01.github.io/css-animation/demo/jsfg1.html)

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/642.gif)](https://liujy01.github.io/css-animation/demo/jsfg2.html)
> Demo :(https://liujy01.github.io/css-animation/demo/jsfg2.html)

3. 随机粒子动画

---
说到随机性，我们可以实现一种更疯狂的效果：给几百个粒子添加交错动画，并且交错时间随机，位置大小也都是随机。如此一来我们就能用纯CSS模拟出下雪的效果。

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/640.webp)](https://liujy01.github.io/css-animation/demo/sjlz.html)
> Demo :(https://liujy01.github.io/css-animation/demo/sjlz.html)

4. 伪类

---
HTML元素的状态是可以动态变化的。举个栗子，当你的鼠标悬浮到一个按钮上时，按钮就会变成“悬浮”状态，这时我们就可以利用伪类:hover来选中这一状态的按钮，并对其样式进行改变。

:hover是笔者最最常用的一个伪类。还有一个很常用的伪类是:nth-child，用于选中元素的某一个子元素。其他的类似:focus、:focus-within等也有一定的使用。

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/643.gif)](https://liujy01.github.io/css-animation/demo/wl.html)

> Demo :(https://liujy01.github.io/css-animation/demo/wl.html)

5. 绝对定位实现多重边框

---
谁规定按钮只能有一套边框的？利用绝对定位和padding，我们可以给按钮做出3套大小不一的边框来，这样效果更炫了。

[![image](https://raw.githubusercontent.com/liujy01/css-animation/master/imgs/644.gif)](https://liujy01.github.io/css-animation/demo/dcbk.html)

> Demo :(https://liujy01.github.io/css-animation/demo/dcbk.html)