# VD 项目样板

VD 内置 Webpack 项目样板相关的 NPM 依赖包描述

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
[webpack](https://webpack.js.org/) | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)](https://github.com/webpack/webpack) | v4.17.1 | - | 用于现代 JavaScript 应用程序的静态模块捆绑器
[webpack-dev-server](https://github.com/webpack/webpack-dev-server) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-dev-server.svg)](https://github.com/webpack/webpack-dev-server) | v3.1.6 | - | Webpack 开发服务
[webpack-merge](https://github.com/survivejs/webpack-merge) | - | -D | [![npm](https://img.shields.io/npm/v/webpack-merge.svg)](https://github.com/survivejs/webpack-merge) | v4.1.4 | - | 为 Webpack 设计的合并（merge）
[copy-webpack-plugin](https://github.com/webpack-contrib/copy-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/copy-webpack-plugin.svg)](https://github.com/webpack-contrib/copy-webpack-plugin) | v4.5.2 | - | 使用 Webpack 复制文件和目录
[clean-webpack-plugin](https://github.com/johnagan/clean-webpack-plugin) | - | -D | [![npm](https://img.shields.io/npm/v/clean-webpack-plugin.svg)](https://github.com/johnagan/clean-webpack-plugin) | v0.1.19 | - | 用于在构建之前删除构建文件夹
[@babel/register](http://babeljs.io/docs/en/next/babel-register) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/register.svg)](http://babeljs.io/docs/en/next/babel-register) | v7.0.0-rc.3 | - | 使 Webpack 配置文件支持 ES6 语法
[cross-env](https://github.com/kentcdodds/cross-env) | - | -D | [![npm](https://img.shields.io/npm/v/cross-env.svg)](https://github.com/kentcdodds/cross-env) | v5.2.0 | - | 运行跨平台设置和使用环境变量的脚本


> JavaScript

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[babel-loader@^8.0.0-beta](https://github.com/babel/babel-loader) | `@babel/core` | -D | [![npm](https://img.shields.io/npm/v/babel-loader.svg)](https://github.com/babel/babel-loader) | v8.0.0-beta.6 | - | 允许你使用 Babel 和 Webpack 转换 JavaScript 文件
[@babel/preset-env](http://babeljs.io/docs/en/next/babel-preset-env) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-env.svg)](http://babeljs.io/docs/en/next/babel-preset-env) | v7.0.0-rc.3 | - | 一个智能预设，允许您使用最新的 JavaScript，而无需微观管理您的目标环境需要哪些语法转换（以及可选的浏览器polyfill）
[@babel/preset-react](http://babeljs.io/docs/en/next/babel-preset-react) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-react.svg)](http://babeljs.io/docs/en/next/babel-preset-react) | v7.0.0-rc.3 | - | React 的预设
[@babel/polyfill](http://babeljs.io/docs/en/next/babel-polyfill) | - | -S | [![npm](https://img.shields.io/npm/v/@babel/polyfill.svg)](http://babeljs.io/docs/en/next/babel-polyfill) | v7.0.0-rc.3 | - | Babel 的 polyfill，转换新语法到 ES5 语法
[react](https://reactjs.org/) | - | -S | [![npm](https://img.shields.io/npm/v/react.svg)](https://github.com/facebook/react/) | v16.4.2 | - | 用户构建用户界面的 JavaScript 库
[react-dom](https://reactjs.org/) | - | -S | [![npm](https://img.shields.io/npm/v/react-dom.svg)](https://github.com/facebook/react/) | v16.4.2 | - | React 的 DOM 绑定库
[react-loadable](https://github.com/jamiebuilds/react-loadable) | - | -S | [![npm](https://img.shields.io/npm/v/react-loadable.svg)](https://github.com/jamiebuilds/react-loadable) | v5.5.0 | - | 用于加载具有动态导入的组件的高阶组件
[react-hot-loader](https://github.com/gaearon/react-hot-loader) | - | -S | [![npm](https://img.shields.io/npm/v/react-hot-loader.svg)](https://github.com/gaearon/react-hot-loader) | v4.3.5 | - | React 热加载（实时调整React组件）
[dva](https://dvajs.com/) | - | -S | [![npm](https://img.shields.io/npm/v/dva.svg)](https://github.com/dvajs/dva) | v2.4.0 | - | 基于 `redux`，`redux-saga` 和 `react-router` 的轻量级前端框架
[dva-loading](https://github.com/dvajs/dva/tree/master/packages/dva-loading) | - | -S | [![npm](https://img.shields.io/npm/v/dva-loading.svg)](https://github.com/dvajs/dva/tree/master/packages/dva-loading) | v2.0.5 | - | dva 的自动 loading 插件
[dva-model-extend](https://github.com/dvajs/dva-model-extend) | - | -S | [![npm](https://img.shields.io/npm/v/dva-model-extend.svg)](https://github.com/dvajs/dva-model-extend) | v0.1.2 | - | 扩展 dva model 的实用方法
~~[babel-plugin-dva-hmr](https://github.com/dvajs/babel-plugin-dva-hmr)~~ | ~~`redbox-react@1.x`~~ | -S | [![npm](https://img.shields.io/npm/v/babel-plugin-dva-hmr.svg)](https://github.com/dvajs/babel-plugin-dva-hmr) | v0.4.1 | - | 用于 dva 的 HMR babel 插件
~~[@babel/plugin-transform-runtime](http://babeljs.io/docs/en/next/babel-plugin-transform-runtime)~~ | ~~`@babel/runtime`~~ | -D | [![npm](https://img.shields.io/npm/v/@babel/plugin-transform-runtime.svg)](http://babeljs.io/docs/en/next/babel-plugin-transform-runtime) | v7.0.0-rc.3 | - | 重复使用 Babel 注入的帮助程序代码来节省代码
~~[react-router-dom](https://reacttraining.com/react-router/):dva~~ | ~~`history`~~ | -S | [![npm](https://img.shields.io/npm/v/react-router-dom.svg)](https://github.com/ReactTraining/react-router/tree/master/packages/react-router-dom) | v4.3.1 | - | `react-router` 的 DOM 绑定库
~~[redux](https://redux.js.org/):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/redux.svg)](https://github.com/reduxjs/redux) | v4.0.0 | - | 可预测状态容器
~~[react-redux](https://redux.js.org/basics/usagewithreact):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/react-redux.svg)](https://github.com/reduxjs/react-redux) | v5.0.7 | - | Redux 的 React 绑定库
~~[redux-saga](https://redux-saga.js.org/):dva~~ | - | -S | [![npm](https://img.shields.io/npm/v/redux-saga.svg)](https://github.com/redux-saga/redux-saga) | v0.16.0 | - | 使应用程序副作用（即异步事物，如数据获取和不纯的东西，如访问浏览器缓存）更容易管理，执行更高效，易于测试，以及更好地处理故障的库
[axios](https://github.com/axios/axios) | - | -S | [![npm](https://img.shields.io/npm/v/axios.svg)](https://github.com/axios/axios) | v0.18.0 | - | 基于 Promise 的 HTTP 客户端，用于浏览器和 node.js
[@babel/preset-stage-1](http://babeljs.io/docs/en/next/babel-preset-stage-1) | - | -D | [![npm](https://img.shields.io/npm/v/@babel/preset-stage-1.svg)](http://babeljs.io/docs/en/next/babel-preset-stage-1) | v7.0.0-rc.3 | - | 预设-阶段-1
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
[style-loader](https://github.com/webpack-contrib/style-loader) | - | -D | [![npm](https://img.shields.io/npm/v/style-loader.svg)](https://github.com/webpack-contrib/style-loader) | v0.22.1 | - | 通过注入 `<style>` 标记将 DOM 添加到 DOM
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
[file-loader]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[url-loader]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[assets-webpack-plugin]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[image-webpack-loader]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[webpack-spritesmith]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[svg-sprite-loader]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## UI 相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[antd]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[babel-plugin-import]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[antd-mobile]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅲ 和 Ⅴ | -
[recharts]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[babel-plugin-recharts]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[react-custom-scrollbars]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 动画相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-motion]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 工具助手

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[moment]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[classnames]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[qs]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[crypto-js]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[lodash]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[babel-plugin-lodash]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[lodash-webpack-plugin]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[browser-sync-webpack-plugin]() | `browser-sync` | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅲ | -
[rework.less]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 性能优化

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[immutable]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[reselect]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[redux-observable]() | `rxjs@6` | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[webpack-bundle-analyzer]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[webpack-dashboard]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 数据伪造

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[mockjs]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[axios-mock-adapter]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 文档生成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-styleguidist]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 语法检测

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[prop-types]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
~~[@babel/preset-flow]()~~ | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[babel-eslint@8]() | `eslint@4.x` | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-react]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-compat]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-import]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-jsx-a11y]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
~~[eslint-plugin-flowtype]()~~ | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-immutable]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[eslint-plugin-promise]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[stylelint]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 测试集成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[babel-jest]() | `jest` | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[react-test-renderer]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[enzyme]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -


## 平台相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[electron@latest]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅱ | -
[electron-builder]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅱ | -
[react-native]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅳ | -
[styled-components]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅳ | -
[babel-plugin-styled-components]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅳ | -
[reactotron-redux-saga]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[reactotron-react-native]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅳ | -
[@babel/cli]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | 仅 Ⅴ | -

## 其他

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-intl]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[babel-plugin-react-intl]() | - | -D | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[react-a11y]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[react-lazyload]() | - | -S | [![npm](https://img.shields.io/npm/v/webpack.svg)]() | v1.0.0 | - | -
[react-loadable-visibility]() | - | -S | [![npm](https://img.shields.io/npm/v/react-loadable-visibility.svg)]() | v1.0.0 | - | -
