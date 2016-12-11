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
	+ angular中的表达式两对大括号 
- 指令系统
	+ 最重要的概念是ng-XXX (指令)
		- ng-app就规定了angular的管理范围,**尽可能一个页面只写一个**
		  ng-app在页面中找到了第一个ng-app之后,就不会再往下继续找了(或者用angular.bootstrap());
		  ng-app内部可以创建多个ng-app,并且可以同时使用(angular.module('myApp',["myApp1","myApp2"]))
		- ng-bind针对表达式的写法,提高了用户体验,但是遇到html标签的时候会直接输出,并不会解析
		  ng-bind-html 可以绑定html元素,但是需要引用一个angular-sanitize.min.js进行安全验证,**但是尽量还是别绑定html元素**
		- ng-repeat是很常用的一个指令,用来遍历一个**数组**然后重复创建当前元素,同时每个元素都会有$index $first $last $middle $even $odd $id值
		- ng-repeat 配合track by $index 使用,显示重复元素
		- ng-class设置一个key(class)-value(bool),ng-class会根据当前设置对象的属性和属性值来决定是否添加特定类名
		- ng-show和ng-hide 根据bool值来显示或者隐藏元素
		- ng-if 根据bool值来remove或者还原
		- ng-src和ng-href来代替原本的src和href
		- ng-readonly ng-disabled
		- ng-switch ng-switch-when ng-switch-default用来显示和隐藏多种选择
		- ng-checked和ng-selected 就只会做单向数据绑定,即**数据到view的同步**
		- ng-controller就规定了哪一个控制器来管理
 	+ $scope.$watch方法
### 使用总结

- **Angular最大程度减少了页面上的DOM操作**
- **让JS中更专注业务逻辑的代码**
- **通过简单的指令结合页面结构与逻辑数据**
- **解放了传统js中频繁的DOM操作**