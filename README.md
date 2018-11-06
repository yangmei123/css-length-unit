### css常用尺寸单位总结（待续）

> 常用的字体一些理解，rem要配合js，都把字体设置为屏幕的100分之一；
> 事件resize触发非常高频，尽量不要在回调函数里对dom进行计算修改，建议使用requestAnimationFrame, setTimeout or customEvent这些事件加速渲染；
#### requestAnimationFrame 来实现视觉变化
当屏幕正在发生视觉变化时，您希望在适合浏览器的时间执行您的工作，也就是正好在帧的开头。保证 JavaScript 在帧开始时运行的唯一方式是使用 requestAnimationFrame。(频率每秒60次)当需要更新浏览器画面时就可以调用，在浏览器下次重绘前执行回调函数。IE10

#### setTimeout
每个task执行完毕都会渲染页面
> 最小字体是10px
> 兼容性

#### 了解 JavaScript 的“帧税”
> https://developers.google.com/web/fundamentals/performance/rendering/optimize-javascript-execution?hl=zh-cn
在评估一个框架、库或您自己的代码时，务必逐帧评估运行 JavaScript 代码的开销。当执行性能关键的动画工作（例如变换或滚动）时，这点尤其重要。

测量 JavaScript 开销和性能情况的最佳方法是使用 Chrome DevTools 的timeline (58版本后改为performance monitor)
## em
## percent
## px
## rem
## vh
## vw

![Image text](https://github.com/yangmei123/css-length-unit/blob/master/demo.gif)

