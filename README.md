# iview admin 动态路由例子




* src/libs/util.js 里面加两个方法：backendMenusToRouters，backendMenuToRoute
* src/mock/data.js 里面加路由数据：routersData，模拟服务端获取
* src/mock/index.js这里暴露一个ajax调用接口：Mock.mock(/\/sys\/routers/, routersData)，记得引入一下:routersData
* src/api/routers.js 这里面的请求url改成/sys/routers,当然，你可以自己定义
* src/store/module/app.js ,添加对应的state,getter和actions,看代码。
* src/router/index.js 路由定义里，再route.onReady之后，加载动态路由
* view下面加点测试用的页面，参考pet目录下代码
* src/locale/lang/zh-CN.js 给菜单配一下i18n显示
---
启动：
* npm install
* npm run dev

