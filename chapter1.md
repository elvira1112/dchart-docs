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
        Cube.use('index.js', function (App) {
            var chart = new App('#chart');
            chart.render();
        });
    })();
```

5. 

