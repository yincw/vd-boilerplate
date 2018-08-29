# VD 项目样板

VD 内置的 Webpack 项目样板相关的 NPM 依赖包描述

> 目录

- 基本
  - 环境
  - JavaScript
  - CSS
  - HTML
  - 其他资源
- UI 相关
- 动画相关
- 工具助手
- 性能优化
- 数据伪造
- 文档生成
- 语法检测
- 测试集成
- 平台相关
- 其他

> 适用形态

- Ⅰ：PC Web（+）
- Ⅱ：PC Native（+）
- Ⅲ：Mobile Web（+）
- Ⅳ：Mobile Native
- Ⅴ：Library（+）
- Ⅵ：Node Server

## 基本

> 环境

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[**webpack**](https://webpack.js.org/) | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)](https://github.com/webpack/webpack) | v4.17.1 | - | 用于现代 JavaScript 应用程序的静态模块捆绑器
[**webpack-dev-server**](https://github.com/webpack/webpack-dev-server) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-dev-server.svg)](https://github.com/webpack/webpack-dev-server) | v3.1.6 | - | Webpack 开发服务
[**webpack-merge**](https://github.com/survivejs/webpack-merge) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-merge.svg)](https://github.com/survivejs/webpack-merge) | v4.1.4 | - | 为 Webpack 设计的合并（merge）
[**copy-webpack-plugin**](https://github.com/webpack-contrib/copy-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/copy-webpack-plugin.svg)](https://github.com/webpack-contrib/copy-webpack-plugin) | v4.5.2 | - | 使用 Webpack 复制文件和目录
[**clean-webpack-plugin**](https://github.com/johnagan/clean-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/clean-webpack-plugin.svg)](https://github.com/johnagan/clean-webpack-plugin) | v0.1.19 | - | 用于在构建之前删除构建文件夹
[**@babel/register**](http://babeljs.io/docs/en/next/babel-register) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/register.svg)](http://babeljs.io/docs/en/next/babel-register) | v7.0.0 | - | 使 Webpack 配置文件支持 ES6 语法
[**cross-env**](https://github.com/kentcdodds/cross-env) | - | -D | [![npm](https://img.shields.io/npm/v/cross-env.svg)](https://github.com/kentcdodds/cross-env) | v5.2.0 | - | 运行跨平台设置和使用环境变量的脚本


> JavaScript

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[**babel-loader**](https://github.com/babel/babel-loader) | `@babel/core` | -D | [![npm](https://img.shields.io/npm/v/babel-loader.svg)](https://github.com/babel/babel-loader) | v8.0.0 | - | 允许你使用 Babel 和 Webpack 转换 JavaScript 文件
[**@babel/preset-env**](http://babeljs.io/docs/en/next/babel-preset-env) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-env.svg)](http://babeljs.io/docs/en/next/babel-preset-env) | v7.0.0 | - | 一个智能预设，允许您使用最新的 JavaScript，而无需微观管理您的目标环境需要哪些语法转换（以及可选的浏览器polyfill）
[**@babel/preset-react**](http://babeljs.io/docs/en/next/babel-preset-react) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-react.svg)](http://babeljs.io/docs/en/next/babel-preset-react) | v7.0.0 | - | React 的预设
[**@babel/polyfill**](http://babeljs.io/docs/en/next/babel-polyfill) | - | -S | [![npm](https://img.shields.io/npm/v/@babel/polyfill.svg)](http://babeljs.io/docs/en/next/babel-polyfill) | v7.0.0 | - | Babel 的 polyfill，转换新语法到 ES5 语法
[**react**](https://reactjs.org/) | - | -S | [![npm](https://img.shields.io/npm/v/react.svg)](https://github.com/facebook/react/) | v16.4.2 | - | 用户构建用户界面的 JavaScript 库
[**react-dom**](https://reactjs.org/) | - | -S | [![npm](https://img.shields.io/npm/v/react-dom.svg)](https://github.com/facebook/react/) | v16.4.2 | - | React 的 DOM 绑定库
[**react-loadable**](https://github.com/jamiebuilds/react-loadable) | - | -S | [![npm](https://img.shields.io/npm/v/react-loadable.svg)](https://github.com/jamiebuilds/react-loadable) | v5.5.0 | - | 用于加载具有动态导入的组件的高阶组件
[**react-hot-loader**](https://github.com/gaearon/react-hot-loader) | - | -S | [![npm](https://img.shields.io/npm/v/react-hot-loader.svg)](https://github.com/gaearon/react-hot-loader) | v4.3.5 | - | React 热加载（实时调整React组件）
[**dva**](https://dvajs.com/) | - | -S | [![npm](https://img.shields.io/npm/v/dva.svg)](https://github.com/dvajs/dva) | v2.4.0 | - | 基于 `redux`，`redux-saga` 和 `react-router` 的轻量级前端框架
[**dva-loading**](https://github.com/dvajs/dva/tree/master/packages/dva-loading) | - | -S | [![npm](https://img.shields.io/npm/v/dva-loading.svg)](https://github.com/dvajs/dva/tree/master/packages/dva-loading) | v2.0.5 | - | dva 的自动 loading 插件
[**dva-model-extend**](https://github.com/dvajs/dva-model-extend) | - | -S | [![npm](https://img.shields.io/npm/v/dva-model-extend.svg)](https://github.com/dvajs/dva-model-extend) | v0.1.2 | - | 扩展 dva model 的实用方法
~~[babel-plugin-dva-hmr](https://github.com/dvajs/babel-plugin-dva-hmr)~~ | ~~`redbox-react@1.x`~~ | -S | [![npm](https://img.shields.io/npm/v/babel-plugin-dva-hmr.svg)](https://github.com/dvajs/babel-plugin-dva-hmr) | v0.4.1 | - | 用于 dva 的 HMR babel 插件
~~[@babel/plugin-transform-runtime](http://babeljs.io/docs/en/next/babel-plugin-transform-runtime)~~ | ~~`@babel/runtime`~~ | -D | [![npm](https://img.shields.io/npm/v/@babel/plugin-transform-runtime.svg)](http://babeljs.io/docs/en/next/babel-plugin-transform-runtime) | v7.0.0 | - | 重复使用 Babel 注入的帮助程序代码来节省代码
~~[redux-observable](https://redux-observable.js.org/)~~ | ~~`rxjs@6`~~ | -S | [![npm](https://img.shields.io/npm/v/redux-observable.svg)](https://github.com/redux-observable/redux-observable) | v1.0.0 | - | 基于 RxJS 6 的 Redux 中间件。撰写和取消异步操作以创建副作用等
~~[react-router-dom](https://reacttraining.com/react-router/):dva~~ | ~~`history`~~ | -S | [![npm](https://img.shields.io/npm/v/react-router-dom.svg)](https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom) | v4.3.1 | - | `react-router` 的 DOM 绑定库
~~[redux](https://redux.js.org/):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/redux.svg)](https://github.com/reduxjs/redux) | v4.0.0 | - | 可预测状态容器
~~[react-redux](https://redux.js.org/basics/usagewithreact):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/react-redux.svg)](https://github.com/reduxjs/react-redux) | v5.0.7 | - | Redux 的 React 绑定库
~~[redux-saga](https://redux-saga.js.org/):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/redux-saga.svg)](https://github.com/redux-saga/redux-saga) | v0.16.0 | - | 使应用程序副作用（即异步事物，如数据获取和不纯的东西，如访问浏览器缓存）更容易管理，执行更高效，易于测试，以及更好地处理故障的库
[**axios**](https://github.com/axios/axios) | - | -S | [![npm](https://img.shields.io/npm/v/axios.svg)](https://github.com/axios/axios) | v0.18.0 | - | 基于 Promise 的 HTTP 客户端，用于浏览器和 node.js
[**@babel/preset-stage-1**](http://babeljs.io/docs/en/next/babel-preset-stage-1) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-stage-1.svg)](http://babeljs.io/docs/en/next/babel-preset-stage-1) | v7.0.0 | - | 预设-阶段-1
[babel-preset-minify](http://babeljs.io/docs/en/next/babel-preset-minify) | - | -D | [![npm](https://img.shields.io/npm/v/babel-preset-minify.svg)](http://babeljs.io/docs/en/next/babel-preset-minify) | v0.4.3 | - | 预设-缩小
[uglifyjs-webpack-plugin](https://github.com/webpack-contrib/uglifyjs-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/uglifyjs-webpack-plugin.svg)](https://github.com/webpack-contrib/uglifyjs-webpack-plugin) | v1.3.0 | - | 使用 UglifyJS v3 （`uglify-es`）来缩小你的 JavaScript
[babel-plugin-transform-react-remove-prop-types](https://github.com/oliviertassinari/babel-plugin-transform-react-remove-prop-types) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-transform-react-remove-prop-types.svg)](https://github.com/oliviertassinari/babel-plugin-transform-react-remove-prop-types) | v0.4.15 | - | 从生产版本中删除不必要的 React propTypes

dva@2.4.0

- dva-core@1.4.0
  - redux-saga@0.16.0
- redux@3.7.2
- react-redux@5.0.5
- react-router-dom@4.1.2
  - history@4.6.3
- react-router-redux@5.0.0-alpha.9
- isomorphic-fetch@2.2.1
- @babel/runtime@7.0.0-beta.46

> CSS

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[style-loader](https://github.com/webpack-contrib/style-loader) | - | -D | [![npm](https://img.shields.io/npm/v/style-loader.svg)](https://github.com/webpack-contrib/style-loader) | v0.23.0 | - | 通过注入 `<style>` 标记将 DOM 添加到 DOM
[css-loader](https://github.com/webpack-contrib/css-loader) | - | -D | [![npm](https://img.shields.io/npm/v/css-loader.svg)](https://github.com/webpack-contrib/css-loader) | v1.0.0 | - | 解析 `@import` 和 `url()`
[less-loader](https://github.com/webpack-contrib/less-loader) | `less` | -D | [![npm](https://img.shields.io/npm/v/less-loader.svg)](https://github.com/webpack-contrib/less-loader) | v4.1.0 | - | 编译 Less 到 CSS
[postcss-loader](https://github.com/postcss/postcss-loader) | - | -D | [![npm](https://img.shields.io/npm/v/postcss-loader.svg)](https://github.com/postcss/postcss-loader) | v3.0.0 | - | 用于使用 PostCSS 处理 CSS 的 webpack 的加载器
[postcss-import](https://github.com/postcss/postcss-import) | - | -D | [![npm](https://img.shields.io/npm/v/postcss-import.svg)](https://github.com/postcss/postcss-import) | v12.0.0 | - | PostCSS 插件内联 `@import` 规则内容
[postcss-preset-env](https://preset-env.cssdb.org/) | - | -D | [![npm](https://img.shields.io/npm/v/postcss-preset-env.svg)](https://github.com/csstools/postcss-preset-env) | v5.3.0 | - | 将现代 CSS 转换为浏览器理解的内容
[cssnano](https://cssnano.co/) | - | -D | [![npm](https://img.shields.io/npm/v/cssnano.svg)](https://github.com/cssnano/cssnano) | v4.1.0 | - | 模块化的 minifier，建立在 PostCSS 生态系统之上
[mini-css-extract-plugin](https://github.com/webpack-contrib/mini-css-extract-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/mini-css-extract-plugin.svg)](https://github.com/webpack-contrib/mini-css-extract-plugin) | v0.4.2 | - | 轻量级 CSS 提取插件
[optimize-css-assets-webpack-plugin](https://github.com/NMFR/optimize-css-assets-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/optimize-css-assets-webpack-plugin.svg)](https://github.com/NMFR/optimize-css-assets-webpack-plugin) | v5.0.0 | - | 用于 优化/最小化 CSS 资产


> HTML

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[html-webpack-plugin](https://github.com/jantimon/html-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/html-webpack-plugin.svg)](https://github.com/jantimon/html-webpack-plugin) | v3.2.0 | - | 简化 HTML 文件的创建，以便为您的 webpack 包提供服务


> 其他资源

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[file-loader](https://github.com/webpack-contrib/file-loader) | - | -D | [![npm](https://img.shields.io/npm/v/file-loader.svg)](https://github.com/webpack-contrib/file-loader) | v2.0.0 | - | 用于 webpack 的文件加载器模块
[url-loader](https://github.com/webpack-contrib/url-loader) | - | -D | [![npm](https://img.shields.io/npm/v/url-loader.svg)](https://github.com/webpack-contrib/url-loader) | v1.1.1 | - | 用于将文件转换为 base64 URI
[assets-webpack-plugin](https://github.com/ztoben/assets-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/assets-webpack-plugin.svg)](https://github.com/ztoben/assets-webpack-plugin) | v3.9.6 | - | 发出带有资源路径的 json 文件
[image-webpack-loader](https://github.com/tcoopman/image-webpack-loader) | - | -D | [![npm](https://img.shields.io/npm/v/image-webpack-loader.svg)](https://github.com/tcoopman/image-webpack-loader) | v4.3.1 | - | 使用 imagemin 缩小 PNG，JPEG，GIF，SVG 和 WEBP 图像
[webpack-spritesmith](https://github.com/mixtur/webpack-spritesmith) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-spritesmith.svg)](https://github.com/mixtur/webpack-spritesmith) | v0.5.2 | - | 使用 spritesmith 和 spritesheet-templates 将一组图像转换为 spritesheet 和 SASS / LESS / Stylus mixins
[svg-sprite-loader](https://github.com/kisenka/svg-sprite-loader) | - | -D | [![npm](https://img.shields.io/npm/v/svg-sprite-loader.svg)](https://github.com/kisenka/svg-sprite-loader) | v3.9.2 | - | 用于创建 SVG 精灵的 Webpack 加载程序


## UI 相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[antd](https://ant.design/) | - | -S | [![npm](https://img.shields.io/npm/v/antd.svg)](https://github.com/ant-design/ant-design) | v3.8.4 | - | 一个 UI 设计语言（PC 端）
[babel-plugin-import](https://github.com/ant-design/babel-plugin-import) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-import.svg)](https://github.com/ant-design/babel-plugin-import) | v1.8.0 | - | 模块化导入 babel 插件
[antd-mobile](https://mobile.ant.design/) | - | -S | [![npm](https://img.shields.io/npm/v/antd-mobile.svg)](https://github.com/ant-design/ant-design-mobile) | v2.2.3 | 仅 Ⅲ 和 Ⅴ | 一个基于 Preact / React / React Native 的 UI 组件库（移动端）
[recharts](http://recharts.org/) | - | -S | [![npm](https://img.shields.io/npm/v/recharts.svg)](https://github.com/recharts/recharts) | v1.1.0 | - | 使用 React 和 D3 构建的重新定义的图表库
[babel-plugin-recharts](https://github.com/recharts/babel-plugin-recharts) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-recharts.svg)](https://github.com/recharts/babel-plugin-recharts) | v1.1.1 | - | 模块化加载 Recharts 组件
[react-custom-scrollbars](https://github.com/malte-wessel/react-custom-scrollbars) | - | -S | [![npm](https://img.shields.io/npm/v/react-custom-scrollbars.svg)](https://github.com/malte-wessel/react-custom-scrollbars) | v4.2.1 | - | React 滚动条组件


## 动画相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-motion](https://github.com/chenglou/react-motion) | - | -S | [![npm](https://img.shields.io/npm/v/react-motion.svg)](https://github.com/chenglou/react-motion) | v0.5.2 | - | 一个解决你动画问题的 spring


## 工具助手

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[moment](http://momentjs.com/) | - | -S | [![npm](https://img.shields.io/npm/v/moment.svg)](https://github.com/moment/moment) | v2.22.2 | - | 一个轻量级的 JavaScript 日期库，用于解析，验证，操作和格式化日期
[classnames](https://github.com/JedWatson/classnames) | - | -S | [![npm](https://img.shields.io/npm/v/classnames.svg)](https://github.com/JedWatson/classnames) | v2.2.6 | - | 一个简单的JavaScript实用程序，用于有条件地将classNames连接在一起
[qs](https://github.com/ljharb/qs) | - | -S | [![npm](https://img.shields.io/npm/v/qs.svg)](https://github.com/ljharb/qs) | v6.5.2 | - | 查询字符串解析和字符串化库，增加了一些安全性
[crypto-js](https://github.com/brix/crypto-js) | - | -S | [![npm](https://img.shields.io/npm/v/crypto-js.svg)](https://github.com/brix/crypto-js) | v3.1.9-1 | - | 标准的 JavaScript 加密库
[lodash](https://lodash.com/) | - | -S | [![npm](https://img.shields.io/npm/v/lodash.svg)](https://github.com/lodash/lodash) | v4.17.10 | - | 一个现代 JavaScript 实用程序库，提供模块化，性能和附加功能
[babel-plugin-lodash](https://github.com/lodash/babel-plugin-lodash) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-lodash.svg)](https://github.com/lodash/babel-plugin-lodash) | v3.3.4 | - | 模块化 Lodash 构建
[lodash-webpack-plugin](https://github.com/lodash/lodash-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/lodash-webpack-plugin.svg)](https://github.com/lodash/lodash-webpack-plugin) | v0.11.5 | - | 更小的模块化 Lodash 构建
[browser-sync-webpack-plugin](https://github.com/Va1/browser-sync-webpack-plugin) | `browser-sync` | -D | [![npm](https://img.shields.io/npm/v/browser-sync-webpack-plugin.svg)](https://github.com/Va1/browser-sync-webpack-plugin) | v2.2.2 | 仅 Ⅲ | 在 Webpack 项目中轻松使用 BrowserSync
[rework.less](https://github.com/yincw/rework.less) | - | -S | [![npm](https://img.shields.io/npm/v/rework.less.svg)](https://github.com/yincw/rework.less) | v1.0.0 | - | 一种面向浏览器用户代理样式（user agent stylesheet）兼容的解决方案


## 性能优化

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[immutable](http://facebook.github.io/immutable-js/) | - | -S | [![npm](https://img.shields.io/npm/v/immutable.svg)](https://github.com/facebook/immutable-js) | v3.8.2 | - | Javascript 的不可变持久数据集合，可提高效率和简单性
[reselect](https://github.com/reduxjs/reselect) | - | -S | [![npm](https://img.shields.io/npm/v/reselect.svg)](https://github.com/reduxjs/reselect) | v3.0.1 | - | Redux 的选择器库
[webpack-bundle-analyzer](https://github.com/webpack-contrib/webpack-bundle-analyzer) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-bundle-analyzer.svg)](https://github.com/webpack-contrib/webpack-bundle-analyzer) | v2.13.1 | - | 使用交互式可缩放树形图可视化 webpack 输出文件的大小
[webpack-dashboard](https://github.com/FormidableLabs/webpack-dashboard) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-dashboard.svg)](https://github.com/FormidableLabs/webpack-dashboard) | v2.0.0 | - | Webpack dev 服务器的 CLI 仪表板


## 数据伪造

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[mockjs](http://mockjs.com/) | - | -D | [![npm](https://img.shields.io/npm/v/mockjs.svg)](https://github.com/nuysoft/Mock) | v1.0.1-beta3 | - | 生成随机数据，拦截 Ajax 请求
[axios-mock-adapter](https://github.com/ctimmerm/axios-mock-adapter) | - | -D | [![npm](https://img.shields.io/npm/v/axios-mock-adapter.svg)](https://github.com/ctimmerm/axios-mock-adapter) | v1.15.0 | - | Axios 适配器，允许轻松模拟请求


## 文档生成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-styleguidist](https://react-styleguidist.js.org/) | - | -D | [![npm](https://img.shields.io/npm/v/react-styleguidist.svg)](https://github.com/styleguidist/react-styleguidist) | v7.3.0 | - | 隔离的 React 组件开发环境，带有生活方式指南


## 语法检测

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[prop-types](https://github.com/facebook/prop-types) | - | -S | [![npm](https://img.shields.io/npm/v/prop-types.svg)](https://github.com/facebook/prop-types) | v15.6.2 | - | 运行时类型检查 React props 和类似对象
~~[@babel/preset-flow](http://babeljs.io/docs/en/next/babel-preset-flow)~~ | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-flow.svg)](http://babeljs.io/docs/en/next/babel-preset-flow) | v7.0.0 | - | Babel 预设-Flow
[babel-eslint@8](https://github.com/babel/babel-eslint) | `eslint@4.x` | -D | [![npm](https://img.shields.io/npm/v/babel-eslint.svg)](https://github.com/babel/babel-eslint) | v8.0.0 | - | 允许您使用梦幻般的 ESLint 来提示所有有效的 Babel 代码
[eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-react.svg)](https://github.com/yannickcr/eslint-plugin-react) | v7.11.1 | - | 响应 ESLint 的特定 linting 规则
[eslint-plugin-compat](https://github.com/amilajack/eslint-plugin-compat) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-compat.svg)](https://github.com/amilajack/eslint-plugin-compat) | v2.5.1 | - | 提示您的代码的浏览器兼容性
[eslint-plugin-import](https://github.com/amilajack/eslint-plugin-compat) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-import.svg)](https://github.com/amilajack/eslint-plugin-compat) | v2.14.0 | - | 支持 ES2015 +（ES6 +）导入/导出语法的 linting，并防止错误拼写文件路径和导入名称的问题
[eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-jsx-a11y.svg)](https://github.com/evcohen/eslint-plugin-jsx-a11y) | v6.1.1 | - | 用于JSX元素的可访问性规则的静态AST检查器
~~[eslint-plugin-flowtype]()~~ | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-flowtype.svg)]() | v2.50.0 | - | ESLint 的流类型 linting 规则
[eslint-plugin-immutable](https://github.com/jhusain/eslint-plugin-immutable) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-immutable.svg)](https://github.com/jhusain/eslint-plugin-immutable) | v1.0.0 | - | 在 JavaScript 中禁用所有突变（实现严格的不可变数据）
[eslint-plugin-promise](https://github.com/xjamundx/eslint-plugin-promise) | - | -D | [![npm](https://img.shields.io/npm/v/eslint-plugin-promise.svg)](https://github.com/xjamundx/eslint-plugin-promise) | v4.0.0 | - | 实施 JavaScript 承诺的最佳实践
[stylelint](https://stylelint.io/) | - | -D | [![npm](https://img.shields.io/npm/v/stylelint.svg)](https://github.com/stylelint/stylelint) | v9.5.0 | - | 一个强大的，现代的 linter，可以帮助您避免错误并在您的样式中强制执行约定


## 测试集成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[babel-jest](https://github.com/facebook/jest/tree/master/packages/babel-jest) | `jest` | -D | [![npm](https://img.shields.io/npm/v/babel-jest.svg)](https://github.com/facebook/jest/tree/master/packages/babel-jest) | v23.4.2 | - | Jest 的 Babel 解析器
[react-test-renderer](https://github.com/facebook/react/tree/master/packages/react-test-renderer) | - | -D | [![npm](https://img.shields.io/npm/v/react-test-renderer.svg)](https://github.com/facebook/react/tree/master/packages/react-test-renderer) | v16.4.2 | - | 用于将 React 组件呈现为纯 JavaScript 对象，而不依赖于 DOM 或本机移动环境
[enzyme](http://airbnb.io/enzyme/) | `enzyme-adapter-react-16` | -D | [![npm](https://img.shields.io/npm/v/enzyme.svg)](https://github.com/airbnb/enzyme) | v3.5.0 | - | Enzyme 是 React 的 JavaScript 测试实用程序，可以更容易地断言，操作和遍历 React Components 的输出


## 平台相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[electron@latest](https://electronjs.org/) | - | -D | [![npm](https://img.shields.io/npm/v/electron.svg)](https://github.com/electron/electron) | v2.0.8 | 仅 Ⅱ | 使用 JavaScript, HTML 和 CSS 构建跨平台的桌面应用
[electron-builder](https://www.electron.build/) | - | -D | [![npm](https://img.shields.io/npm/v/electron-builder.svg)](https://github.com/electron-userland/electron-builder) | v20.28.3 | 仅 Ⅱ | 打包并构建一个准备好分发的 Electron 应用程序，支持开箱即用的“自动更新”支持
[react-native](https://facebook.github.io/react-native/) | - | -S | [![npm](https://img.shields.io/npm/v/react-native.svg)](https://github.com/facebook/react-native) | v0.56.0 | 仅 Ⅳ | 使用 JavaScript 和 React 构建原生移动应用程序
[styled-components](https://www.styled-components.com/) | - | -S | [![npm](https://img.shields.io/npm/v/styled-components.svg)](https://github.com/styled-components/styled-components) | v3.4.5 | 仅 Ⅳ | 使用 ES6 和 CSS 的最佳位来设计应用程序，而不会产生压力
[babel-plugin-styled-components](https://github.com/styled-components/babel-plugin-styled-components) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-styled-components.svg)](https://github.com/styled-components/babel-plugin-styled-components) | v1.5.1 | 仅 Ⅳ | 改进调试体验，并为 `styled-components` 添加服务器端呈现支持
[react-navigation](https://reactnavigation.org/) | - | -D | [![npm](https://img.shields.io/npm/v/react-navigation.svg)](https://github.com/react-navigation/react-navigation) | v2.12.1 | 仅 Ⅳ | React Native 应用程序的路由和导航
[reactotron-react-native](https://github.com/infinitered/reactotron/blob/master/docs/quick-start-react-native.md) | - | -D | [![npm](https://img.shields.io/npm/v/reactotron-react-native.svg)](https://github.com/infinitered/reactotron/blob/master/docs/quick-start-react-native.md) | v2.1.0 | 仅 Ⅳ | 检查你的 React Native 项目
[reactotron-redux-saga](https://github.com/infinitered/reactotron/blob/master/docs/plugin-redux-saga.md) | - | -D | [![npm](https://img.shields.io/npm/v/reactotron-redux-saga.svg)](https://github.com/infinitered/reactotron/blob/master/docs/plugin-redux-saga.md) | v2.1.0 | - | 检查你的 React（使用 Redux Saga） 项目
[@babel/cli](http://babeljs.io/docs/en/next/babel-cli) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/cli.svg)](http://babeljs.io/docs/en/next/babel-cli) | v7.0.0 | 仅 Ⅴ | 用于从命令行编译文件

## 其他

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-intl](https://github.com/yahoo/react-intl) | - | -S | [![npm](https://img.shields.io/npm/v/react-intl.svg)](https://github.com/yahoo/react-intl) | v2.4.0 | - | 国际化React应用程序。该库提供了React组件和API，用于格式化日期，数字和字符串，包括复数和处理翻译
[babel-plugin-react-intl](https://github.com/yahoo/babel-plugin-react-intl) | - | -D | [![npm](https://img.shields.io/npm/v/babel-plugin-react-intl.svg)](https://github.com/yahoo/babel-plugin-react-intl) | v2.4.0 | - | 从使用 React Intl 的模块中提取字符串消息以进行转换
[react-a11y](https://github.com/reactjs/react-a11y) | - | -S | [![npm](https://img.shields.io/npm/v/react-a11y.svg)](https://github.com/reactjs/react-a11y) | v1.0.0 | - | 标识 React.js 元素中的可访问性问题
[react-lazyload](https://github.com/jasonslyvia/react-lazyload) | - | -S | [![npm](https://img.shields.io/npm/v/react-lazyload.svg)](https://github.com/jasonslyvia/react-lazyload) | v2.3.0 | - | 延迟加载您的组件，图像或任何重要的性能
[react-loadable-visibility](https://github.com/stratiformltd/react-loadable-visibility) | - | -S | [![npm](https://img.shields.io/npm/v/react-loadable-visibility.svg)](https://github.com/stratiformltd/react-loadable-visibility) | v2.5.0 | - | `react-loadable` 和 `loadable-components` 的包容容器，用于加载页面上可见的元素
[react-sketchapp](http://airbnb.io/react-sketchapp/) | - | -S | [![npm](https://img.shields.io/npm/v/react-sketchapp.svg)](https://github.com/airbnb/react-sketchapp/) | v2.0.0 | - | 渲染 React 组件到 Sketch; 为设计系统量身定制
