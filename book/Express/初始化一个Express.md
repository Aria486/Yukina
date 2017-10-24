# Express

Express 是一个简洁而灵活的 node.js Web应用框架, 提供了一系列强大特性帮助你创建各种 Web 应用，和丰富的 HTTP 工具。
使用 Express 可以快速地搭建一个完整功能的网站。
Express 框架核心特性：
* 可以设置中间件来响应 HTTP 请求。
* 定义了路由表用于执行不同的 HTTP 请求动作。
* 可以通过向模板传递参数来动态渲染 HTML 页面。


###  初始化一个Express项目

1.输入以下命令
```
expree --view=ejs myexpress
```
![如图](https://github.com/Aria486/Yukina/blob/master/img/expres.jpg)


2.目录结构说明  
<1>bin,存放启动项目的脚本文件   
<2>node_modules, 存放所有的项目依赖库   
<3>public，静态文件(css,js,img)   
<4>routes，路由文件(MVC中的C,controller)   
<5>views，页面文件(Ejs模板)   
<6>package.json，项目依赖配置及开发者信息 （类似于maven的pom）  
<7>app.js，应用核心配置文件   


3.运行 node index，打开浏览器访问 localhost:3000 时，页面应显示 hello, express

