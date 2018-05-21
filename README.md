## build-react-cli
##### build-react-cli是帮助你快速创建生成react项目的脚手架工具，配置了多种可选择的不同类型项目模版。
![Demonstration](https://github.com/Hzy0913/hanlibrary/blob/master/Demonstration.gif "Demonstration")
### Installation

```
npm install -g build-react
```
### Usage
```
build-react init my-react
```
**tip：** 初始化项目是第一项选择项目模版提供三种类型。
1. `init`为通用项目模版，配置了常用的react工具。
2. `complete-project`为完整的react项目，包括请求工具，服务转发，登录注册，复杂嵌套路由。
3. `simple-project`为简单项目模版，提供了react以及react-router基本配置。
##### 初始化项目完成以后
```
cd my-react //进入项目目录
npm install //安装项目依赖
npm start //运行项目
```
### command
###### 启动项目
`npm start` 或者 `npm run dev`
###### 启动项目后自动打开浏览器(传入 --o 参数)
`npm start --o` 或者`npm start --open`
###### 打包项目
`npm run build`
###### 打包项目并查看分析项目大小
`npm run build --a`
### config
`config`目录下的`index.js`文件为项目webpack配置文件，包括有运行端口、地址、本地服务代理配置等一系列配置。

| 名称  | 类型  | 描述  |
| ------------ | ------------ | ------------ |
|  host |String   |  主机 |
| port  | Number  | 端口  |
| proxyTable  | Object  | 代理配置  |
| useEslint  | Boolean  | 是否使用eslint  |
| autoOpenBrowser  | Boolean  | 是否自动打开浏览器  |
| errorOverlay  | Boolean  | 是否使用全屏报错提示  |
|  notifyOnErrors | Boolean  | 是否使用消息通知  |
| showEslintErrorsInOverlay  | Boolean  | 是否使用eslint全屏报错提示  |
| bundleAnalyzerReport  | Boolean  | 是否使用打包编译完成后显示依赖分析  |
