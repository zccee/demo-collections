# Webpack Learning


### 特点

- 基于Node.js
- 自动化打包
- 根据依赖关系来打包静态资源文件


### 核心

- 入口(entry)
- 输出(output)
- loader
- 插件(plugins)


### 链接

- [官方网址](https://webpack.js.org/)
- [学习资源](https://segmentfault.com/a/1190000006178770) - 非常感谢，很适合入门，较为详细，且作者有维护


### 安装

- 基于node，安装node+npm+cnpm环境
```bash
    
   === 安装操作，此处不表 ===========================

    node -v
    npm -v 
    cnpm -v
    
   ===========================
```

- 全局安装webpack
```bash
     
   === 安装操作，此处不表 ===========================

    webpack -v
    
   ===========================
```

- 在项目文件中生成package.json文件（json文件不写注释）
```bash
    
    cnpm init

```

-  项目内部安装webpack以及需要使用的plugins
```bash
    
    === webpack打包常用的loader和plugins（按需加载） ===========================
    
    cnpm install webpack --save-dev

    webpack                   // 全局和项目都需要安装webpack
    webpack-dev-server        // 构建本地服务器

    babel-core                // babel系列
    babel-loader              // babel系列
    babel-env-preset          // babel系列

    style-loader              // loader系列
    css-loader                // loader系列
    postcss-loader            // loader系列

    autoprefixer              // 兼容各个浏览器的前缀
    html-webpack-plugin       // 生成html
    clean-webpack-plugin      // 在build时清除过去哈希文件

    ===========================
```


### 解释

- ...


### 结构

```bash
    
    === "+" 指文件夹，"-" 指文件 ===============================

    + webpack
      + 20171205-init                                       - 某一个项目
        + app                                               - 源码
          - index.tmpl.html
          - main.css
          - main.js
        + build                                             - 生产环境编译代码
          - bundle-*****.js
          - index.html
        + dev                                               - 开发环境编译代码
          - bundle.js
          - index.html
        + node_modules                                      - 相关依赖，不被上传，此处仅仅是做文件结构说明
        - babelrc                                           - babel配置文件
        - package.json                                      - 安装相关依赖以及项目相关信息配置
        - postcss.config.js                                 - postcss的配置文件
        - webpack.config.js                                 - 开发环境webpack配置文件
        - webpack.production.config.js                      - 生产环境webpack的配置文件
      - .gitignore                                          - 需要git忽略的上传文件，不被上传，此处仅仅是做文件结构说明
      - README.md                                           - 说明文档
    
    ===========================
```


### 扩展

- ...


### 项目

- 20171205-init: Webpack Demo


---
Created By Huooo At 2018.02.11 19:30:00 （未完）