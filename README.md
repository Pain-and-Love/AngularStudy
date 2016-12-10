# Angular入门

## 推荐工具

- 前端框架大全
	+ [查看框架使用趋势](www.awesomes.cn)
	+ [百度CDN](cdn.code.baidu)
## Angular简介

### 什么是AngularJS

- 它可以用来轻松构建 SPA (单一页面应用)
- 单一页面应用程序:
	+ 只有一个页面(整个应用的一个载体)
	+ 内容全部是由Ajax方式呈现出来的

### 为什么使用Angular

- 用更少的代码,实现更多的功能

### Angular特点

- MVC
- 模块化
- 自动化双向数据绑定
	+ ng-model 是双向数据绑定指令,效果是将当前元素的value属性和模型中的xxx建立绑定关系
	+ 对应ng-model,在对应module的controller中使用$scope来创建数据模型中的xxx
- 指令系统
	+ 最重要的概念是ng-XXX (指令) , 比如:ng-app就规定了angular的管理范围,ng-controller就规定了哪一个控制器来管理
 	+ $scope.$watch()
### 使用总结

- Angular最大程度减少了页面上的DOM操作
- 让JS中更专注业务逻辑的代码
- 通过简单的指令结合页面结构与逻辑数据
- <font color=red>解放了传统js中频繁的DOM操作</font>