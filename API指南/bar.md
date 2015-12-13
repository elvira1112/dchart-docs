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

### bar.data([data])
与[chart.data([data])](./chart.md)一样。

### chart.render([data])

与[bar.render([data])](./chart.md)一样。


### bar.destroy()
与[chart.destroy()](./chart.md)一样。

### bar.on(event_name, func)
与[chart.on(event_name, func)](./chart.md)一样。


