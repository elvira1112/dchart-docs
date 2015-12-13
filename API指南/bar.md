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
与[chart.data([data])](./chart.md)一样。用于设置或者获取图表数据。当data没有传入时，返回图表数据，当data传入时，设置图表数据。

