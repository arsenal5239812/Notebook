# React 版本
- 19.1.0
- React 17及以下，在写JSX时，Babel需要用到React.createElement去转译原生JavaScript。所以无论是否用到React变量，都要**import React**
- React 17+, Babel 里引入了新的JSX转换方式，即使不显式**import React**，Babel也会自动注入React而不报错；除非你在程序中使用了React变量但是却没有声明。
# Raect开发环境配置
- 安装Node.ls
- 配置VScode插件
- 安装
