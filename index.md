# 0905笔记

npm node package manage的缩写 node包管理工具  安装node环境的时候,会自带这个npm
yarn 干净 速度较快
npm cnpm 淘宝镜像 
为什么用cnpm代替npm呢? 很多包是在国外的网站, google facebook youtube 被墙了
cnpm是淘宝的 每10分钟会自动更新包数据 


npm install -g cnpm --registry=https://registry.npm.taobao.org 

https://cli.vuejs.org/zh/ 官方中文网址

 vue create vue-cli 创建指令

 -webkit-xxx
 -o-xxxx

 路由模式 hash history  hash 带#  history模式在线上的话 需要配合服务端去做拦截才会生效 在本地的话 直接使用即可

 sass/scss  sass是老版本 scss是新版本
 dart-sass node-sass 建议用dart-sass 
 node-sass是以前的 包经常会拉取失败 
 dart-sass是新的 底层是用dart编写的 dart其实是google推出的一门语言 是想要将来取代js的 
 flutter 跨平台开发 dart作为编程语言的 
 Bootstrap 现在新版本 也改用了dart作为底部的编程语言


 less css预编译语言
 Stylus 也是css预编译语言

 less 通过一个js脚本在客户端编译 

 babel ES6 => ES5 
 ESLint 语法检测 


package.json 

dependencies 生产依赖 cookie 
devDependencies 开发依赖 babel 


babel.config.js 是babel的配置文件 


vue-router 路由管理 控制跳转
vuex 状态管理 全局的数据状态管理  
父子之间 emit on 

生命周期 钩子函数


vue-resource 官方的数据通信插件 
axios 基于ajax封装的 
vue作者 尤雨溪 推荐axios 

推荐axios


webpack 打包配置  一切皆模块 js文件是一个模块 

webpack的理念 一切皆模块 图片 js css 都是模块 


vue-element-admin 字节跳动的大神 花裤衩

vant 饿了么的移动端UI框架
element 饿了么的PCUI框架
element iview ant dedign vue

<el-button></el-button>
<i-button></i-button> <Button></Button>

vue的原理 千千万万的框架 问不过来 上手一个UI框架很快 



vue react
vue 是一个 个人框架
react facebook 出品的一个库  

MVVM 是一种系统架构模式 
vue用的就是MVVM
M V VM 
model view viewmodel
数据  视图  视图数据

改变 model 之后 通过  viewmodel 来改变 view
改变 view 之后 通过  viewmodel 来改变 model
viewmodel 相当于一个中间转换层 



var that = this 

tree 组件  

ES6 let const 解构 class Promise generate Symbol Map Set 数组和对象的新方法

ES6 模块的导入 导出
import 导入  export 导出
import xxx from 'xxx'
import {xxx} from 'xxx'
import * from 'xxx'
import {s as sss} from 'xxx' 
import {* as xxx} from 'xxx' 

export const s = 1111
export const s2 = 2222
export const s3 = 333
export s as xx 
export default {}


scoped css样式作用域  加了 scoped 就只会在当前页面生效

create 创建 vNode 虚拟节点
mount 挂载 到某个元素

let div = document.createElement('div') 创建
document.body.appendChild(div) 挂载



## 数据突变
- 突变方法
- 非突变方法

## nextTick
会在下一个节点更新数据 

相当于 setTimeout 

## 事件循环 Event Loop
涉及到浏览器V8引擎的原理 主线程 事件队列

### 事件队列
- 宏任务
- 微任务




























