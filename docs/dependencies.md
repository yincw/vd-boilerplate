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
[webpack]() | - | -D | [![]()]() | v1.0.0 | - | -
[webpack-dev-server]() | - | -D | [![]()]() | v1.0.0 | - | -
[webpack-merge]() | - | -D | [![]()]() | v1.0.0 | - | -
[copy-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[clean-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[@babel/register]() | - | -D | [![]()]() | v1.0.0 | - | -
[cross-env]() | - | -D | [![]()]() | v1.0.0 | - | -


> JavaScript

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[babel-loader@^8.0.0-beta]() | `@babel/core` | -D | [![]()]() | v1.0.0 | - | -
[@babel/preset-env]() | - | -D | [![]()]() | v1.0.0 | - | -
[@babel/preset-react]() | - | -D | [![]()]() | v1.0.0 | - | -
[@babel/polyfill]() | - | -S | [![]()]() | v1.0.0 | - | -
[react]() | - | -S | [![]()]() | v1.0.0 | - | -
[react-dom]() | - | -S | [![]()]() | v1.0.0 | - | -
[react-loadable]() | - | -S | [![]()]() | v1.0.0 | - | -
~~[react-router-dom]():dva~~ | ~~`history`~~ | -S | [![]()]() | v1.0.0 | - | -
~~[redux]():dva~~ | - | -S | [![]()]() | v1.0.0 | - | -
~~[react-redux]():dva~~ | - | -S | [![]()]() | v1.0.0 | - | -
~~[redux-saga]():dva~~ | - | -S | [![]()]() | v1.0.0 | - | -
[axios]() | - | -S | [![]()]() | v1.0.0 | - | -
[dva]() | - | -S | [![]()]() | v1.0.0 | - | -
[dva-loading]() | - | -S | [![]()]() | v1.0.0 | - | -
[babel-plugin-dva-hmr]() | `redbox-react@1.x` | -S | [![]()]() | v1.0.0 | - | -
[dva-model-extend]() | - | -S | [![]()]() | v1.0.0 | - | -
[@babel/plugin-transform-runtime]() | `@babel/runtime` | -D | [![]()]() | v1.0.0 | - | -
[@babel/preset-stage-1]() | - | -D | [![]()]() | v1.0.0 | - | -
[babel-preset-minify]() | - | -D | [![]()]() | v1.0.0 | - | -
[uglifyjs-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[babel-plugin-transform-react-remove-prop-types]() | - | -D | [![]()]() | v1.0.0 | - | -


> CSS

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[style-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[css-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[less-loader]() | `less` | -D | [![]()]() | v1.0.0 | - | -
[postcss-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[postcss-import]() | - | -D | [![]()]() | v1.0.0 | - | -
[postcss-preset-env]() | - | -D | [![]()]() | v1.0.0 | - | -
[cssnano]() | - | -D | [![]()]() | v1.0.0 | - | -
[mini-css-extract-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[optimize-css-assets-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -


> HTML

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[html-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -


> 其他资源

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[file-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[url-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[assets-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[image-webpack-loader]() | - | -D | [![]()]() | v1.0.0 | - | -
[webpack-spritesmith]() | - | -D | [![]()]() | v1.0.0 | - | -
[svg-sprite-loader]() | - | -D | [![]()]() | v1.0.0 | - | -


## UI 相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[antd]() | - | -S | [![]()]() | v1.0.0 | - | -
[babel-plugin-import]() | - | -D | [![]()]() | v1.0.0 | - | -
[antd-mobile]() | - | -S | [![]()]() | v1.0.0 | 仅 Ⅲ 和 Ⅴ | -
[recharts]() | - | -S | [![]()]() | v1.0.0 | - | -
[babel-plugin-recharts]() | - | -D | [![]()]() | v1.0.0 | - | -
[react-custom-scrollbars]() | - | -S | [![]()]() | v1.0.0 | - | -


## 动画相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-motion]() | - | -S | [![]()]() | v1.0.0 | - | -


## 工具助手

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[moment]() | - | -S | [![]()]() | v1.0.0 | - | -
[classnames]() | - | -S | [![]()]() | v1.0.0 | - | -
[qs]() | - | -S | [![]()]() | v1.0.0 | - | -
[crypto-js]() | - | -S | [![]()]() | v1.0.0 | - | -
[lodash]() | - | -S | [![]()]() | v1.0.0 | - | -
[babel-plugin-lodash]() | - | -D | [![]()]() | v1.0.0 | - | -
[lodash-webpack-plugin]() | - | -D | [![]()]() | v1.0.0 | - | -
[browser-sync-webpack-plugin]() | `browser-sync` | -D | [![]()]() | v1.0.0 | 仅 Ⅲ | -
[rework.less]() | - | -S | [![]()]() | v1.0.0 | - | -


## 性能优化

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[immutable]() | - | -S | [![]()]() | v1.0.0 | - | -
[reselect]() | - | -S | [![]()]() | v1.0.0 | - | -
[redux-observable]() | `rxjs@6` | -S | [![]()]() | v1.0.0 | - | -
[webpack-bundle-analyzer]() | - | -D | [![]()]() | v1.0.0 | - | -
[webpack-dashboard]() | - | -D | [![]()]() | v1.0.0 | - | -


## 数据伪造

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[mockjs]() | - | -D | [![]()]() | v1.0.0 | - | -
[axios-mock-adapter]() | - | -D | [![]()]() | v1.0.0 | - | -


## 文档生成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-styleguidist]() | - | -D | [![]()]() | v1.0.0 | - | -


## 语法检测

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[prop-types]() | - | -S | [![]()]() | v1.0.0 | - | -
~~[@babel/preset-flow]()~~ | - | -D | [![]()]() | v1.0.0 | - | -
[babel-eslint@8]() | `eslint@4.x` | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-react]() | - | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-compat]() | - | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-import]() | - | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-jsx-a11y]() | - | -D | [![]()]() | v1.0.0 | - | -
~~[eslint-plugin-flowtype]()~~ | - | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-immutable]() | - | -D | [![]()]() | v1.0.0 | - | -
[eslint-plugin-promise]() | - | -D | [![]()]() | v1.0.0 | - | -
[stylelint]() | - | -D | [![]()]() | v1.0.0 | - | -


## 测试集成

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[babel-jest]() | `jest` | -D | [![]()]() | v1.0.0 | - | -
[react-test-renderer]() | - | -D | [![]()]() | v1.0.0 | - | -
[enzyme]() | - | -D | [![]()]() | v1.0.0 | - | -


## 平台相关

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[electron@latest]() | - | -D | [![]()]() | v1.0.0 | 仅 Ⅱ | -
[electron-builder]() | - | -D | [![]()]() | v1.0.0 | 仅 Ⅱ | -
[react-native]() | - | -S | [![]()]() | v1.0.0 | 仅 Ⅳ | -
[styled-components]() | - | -S | [![]()]() | v1.0.0 | 仅 Ⅳ | -
[babel-plugin-styled-components]() | - | -D | [![]()]() | v1.0.0 | 仅 Ⅳ | -
[reactotron-redux-saga]() | - | -D | [![]()]() | v1.0.0 | - | -
[reactotron-react-native]() | - | -D | [![]()]() | v1.0.0 | 仅 Ⅳ | -
[@babel/cli]() | - | -D | [![]()]() | v1.0.0 | 仅 Ⅴ | -

## 其他

名称 | 依赖 | 安装环境 | NPM 当前版本 | VD 内置版本 | 适用形态 | 功能描述
---|---|---|---|---|---|---
[react-intl]() | - | -S | [![]()]() | v1.0.0 | - | -
[babel-plugin-react-intl]() | - | -D | [![]()]() | v1.0.0 | - | -
[react-a11y]() | - | -S | [![]()]() | v1.0.0 | - | -
[react-lazyload]() | - | -S | [![]()]() | v1.0.0 | - | -
