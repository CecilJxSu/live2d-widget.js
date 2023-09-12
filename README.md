# live2d-widget.js

此项目是从[原仓库](https://github.com/xiazeyu/live2d-widget.js) fork 出来的个人仓库，用于修复特定的 bug。

# How to use
步骤一：在 package.json 中添加如下代码：
```json
{
    // ...
    "resolutions": {
        // ...
        "live2d-widget": "https://github.com/CecilJxSu/live2d-widget.js"
    }
    // ...
}
```

步骤二：执行 `yarn install` 即可。

以上操作是替换 live2d-widget 依赖，使用本项目的依赖。

# Changes
## 2023-09-12
+ 修复：
    1. 看板娘在页面加载时，只加载动作的其中一个。如果有多个动作时，则不能随机切换其它动作。
    2. 修复：点击看板娘头部区域时，不能切换头部指定的动作。
+ [解决方法](https://github.com/xiazeyu/live2d-widget.js/issues/62)