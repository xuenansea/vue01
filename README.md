# vue01

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


#### 一、安装vue的步骤
    环境：windows64

    1：安装 node.js
        直接安装对应的exe

    2：执行如下命令：（D:\Program Files\nodejs）为文件（node_modules、node.exe）的同级目录，新建“node_global、node_cache”两个文件,
        npm config set prefix "D:\Program Files\nodejs\node_global"
        npm config set cache "D:\Program Files\nodejs\node_cache"

    3：将 node_global 文件加加到计算机的“path”环境变量中，然后安装其他插件，如下：
        环境变量：（重要）
        1）添加：在系统变量新建 NODE_PATH，输入路径为：D:\Program Files\nodejs\node_global\node_modules
        2）在 path 中添加 D:\Program Files\nodejs\node_global
        其他插件
        1）    npm install express -g
        2）    进入node  ,执行：require('express')
        3)     -- 第三步的环境变量直接影响 4 的第二步。

    4：安装 安装淘宝npm（cnpm）
        npm install -g cnpm --registry=https://registry.npm.taobao.org
        cnpm -v

    5：安装webpack：利用cnpm安装webpack
        cnpm install webpack -g     时间略长。测试安装成功的界面如下：
        webpack -v                  验证命令

    6：全局安装vue-cli。时间略长
        cnpm install --global vue-cli
        验证命令:vue -V (V要大写)

    7：新建一个项目：到指定的文件夹下，创建 “vue01” 项目，时间较长
        1）创建完整版vue：vue init webpack vue01
        2）创建简易版vue：vue init webpack-simple vue02

    8：新项目使用淘宝依赖
        cnpm install


#### 二、开发引用参考
    1、添加 “axios” 依赖
        1）cnpm install axios --save
        2）cnpm i axios -S   #缩写参考 i=install 、--save=-S

    2、移除 “axios” 依赖
        1）cnpm uninstall axios -S

    3、其他依赖添加
        1）echarts ：cnpm install echarts --save

#### 三、使用git上传到github
    1、git.exe安装文件路径：D:\Git
    2、计算机cmd进入欲要存放密钥的文件夹，执行 D:\Git\bin\bash.exe
    3、$ ssh-keygen -t rsa -C "登录邮箱"
       $ git config --global user.name "用户名"
       $ git config --global user.email "登录邮箱"
    4、将“xx.pub”内的内容放入 github中的settings->SSH and GPG keys->SSH keys->New ssh key
