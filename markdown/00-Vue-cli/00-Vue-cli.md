## Vue-cli

### Vue-cli介绍(node包)

```bash
# 目录结构
# 本地调试
# 代码部署
# 热加载
# 单元测试
```
### Vue-cli安装(必须安装node4.1^)

```bash
# 没翻墙尽量使用cnpm
# mac 安装
$ sudo npm install -g vue-cli

# windows
$ npm install -g vue-cli
```
### Usage(项目使用)

```bash
# 查看可使用的模板
$ vue list

# 用Vue-cli初始一个项目,模板名称加项目名称
$ vue init <template-name> <project-name>

# 使用webpack模板初始化项目
$ vue init webpack my-project

# 执行操作
    + Project name :项目名称 ，如果不需要更改直接回车就可以了。注意：这里不能使用大写，所以我把名称改成了vueclitest
    + Project description:项目描述，默认为A Vue.js project,直接回车，不用编写。
    + Author：作者，如果你有配置git的作者，他会读取。
    + Install  vue-router? 是否安装vue的路由插件，我们这里需要安装，所以选择Y
    + Use ESLint to lint your code? 是否用ESLint来限制你的代码错误和风格。我们这里不需要输入n，如果你是大型团队开发，最好是进行配置。
    + setup unit tests with  Karma + Mocha? 是否需要安装单元测试工具Karma+Mocha，我们这里不需要，所以输入n。
    + Setup e2e tests with Nightwatch?是否安装e2e来进行用户行为模拟测试，我们这里不需要，所以输入n。
```
### 运行项目

```bash
$ cd my-project
$ npm install
$ npm run dev
```
### 项目目录介绍

 ```bash
  |-- build                            // 项目构建(webpack)相关代码
  |   |-- build.js                     // 生产环境构建代码
  |   |-- check-version.js             // 检查node、npm等版本
  |   |-- dev-client.js                // 热重载相关
  |   |-- dev-server.js                // 构建本地服务器
  |   |-- utils.js                     // 构建工具相关
  |   |-- webpack.base.conf.js         // webpack基础配置
  |   |-- webpack.dev.conf.js          // webpack开发环境配置
  |   |-- webpack.prod.conf.js         // webpack生产环境配置
  |-- config                           // 项目开发环境配置
  |   |-- dev.env.js                   // 开发环境变量
  |   |-- index.js                     // 项目一些配置变量
  |   |-- prod.env.js                  // 生产环境变量
  |   |-- test.env.js                  // 测试环境变量
  |-- src                              // 源码目录
  |   |-- components                     // vue公共组件
  |   |-- store                          // vuex的状态管理
  |   |-- App.vue                        // 页面入口文件
  |   |-- main.js                        // 程序入口文件，加载各种公共组件
  |-- static                           // 静态文件，比如一些图片，json数据等
  |   |-- data                           // 群聊分析得到的数据用于数据可视化
  |-- .babelrc                         // ES6语法编译配置
  |-- .editorconfig                    // 定义代码格式
  |-- .gitignore                       // git上传需要忽略的文件格式
  |-- README.md                        // 项目说明
  |-- favicon.ico
  |-- index.html                       // 入口页面
  |-- package.json                     // 项目基本信息
  ```


