# 系统分析与设计秋季学期大作业-前端
这是一个点餐系统，包含用户点餐、商家出餐、管理员管理三部分功能

## 使用的框架、插件等

* 用Vue-cli脚手架、vue-router、vuex
* 用element-ui样式框架
* 用axios发请求

## 包含的功能

* 手机注册，登录，重置密码
* 用户点餐，该商家会收到消息提示有新订单(用轮询实现)
* 用户查看自己的订单，评价、删除等
* 修改自己的信息，申请成为商户等
* 商家管理订单，接单等
* 统计商家订单数，评分等(页面上的月销量是总销量)
* 商家管理菜单、查看评论
* 管理员管理用户、商铺、分类等
* 搜索功能

## 目录结构

顶层就是vue-cli的结构，主要看前端src和后台server的结构

``` md
─ src
 ├── common                         #
 │  ├── audio                       #音频
 │  ├── images                      #图片
 │  ├── javascript                  #api接口、cache、config等js文件
 │  ├── style                       #公用style
 ├── components                     #组件
 ├── pages                          #页面，处理业务，主要分为三个模块
 │  ├── admin
 │  ├── seller
 │  ├── user
 │  ├── index.vue
 │  ├── login.vue
 ├── router                         #路由
 │  ├── index.js
 ├── store                          #vuex的store，分了三个模块
 │  ├── admin
 │  ├── seller
 │  ├── user
 │  ├── index.js
 ├── App.vue
 ├── main.js
```