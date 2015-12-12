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

#### options.animatedEasing
类型：`number`

#### options.animatedTiming
类型：`number`

#### options.withInteract
类型：`number`

#### options.theme
类型：`number`