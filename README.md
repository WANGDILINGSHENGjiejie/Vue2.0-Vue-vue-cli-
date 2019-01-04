# Vue2.0-Vue-vue-cli-
Vue.js是一套构建用户界面的渐进式框架。 Vue 只关注视图层，采用自底向上增量开发的设计。 Vue 的目标是通过尽可能简单的 API 实现响应的数据绑定和组合的视图组件。

# 阅读之前需要了解的知识(htnl. css .javascript .node.js环境(npm包管理工具） .webpack打包工具)

# 安装node.js
从node官网下载并安装node，安装步骤很简单，只要一路“next”就可以了。
安装完成后，打开命令行工具输入命令node -v，如果出现对应版本号，就说明安装成功了。
我们所需要的npm包管理器，是集成在node中的，所以，直接输入npm -v就会显示出npm的版本信息。
到这里node的环境已经安装完了,npm包管理工具也有了，但是由于npm的有些资源被墙，为了更快更稳定,所以我们需要切换到淘宝的npm镜像——cnpm。

# 安装cnpm
进入淘宝的cnpm网站,里面有详细的配置方法。
或者直接在命令行输入：

$ npm install -g cnpm --registry=https://registry.npm.taobao.org
然后等待，安装完成。

输入cnpm -v，可以查看当前cnpm版本，这个和npm的版本还是不一样的。

## 使用cnpm的方法就是，需要用到npm的地方直接使用cnpm替换就可以了

在用 vue.js 构建大型应用时推荐使用 npm 安装，npm 能很好地和诸如 webpack 或 browserify 模块打包器配合使用。vue.js 也提供配套工具来开发单文件组件。

$ cnpm install vue

# 安装vue-cli脚手架构建工具
vue-cli 提供一个官方命令行工具，可用于快速搭建大型单页应用。该工具提供开箱即用的构建工具配置，带来现代化的前端开发流程。只需几分钟即可创建并启动一个带热重载、保存时静态检查以及可用于生产环境的构建配置的项目：

# 全局安装 vue-cli
$ cnpm install --global vue-cli
创建一个基于 webpack 模板的新项目
要创建项目，首先我们要选定目录，然后再命令行中把目录转到选定的目录。可以使用：

# my-project为自定义项目名
$ vue init webpack my-project
初始化一个项目，或使用

$ vue init webpack-simple my-project
初始化一个简单的项目
运行初始化命令的时候回让用户输入几个基本的选项，如项目名称，描述，作者等信息，如果不想填直接回车默认就好。

需要注意的是项目的名称不能大写，不然会报错。

Project name (my-project) # 项目名称（我的项目）

Project description (A Vue.js project) # 项目描述一个Vue.js 项目

Author 作者（你的名字）

Install vue-router? (Y/n) # 是否安装Vue路由，也就是以后是spa（单页面应用需要的模块）

Use ESLint to lint your code? (Y/n) # 使用 ESLint 到你的代码？ （Y [ yes ] / N [ no ]）

Pick an ESLint preset (Use arrow keys) # 选择一个预置ESLint（使用箭头键）

Setup unit tests with Karma + Mocha? (Y/n) # 设置单元测Karma + Mocha？ （Y/ N）

Setup e2e tests with Nightwatch? (Y/n) # 设置端到端测试，Nightwatch？ （Y/ N）

当然这些都看你自己个人的情况，我这里是全选了是。

# 安装项目所需要的依赖
刚初始化的项目是没有依赖的，如果运行会报类似这样的错误，

clipboard.png

所以在这之前需要解决项目的依赖问题，使用下面的命令安装项目的依赖。

$ cnpm install
如果出现如下图情况，说明依赖解决成功。

# 运行项目
$ cnpm run dev

看到Welcome to Your Vue.js App界面，说明配置成功
