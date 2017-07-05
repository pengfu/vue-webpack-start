# vue-webpack-start

> A Vue.js project

## 备注

- output.publicPath 表示生成js或者css嵌入html中的引用路径。这里，我修改了config.build.assetsPublicPath为‘’，否则引用路径会有点小问题。

- 配置了resolve extensions属性，解析时，可以省略后面的后缀名，例如，`import App from './components/App';` 不用写成`import App from './components/App.jsx`
```javascript
resolve: {
       extensions: ['.js', '.jsx'],
},
```
