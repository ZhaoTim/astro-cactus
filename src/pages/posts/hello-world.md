---
setup: |
  import Layout from '@/layouts/BlogPost'
title: Hello World!
publishDate: 13 May 2022
description: Hello world!!! This is an example blog post showcasing some of the cool stuff Astro Cactus theme can do.
---

https://developer.mozilla.org/zh-CN/docs/Web/API/Element/closest
``` js
	  const relativeDom = document.querySelector('.base');
	  const result = relativeDom.closest('.container');
```
`closest`翻译过来是**离得最近的**
上面的代码本质上做的事：
先找到`relativeDom`元素
从`relativeDom`元素沿着父级元素向上寻找元素，这个被寻找的元素要有类名`.container`。
请注意：👆如果`relativeDom`也有`.container`类名，那么也算找到了。也就是说，从`relativeDom`元素开始向上寻找，**包括`relativeDom`元素。**
