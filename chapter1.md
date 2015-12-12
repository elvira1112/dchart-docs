# 入门指南

1. 安装dchart
```
    npm install dchart-core
```

2. 作为项目依赖，安装cube
```
    npm install --global cube
```

3. 在页面引入cube
```javascript
    <script type="text/javascript" src="../../cube.min.js"></script>
```

4. 初始化cube
```javascript
    (function () {
        Cube.init({
            base: '/',
            debug: true,
            enableCss: true,  // enbale require css file
            timeout: 20000    // load resource timeout
        });
    })();
```

5. 绘制图表
```javascript
    var Chart = require('dchart-core/bar/bar');
    var chart = new Chart('#selector', options);
    chart.render(data);
```

6. 案例

如果你有源码的话，在根目录运行cube start, 然后访问http://localhost:9999/examples/index.html

#### 下一步要做什么呢？
安装完所有必要的东西，你还需要知道图表的基础配置和数据的规范，请移步[API指南](chapter2.md)



