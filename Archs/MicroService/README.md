# Micro-Service (MicroServices Architecture)

## [What Is](WhatIs.md)

## 实现
### 模式
* RESTful API 模式：服务通过 API 提供，云服务就属于这一类
* RESTful 应用模式：服务通过传统的网络协议或者应用协议提供，背后通常是一个多功能的应用程序，常见于企业内部
* 集中消息模式：采用消息代理（message broker），可以实现消息队列、负载均衡、统一日志和异常处理，缺点是会出现单点失败，消息代理可能要做成集群

### 组件
* [API Gateway](API-Gateway/README.md)

## 实践
* [网易云 - 轻舟微服务](https://www.163yun.com/product-nsf?fromnsf=baiduP_service_C190130P11)
* [iResty - 微服务 API 管理平台](https://www.iresty.com)

## References
* [基于Spring + SpringMVC + Mybatis 分布式敏捷开发系统架构](https://github.com/shuzheng/zheng)
```md
提供整套公共微服务服务模块：
集中权限管理（单点登录）、内容管理、支付中心、用户管理（支持第三方登录）、
微信平台、存储系统、配置中心、日志分析、任务和通知等，支持服务治理、监控和追踪。
```

* [MicroServices AntiPatterns and Pitfalls](https://github.com/SunnnyChan/SunnnyChan.github.io/blob/master/post/readme/reading/arch/Microservices-AntiPatterns-and-Pitfalls/README.md)

* [Awesome MicroServices](https://github.com/mfornos/awesome-microservices)

* [微服务架构起源、简介及设计](https://cloud.tencent.com/info/7360f254f288e24bdc1b3da89c686676.html)
* [微服务架构有毒，何时不使用微服务？](https://cloud.tencent.com/developer/news/369360)
