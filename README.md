# seat-select (vue移动端座位选择)
> if this project is useful to you :D , Please star this project~
>
> 如果这个项目对你有帮助 :D 请点个star吧~

> [点击这里demo预览](https://zenghao0219.github.io/seat-select-demo/ "请使用手机访问")
>
> 此次项目是基于vue编写的类似淘票票和猫眼的电影`移动端`锁座页面,经过超过百个影厅的测试,其中包含功能
>
> - 座位图生成
> - 座位预览图生成
> - 座位`留空`检测
> - 座位智能选择`最优座位`算法
> - 自适应影厅大小
> - 座位图左侧导航栏的过道检测
> - 普通座位的选择逻辑
> - 情侣座位的选择逻辑
#### 项目截图

<img src="https://www.xollipop.top/demo.jpg" width="200" hegiht="300"/>

#### 之后的计划

- 文档补全,功能实现解析
- 后台控制端,可以编辑座位图提供接口生成座位图JSON
### README导航

[座位JSON结构解析](https://github.com/zenghao0219/seat-select/tree/master/public/mock)

#### 智能选座示例
```
以下为多个影厅的智能选座gif图演示
```
<img src="https://www.xollipop.top/soogif1.gif" width="200" hegiht="300"/>

<img src="https://www.xollipop.top/soogif2.gif" width="200" hegiht="300"/>

<img src="https://www.xollipop.top/soogif3.gif" width="200" hegiht="300"/>

#### 智能选座示例
```
以下为空位检测逻辑gif图演示
```
<img src="https://www.xollipop.top/soogif4.gif" width="200" hegiht="300"/>

### 项目依赖组件

该项目引用到的外部常用组件

> [amfe-flexible](https://github.com/amfe/lib-flexible "阿里巴巴弹性rem布局")
>
> [vue-touch](https://github.com/vuejs/vue-touch "vue-touch")
>
> [better-scroll](https://github.com/ustbhuangyi/better-scroll "better-scroll")

### 目录结构
```
.public
├── index.html
└── mock
    └── seatLove.json(mock数据在这里)

.src
├── App.vue --(入口组件)
├── assets --(静态文件)
│   ├── images
│   │   └── loading.gif --(加载图片)
│   └── stylus
│       ├── golbal.styl --(全局styl)
│       └── reset.styl --(移动端重写CSS)
├── components --(公用组件)
│   ├── Header.vue --(头部公用组件)
│   └── loading.vue --(载入公用组件)
├── http.js (axios工具类)
├── main.js (vue入口js)
├── pages --(组件目录)
│   └── hallseat
│       ├── HallSeat.vue --(选座父组件)
│       └── component --(选座子组件目录)
│           ├── ConfirmLock.vue --(确认选择组件)
│           ├── PlanDetail.vue --(电影信息组件)
│           ├── QuickSelectTab.vue --(智能选座组件)
│           ├── SeatArea.vue --(座位图生成组件)
│           └── SelectedTab.vue --(已选座展示组件)
└── router.js
```
### 初始化项目 (Project setup)
```
npm install
```

### 直接运行开发环境 (Compiles and hot-reloads for development)
```
npm run serve
```

### 项目打包 (Compiles and minifies for production)
```
npm run build
```
### 讨论

欢迎加群讨论: 3544395

### 项目捐赠
写代码不易...请作者喝杯咖啡呗?

<img src="https://www.xollipop.top/code.png" width="200" hegiht="300"/>

(PS: 支付的时候 请带上你的名字/昵称呀 会维护一个赞助列表~ )
