# React 版本
- 19.1.0
## import React
- React 17及以下，在写JSX时，Babel需要用到React.createElement去转译原生JavaScript。所以无论是否用到React变量，都要**import React**
- React 17+, Babel 里引入了新的JSX转换方式，即使不显式**import React**，Babel也会自动注入React而不报错；除非你在程序中使用了React变量但是却没有声明。
## creatRoot
- ```creatRoot```是React 18+的新API：支持并发特性（Concurrent Mode）；性能更好、架构更先进；是React官方推荐的写法。
- ```ReactDom.render```是React17及以下的老写法，从React18开始，```ReactDOM.render```已经不推荐使用，也不支持新的并发特性。
## reportWebVitals
- ```reportWebVitals```是Creat React App (CRA) 从 v4开始在脚手架中自动生成的。
- ```reportWebVitals```文件里封装了一个函数，帮助把网页的性能指标（Web Vitals）上报到日志或Google Analytics等第三方分析工具。
- **Web Vitals** 是一些衡量网页性能和用户体验的指标，包括：
  - FCP (First Contentful Paint)
  - LCP (Largest Contentful Paint)
  - CLS (Cumulative Layout Shift)
  - TTFB (Time To First Bite)
  - ……
# Raect开发环境配置
## VS code 插件配置
[react开发者必备vscode插件【2024最新】](https://juejin.cn/post/7337519776794918921)
- ESLint
- Prettier - Code formatter
- Simple React Snippets
- React Developer Tools
- GitLens
- Auto Rename Tag
- Path Intellisense
- Color Highlight
- Code Spell Checker
## 安装Node.js (及npm)
Node.js安装包及源码下载地址为：[https://nodejs.org/en/download](https://nodejs.org/en/download)
安装完成后，打开终端
```
win + R
cmd
```
通过以下命令检查Node.js和npm是否已经安装：
```
node -v 
npm -v
```
输出结果为：
```
v22.16.0
11.4.1
```
## 创建第一个项目
打开终端，进入想要存储项目的目录，使用Creat React App创建项目
```
npx creat-react-app my-app
```
执行成功后，生成项目```my-app/```，项目的目录结构如下：
```
my-app/
├── node_modules/           # 项目依赖库
├── public/                 # 存放静态文件
│   ├── favicon.ico         # 浏览器图标
│   ├── index.html          # 应用的 HTML 模板文件
│   ├── logo192.png         # React logo 图标（192×192）
│   ├── logo512.png         # React logo 图标（512×512）
│   ├── mainfest.json       # Web 应用清单文件
│   ├── robots.txt          # 用于告诉搜索引擎哪些页面可以被抓取
├── src/                    # 存放源代码
│   ├── App.css             # 样式文件
│   ├── App.js              # 主要的 React 组件
│   ├── App.js              # 主要的 React 组件
│   ├── index.css           # 全局样式
│   ├── index.js            # React 入口文件
├── package.json            # 配置信息和依赖列表
└── .gitignore              # Git 忽略文件
```