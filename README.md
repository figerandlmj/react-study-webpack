# 搭建 webpack + React 开发环境

## 初始化npm

mkdir react-study-webpack

npm init

## 安装插件

### dependencies:--save，项目在运行时必须依赖的插件

react react-dom

### devDependencies:--save-dev，项目在开发过程中使用的插件

webpack webpack-dev-server

open-browser-webpack-plugin //webpack启动时自动打开浏览器插件

html-webpack-plugin //处理html模板文件

extract-text-webpack-plugin //将css代码分离出来

less less-loader //less文件处理

css-loader style-loader //css文件处理

postcss-loader autoprefixer //css3加前缀

url-loader file-loader //处理资源文件，如图片、字体等

json-loader //处理.json文件

babel-core babel-loader //es6转码

babel-preset-es2015 babel-preset-react //babel转码规则

babel-plugin-react-transform //babel插件，通过任意转换的方式封装react组件

react-transform-hmr //react转换装置，热重载react类

koa koa-router //页面路由处理

eslint eslint-loader //js检测器，允许检测babel代码

## 配置webpack.config.js

### npm start

package.json:

"start": "set NODE_ENV=dev && webpack-dev-server --progress --colors"

## 配置 webpack.production.config.js

### npm run build

注意执行前确保有build文件夹，否则报错

package.json:

"build": "rd/s/q build && set NODE_ENV=production && webpack --config ./webpack.production.config.js --progress --colors"







