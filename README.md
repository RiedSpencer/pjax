# pjax
pushState就是 web history api，用于进行ajax刷新的时候记住状态，也就是说通过在url地址加参的方式进行f5刷新的时候，ajax不会从头开始，属于html5的特性，对于ie党还是有点尬。

主要有5个函数，back,forward,go,pushState，replaceState，

前面三个函数里面的参数都是数字

pushState（state object,title,url）:
state object:状态对象，与历史记录相关的一个js对象
title：可选，已经被忽略
url：浏览器地址，可以绝对也可以相对直接在后面加上?url=xxx,绝对地址必须和以前的地址同源，也就是说？前面的内容不能变

placeState（state object,title,url）:
跟pushState的参数是一样的

其实url不一定需要参数一样?param=XXX,直接在后面接上 xxx也是可以的，
在这个demo里面只有模拟ajax的动作，并没有写真实的ajax异步刷新


