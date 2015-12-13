# chart

## new Chart(selector[, options])

生成Chart实例，Chart可能为Bar,Pie,Radar等(图表种类请移步[目录结构](./README.md))。

### selector
类型：`string`或`object`

选择器可以为[css选择器](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started/Selectors)那样的字符串，也可以为一个DOM结点

> 注：对jquey或者d3选择出来的DOM结点需要再处理，这里只接受原生js选择出来的结点类型 

### options
类型：`object`

这里只介绍全局配置，详细的配置请根据自己绘制的图表看图表中的配置。

#### options.margin
类型：`object`

类似于css中的margig，内部含left，top，right，bottom。

用来设置图表中的边距。[图表结构]()详情请戳我。

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

#### options.xaxis.key
类型：`string`

x轴key，key即x轴数据对应于数据项中的字段，默认为x。

```
example:
  data = [
    {name : "逗比", age: 18},
    {name : "牛逼", age: 19}
  ];
  
x轴显示的是name字段，所以需要设置key:"name"。
```

#### options.xaxis.type
类型：`string`

x轴的类型，默认为“default”，具体其他类型请戳[轴](../plugin/wedget/axis.md)。

#### options.xaxis.orient
类型：`string`

x轴的方向，默认为“bottom”。

#### options.yaxis.key
类型：`string`

y轴key，key即y轴数据对应于数据项中的字段，默认为y。

#### options.yaxis.type
类型：`string`

y轴的类型，默认为“default”，具体其他类型请戳[轴](../plugin/wedget/axis.md)。

## chart.data([data])

用于设置或者获取图表数据。当data没有传入时，返回图表数据，当data传入时，设置图表数据。

## chart.render([data])

图表绘制命令，可以带数据，也可以不带（一般不带是已经用过chart.data(data)方法了）


## chart.destroy()
销毁图表命令。

## chart.on(event_name, func)
图表监听事件，实现方法。

#### event_name
监听事件列表：

| 事件名 | 参数 | 说明 |
| -- | -- | -- |
| before.render | 无 | 在核心绘制前做的事情 |
| start.beforerender | 无 | 在beforeRender前做的事情 |
| end.beforerender | 无 | 在beforeRender后做的事情 |
| after.render | 无 | 在核心绘制后做的事情 |
| start.afterrender | 无 | 在afterRende前做的事情 |
| end.afterrender | 无 | 在afterRender后做的事情 |
| error | error | 图表出错 |
| series_click | data, event | 点击核心单元事件 |
| series_mouseenter | data, event | 鼠标进入核心单元事件 |
| series_mouseover | data, event | 鼠标移过核心单元事件 |
| series_mouseleave | data, event | 鼠标离开核心单元事件 |

