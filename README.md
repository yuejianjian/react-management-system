# react-admin
react-admin system solution

<img src="https://github.com/yuejianjian/react-management-system/blob/master/tu-1.png"  width="100%" />
<img src="https://github.com/yuejianjian/react-management-system/blob/master/tu-2.png"  width="100%" />
<img src="https://github.com/yuejianjian/react-management-system/blob/master/tu-3.png"  width="100%" />

### 前言
> 网上react后台管理开源免费的完整版项目比较少，所以利用空余时间集成了一个版本出来，已放到GitHub
  启动和打包的时间都稍长，请耐心等待两分钟

- [GitHub地址](https://github.com/yuejianjian/react-management-system/)


### 依赖模块
<span style="color: rgb(184,49,47);">项目是用create-react-app创建的，主要还是列出新加的功能依赖包</span>


- [react](https://facebook.github.io/react/)
- [react-router](https://react-guide.github.io/react-router-cn/)(<span style="color: rgb(243,121,52);">react路由，4.x的版本，如果还使用3.x的版本，请切换分支（ps:分支不再维护）</span>)
- [redux](https://redux.js.org/)(基础用法，但是封装了通用action和reducer，demo中主要用于权限控制（ps：目前可以用16.x的context api代替），可以简单了解下)
- [antd](https://ant.design/index-cn)(<span style="color: rgb(243,121,52);">蚂蚁金服开源的react ui组件框架</span>)
- [axios](https://github.com/mzabriskie/axios)(<span style="color: rgb(243,121,52);">http请求模块，可用于前端任何场景，很强大👍</span>)
- [wangeditor](<span style="color: rgb(243,121,52);">基于javascript和css开发的 Web富文本编辑器</span>)


### 功能模块
<span style="color: rgb(184,49,47);">备注：项目只引入了ant-design的部分组件，其他的组件antd官网有源码，可以直接复制到项目中使用，后续有时间补上全部组件。</span>

<span style="color: rgb(184,49,47);">项目使用了antd的自定义主题功能-->蓝色，若想替换其他颜色，具体操作请查看antd官网</span>
<!--more-->


### 功能截图
#### 首页
![截图](https://raw.githubusercontent.com/yezihaohao/yezihaohao.github.io/master/imgs/rd1.gif)


### 代码目录
```js
+-- build/                                  ---打包的文件目录
+-- config/                                 ---npm run eject 后的配置文件目录
+-- node_modules/                           ---npm下载文件目录
+-- public/                                 
|   --- index.html							---首页入口html文件
|   --- npm.json							---echarts测试数据
|   --- weibo.json							---echarts测试数据
+-- src/                                    ---核心代码目录
|   +-- axios                               ---http请求存放目录
|   |    --- index.js
|   +-- components                          ---各式各样的组件存放目录
|   |    +-- animation                      ---动画组件
|   |    |    --- ...   
|   |    +-- charts                         ---图表组件
|   |    |    --- ...   
|   |    +-- dashboard                      ---首页组件
|   |    |    --- ...   
|   |    +-- forms                          ---表单组件
|   |    |    --- ...   
|   |    +-- pages                          ---页面组件
|   |    |    --- ...   
|   |    +-- tables                         ---表格组件
|   |    |    --- ...   
|   |    +-- ui                             ---ui组件
|   |    |    --- ...   
|   |    --- BreadcrumbCustom.jsx           ---面包屑组件
|   |    --- HeaderCustom.jsx               ---顶部导航组件
|   |    --- Page.jsx                       ---页面容器
|   |    --- SiderCustom.jsx                ---左边菜单组件
|   +-- style                               ---项目的样式存放目录，主要采用less编写
|   +-- utils                               ---工具文件存放目录
|   --- App.js                              ---组件入口文件
|   --- index.js                            ---项目的整体js入口文件，包括路由配置等
--- .env                                    ---启动项目自定义端口配置文件
--- .eslintrc                               ---自定义eslint配置文件，包括增加的react jsx语法限制
--- package.json                                    

