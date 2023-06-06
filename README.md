# 鱼皮 - 聚合搜索项目

> 作者：[程序员鱼皮](https://github.com/liyupi)

本项目为 [编程导航知识星球](https://yupi.icu) 的原创全栈项目，后端代码开源。

[加入星球](https://yupi.icu) 可获得该项目从 0 到 1 的完整视频教程 + 源码 + 笔记 + 答疑 + 简历写法。

![加入编程导航](./doc/加入编程导航.jpeg)



## 项目简介

[编程导航知识星球](https://yupi.icu/) 原创项目，基于 Vue 3 + Spring Boot + Elastic Stack 的一站式聚合搜索平台，也是简化版的企业级搜索中台。

对用户来说，使用该平台，可以在同一个页面集中搜索出不同来源、不同类型的内容，提升用户的检索效率和搜索体验。

对企业来说，当企业内部有多个项目的数据都存在搜索需求时，无需针对每个项目单独开发搜索功能，可以直接将各项目的数据源接入搜索中台，从而提升开发效率、降低系统维护成本。

聚合搜索页面 - 搜文章：

![](https://yupi-picture-1256524210.cos.ap-shanghai.myqcloud.com/1/1680425753446-db21e8a2-0fd2-496d-8539-b5e3c1f35758.png)

聚合搜索页面 - 搜图片：

![](https://yupi-picture-1256524210.cos.ap-shanghai.myqcloud.com/1/1680425525242-a6c69abb-1bae-489e-a509-6ddfda0d2c48-20230402170832730.png)

聚合搜索页面 - 搜用户：

![](https://yupi-picture-1256524210.cos.ap-shanghai.myqcloud.com/1/1680425678150-91c35525-a9d4-47e5-9c09-06548c84f7c4-20230402170853604.png)

Elastic Stack - Kibana 数据看板：

![](https://yupi-picture-1256524210.cos.ap-shanghai.myqcloud.com/1/1680425981611-18e62334-1243-4741-9013-124494249fcb.png)



项目架构图：

![](https://yupi-picture-1256524210.cos.ap-shanghai.myqcloud.com/1/image-20230402105911365.png)



此外，这个项目中还应用到了鱼皮提供的万用后端项目模板，熟练之后，**几分钟开发一个新功能 **真的轻轻松松！



### 项目特点

1）本项目选用 Vue 3 + Spring Boot 2.7 新版本实现，包含完整的前后端，从需求分析、技术选型、系统设计、前后端开发再到最后上线，整个项目的制作过程为 **全程直播** ！

2）项目选题新颖，不是电商、不是管理系统、不是博客论坛，而是企业架构层面的 **通用搜索能力** 的抽象，做完这个项目后，之后你自己在做任何业务系统时，都可以复用这次开发的搜索能力。

3）项目中会带大家学习和实战：多种数据爬虫方法、4 种数据同步方法、接口优化（ **运用了多种设计模式** ）、Elastic Stack（Elasticsearch 搜索引擎、Kibana 看板）、压力测试等一系列知识。

4）除了学做项目之外，鱼皮还在直播过程中聊到了不少知识点，帮助大家提升架构设计思维、学会对比方案、阅读文档的套路；所有 Bug 和问题均为直播解决，带大家提升自主排查问题、解决 Bug 的能力。（课程中鱼皮还演示了一小下 ChatGPT 的使用）

5）项目总耗时不长，主打的是 **快速带大家学习新技术并直接实践运用** ，并且鱼皮已经整理好了这个项目可以写在简历上的亮点，成为简历上的亮眼项目。



### 本项目适合的同学

本项目前后端都有，但更侧重后端，重点讲了几种数据抓取方式、使用几种设计模式来优化接口、Elasticsearch 搜索引擎从 0 到 1 的应用、4 种数据同步方式等。

如果你学习过后端开发技术（比如 Java Web），希望做一个区别于管理系统的、有亮点的、写在简历上加分的项目，并提升自己的编程和架构设计能力，那么非常欢迎来学习！

当然，如果你是前端，也可以通过这个项目学习到一些前端开发的小技巧（比如页面状态同步），但是最好学习过 Vue 或 React 等至少一门开发框架。



### 技术选型（全栈项目）

#### 前端

- Vue 3
- Ant Design Vue 组件库
- 页面状态同步



#### 后端

- Spring Boot 2.7 框架 + springboot-init 脚手架
- MySQL 数据库（8.x 版本）
- Elastic Stack
    - Elasticsearch 搜索引擎（重点）
    - Logstash 数据管道
    - Kibana 数据可视化
- 数据抓取（jsoup、HttpClient 爬虫）
    - 离线
    - 实时
- 设计模式
    - 门面模式
    - 适配器模式
    - 注册器模式
- 数据同步（4 种同步方式）
    - 定时
    - 双写
    - Logstash
    - Canal
- JMeter 压力测试



## 项目大纲

1. 项目介绍和计划
2. 需求分析
3. 技术选型、业务流程、系统架构介绍
4. 前端项目初始化
    1. 前端脚手架使用
    2. 框架、组件库、请求库整合
5. 后端项目初始化
    1. Spring Boot 万用模板介绍和使用

6. 前端聚合搜索页面开发
7. 前后端联调
8. 多数据源获取（包含几种爬虫方式的讲解和实践）
    1. JSoup 离线抓取
    2. HttpClient 实时抓取

9. 聚合搜索业务场景分析
10. 聚合搜索接口开发
    1. 门面模式讲解
    2. 性能测试

11. 搜索接口优化
    1. 统一标准
    2. 适配器模式
    3. 注册器模式

12. 前端搜索接口调用优化
13. 从 0 开始学习 Elastic Stack
    1. Elasticsearch 概念及倒排索引原理
    2. Elasticsearch / Kibana 安装
    3. Elasticsearch + Kibana Dev Tools 入门实践
    4. Elasticsearch 调用方式讲解

14. ES 搜索引擎实战
    1. 几种 Java 客户端操作方式讲解
    2. ES 标准开发流程实战
    3. 动静分离

15. 数据同步（4 种同步方式）
    1. 定时
    2. 双写
    3. Logstash
    4. Canal

16. Kibana 搭建看板
17. JMeter 接口性能测试
18. 项目扩展点



## 项目资料

[加入星球](https://yupi.icu) 可获得：

1. 完整视频教程
2. 视频教程大纲
3. 完整项目源码
4. 项目学习笔记
5. 本项目交流答疑
6. 本项目简历写法
7. 更多原创项目教程和学习专栏

![加入编程导航](./doc/加入编程导航.jpeg)


## 版权声明

请尊重原创！与其泄露资料、二次售卖，不如邀请他人加入星球得大额赏金：https://t.zsxq.com/0eP82UuaG
# Xsearch
