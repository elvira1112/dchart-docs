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




