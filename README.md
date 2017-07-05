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
- vue-cli脚手架模板已经为.vue文件外的样式 sass less等文件配置好，使用时安装特定的loader即可。例如，这个项目中使用sass，只需要npm安装sass-loder即可以。由于安装node-sass很慢，项目中新建了一个.npmrc文件，其中放置npm相关淘宝源地址。
```javascript
sass_binary_site=https://npm.taobao.org/mirrors/node-sass/
phantomjs_cdnurl=https://npm.taobao.org/mirrors/phantomjs/
electron_mirror=https://npm.taobao.org/mirrors/electron/
registry=https://registry.npm.taobao.org
```
