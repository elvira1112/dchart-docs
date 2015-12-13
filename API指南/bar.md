# bar

## 基本方法

### new Bar(selector[, options])

#### selector
类型：`string`或`object`

同new Chart(selector[, options]) 的selector一样

#### options
类型：`object`

##### options.xaxis.key
类型：`string`

默认为"x"。

##### options.xaxis.type
类型：`string`

默认为"category", 类目型。即{"周一", "周二", "周三"...}这种类型。

##### options.xaxis.orient
类型：`string`

默认为"bottom"型。

#### bar.data([data])
与[chart.data([data])](./chart.md)一样。

## chart.render([data])

图表绘制命令，可以带数据，也可以不带（一般不带是已经用过chart.data(data)方法了）


## chart.destroy()
销毁图表命令。

## chart.on(event_name, func)
图表监听事件，实现方法。


