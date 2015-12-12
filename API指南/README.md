# API指南

## new Chart(selector[, options])

生成Chart实例，Chart可能为Bar,Pie,Radar等(图表种类请移步[目录结构](../plugin/construct.md))。

### selector
类型：`string`或`object`

选择器可以为[css选择器](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started/Selectors)那样的字符串，也可以为一个DOM结点

> 注：对jquey或者d3选择出来的DOM结点需要再处理，这里只接受原生js选择出来的结点类型 

### options
类型：`object`

这里只介绍全局配置，详细的配置请根据自己绘制的图表看图表中的配置。

#### options.margin
类型：`object`

类似于css中的margin, 用来设置图表中的边距。[图表结构]()详情请戳我。

#### options.width
类型：`number`

用于设置图表画布的宽度。

#### options.height
类型：`number`

用于设置图表画布的高度。

#### options.withAnimated
类型：`number`

图表动画的开关。

#### options.animatedEasing
类型：`number`

图表动画缓动方式。只有当动画开关开启才有作用。

#### options.animatedTiming
类型：`number`

图表动画时间。只有当动画开关开启才有作用。

#### options.withInteract
类型：`number`

图表交互开关。

#### options.theme
类型：`number`

用于设置图表主题。

## chart.data([data])

用于设置或者获取图表数据。当data没有传入时，返回图表数据，当data传入时，设置图表数据。

## chart.render([data])

图表绘制命令，可以带数据，也可以不带（一般不带是已经用过chart.data(data)方法了）

## chart.renderCom(id, type, container, options) 

图表绘制功能性挂件命令

#### id
类型：`string`

功能性挂件id。

#### type
类型：`string`

类似于axis, bg, legend等。[详细的挂件请戳我](../plugin/wedget.md)

#### container
类型：`object`

DOM结点。

#### options

挂件配置，详情见个挂件的介绍。
- [轴](../plugin/wedget/axis.md)
- [背景](../plugin/wedget/bg.md)
- [图例](../plugin/wedget/legend.md)
- [浮动标签](../plugin/wedget/floatTag.md)


## chart.destroy()
销毁图表命令。