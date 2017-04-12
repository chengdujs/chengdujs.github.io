---
title: CD-IT-JOB 第02迭代总结
date: 2017-04-06 22:33:12
type: "categories"
categories: 开源消息
---
### 介绍

原计划CD-IT-JOB 第二个迭代开发时间为：2017.02.15 - 02.26，于02.26晚20:00在成都前端交流群（206731784）中模拟给客户交付场景演示，但是因为种种原因，没有得以演示，现在以文本的形式做一总结，以备忘。

### 任务列表

- 【求职】搜索结果列表页面展现
  - 用户期望一个完整的搜索过程，达到能够顺利投递简历的过程。
  ![](https://striker.teambition.net/thumbnail/110p05b30f8015ff5d20668841c93238d531/w/600/h/1068)
- 【招聘】招聘列表
  - 作为HR能够方便的管理已发布的职业和已下线的职位列表。
  - 前置条件：从HR个人中心：职业管理中进入。
  ![](https://striker.teambition.net/thumbnail/110pe94ebd3f72494fd7edefba6ee8e0e9d6/w/600/h/1068)
- 【招聘】企业HR的个人中心
  - 做为企业HR有一个方便管理自己职位、公司信息、资质等等信息的地方。
  - 与普通用户的个人中心相似，但互斥，一个人登录进来只有一个角色。
  ![](https://striker.teambition.net/thumbnail/110p83390d7c1180c9cb7ee2aa1e6b534dda/w/600/h/1068)
- 【招聘】公司信息添加页面
  ![](https://striker.teambition.net/thumbnail/110p4b7960d9d86155f8f4cad6ef8f7f54f8/w/600/h/1092)
- 【招聘】公司信息添加页面
  - 作为HR希望能够修改公司相关信息的页面。
  - 前置条件：
  - 从HR个人中心中进入。
  - 后置条件：
  - 保存之后返回HR个人中心。
  ![](https://striker.teambition.net/thumbnail/110p4b7960d9d86155f8f4cad6ef8f7f54f8/w/600/h/1092)
- 【个人中心】个人资料维护
  - 作为用户能够设置自己相关资料页面，包括昵称，性别等。
  - 前置条件为：个人中心-> 右上角 资料维护，
  - 点击保存之后返回个人中心。
  ![](https://striker.teambition.net/thumbnail/110pa3c7fbe422b43aad134fd0c74ad571c9/w/600/h/1068)
- 【个人中心】个人信息预览页面
  - 作为个人用户能够预览简历的页面。
  - 前置条件：
  - 个人中心 -> 简历菜单。
  - 点击修改简历进入修改简历的页面。
  ![](https://striker.teambition.net/thumbnail/110pb77b15acf3fca87ce7fe6d75f46081e9/w/600/h/1939)
- 【招聘】作为企业HR能够下线职位
  ![](https://striker.teambition.net/thumbnail/110p0e6cd9227fba5e050edd129305af62ac/w/600/h/1068)
- 【招聘】作为企业HR能够修改职位
  ![](https://striker.teambition.net/thumbnail/110pe22d08f2cf230845037fc821c7751735/w/600/h/1068)
- 【招聘】作为企业HR能够发布职位
  ![](https://striker.teambition.net/thumbnail/110p37ae0eb0a7cfd0631c98b1b858222964/w/600/h/1068)
- 【全局】input-line组件
- 【招聘】公司信息页面修改
  - 公司信息页面可以被修改。
  - 页面表单中有值，且可以被修改。
  ![](https://striker.teambition.net/thumbnail/110pcd17a1c6d1dbea087d83f7fde49ee2e5/w/600/h/1092)
- 【个人中心】收藏页面
  - 作为用户能够收藏比较中心的公司，能够在合适的机会进行投递。
  - 前置条件：
  - 企业详情页面有收藏按钮，点击提示收藏成功之后有入口。
  ![](https://striker.teambition.net/thumbnail/110p2d400bd35ab8e780227c1a81fa6a8f95/w/600/h/758)

完成的任务在线预览地址：[http://chengdujs.com/cd-it-job/](http://chengdujs.com/cd-it-job/)

### 个人总结

- Treasure小结

#### 优点
1. 认领的任务全部完成
2. 总体上符合项目需求
3. 在写组件的时候会考虑复用性
4. 语法、代码规法在这个版本中基本稳定，基本一次性过ESLint

#### 缺点
1. 没有细致的架构图导致组件结构不规范
2. 没有添加动画，过渡不够流畅
3. 因为一些组件需要与其他同学配合，因此一些细节没有实现
4. API接口目前仍然使用mock，还没做到自己调用服务器接口

#### 总结

这个迭代中，编写代码以及规范已经不是什么大问题，基本所有的需求都能够通过一定的手段实现（要求熟悉底层代码）。迭代中出现的主要问题在于
1. 架构层面：各个组件应该放在什么页面不清晰，路由调用逻辑还是不清楚。因此只能完成单个组件。
2. 数据交互层：目前使用的mock，没有真正使用服务器的接口，这部分逻辑是预留了接口的，但是没有对数据信息进行处理，想必实际开发中，这个应该是问题出现的重点地方
3. 美观层面：只是完成了组件的业务，以及基本的UI样式，没有添加过渡动画，显得很僵硬，应该在后续迭代中改进
4. 与其他同学沟通不是很理想，了解别人的组件只能通过看代码完成