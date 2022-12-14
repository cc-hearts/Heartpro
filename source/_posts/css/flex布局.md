---
title: flex布局
categories: CSS
---

> flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。 默认不放大(0)
> flex-shrink属性定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。默认的值是(1)
> flex-basis属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。（默认为auto) **(调整该元素的宽高比例进行缩放)**



# align-items

**stretch**
弹性元素被在侧轴方向被拉伸到与容器相同的高度或宽度。

flex: 1 其实是flex-grow, flex-shrink, flex-basis的缩写
&#x20;       对应的值是：flex-grow: 1, flex-shrink: 1, flex-basis: 0%
&#x20;       flex-grow: 扩展，子元素宽度之和小于父元素宽度 那么子元素就会分配父元素剩余的宽度
&#x20;       flex-shrink: 收缩, 子元素宽度之和大于父元素宽度 那么子元素就会按照比列收缩
&#x20;       flex-basis: 是弹性盒子的基准值，在没有设置宽度的情况下宽度由content决定，如果content内容过长就会溢出外层容器，如果设置一个宽度，只要这个宽度小于外层容器的剩余宽度(一般设置为0，这样就可以保证百分之百小于剩余宽度) flex-grow就会起作用 自动分配剩余宽度，这样就可以保证flex-basis的宽度是外层容器的宽度而不是content的宽度，内容也就不会溢出
