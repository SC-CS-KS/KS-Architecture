
# [What Is Software Architecture ?](Architecture/WhatIs.md)

# [Architect (架构师)](Architect/README.md)

# 架构理论
## 一致性
## 康威定律

# 架构模型 Architecture Model
## [TOGAF](_Model/TOGAF/README.md)

# 架构风格 Architecture Style
## 1
### [C/S](e_Arch-Style/CS/README.md)
### B/S

## 2
### [Layered（分层架构）](e_Layered/README.md)
### [Event Driven (事件驱动架构，EDA)](e_Event-Driven/README.md)
### [Micro-Kernel（微内核架构）](e_Arch-Style/Microkernel/README.md)
### [Cloud Native（云原生架构）](e_Cloud-Native/README.md)

## 3
### [Distributed（分布式）](e_Distributed/README.md)
### [SOA（面向服务）](e_SOA/README.md)
### [Micro-Service（微服务）](e_MicroService/README.md)
### [Decentralized（去中心化）](e_Arch-Style/Decentralized/README.md)
### [Serverless（无服务器）](e_Arch-Style/Serverless/README.md)

## 4
### [中台](f_MiddleGround/README.md)

## 5
### 主从模式（Master-Slave Pattern）
### 管道-过滤器模式（Pipe-Filter Pattern）
```md
用于构造生成和处理数据流的系统。每个处理步骤都包含一个过滤器组件。
要处理的数据通过管道传递。这些管道可用于缓冲或同步目的。
```
```md
应用场景：
编译器。连续过滤器执行词法分析、词法解析、语义分析和代码生成。
生物信息学的工作流
工具链式的应用程序
```
### 代理模式（Broker Pattern）
```md
这种模式通过解耦组件来构造分布式系统。
```
### 点对点模式（Peer-to-Peer Pattern）
### 事件-总线模式（Event-Bus Pattern）
### 黑板模式（Blackboard Pattern）
```md
这种模式对于没有确定解决方案策略的问题非常有用。
```
### 解释器模式（Interpreter Pattern）
```md
模式用于设计一个解释专用语言编写的程序组件。
```

# [架构设计实践](_design/README.md)

# [高可用架构]](https://github.com/SC-CS-KS/KS-HA)

# [产品架构](_ProductArch/README.md)

# References
* [O'Reilly《Software Architecture Patterns》]()

* [互联网公司架构演进之路汇总](https://www.jianshu.com/p/49ddf2f5c165)
* [Book Reading Note](https://github.com/SunnnyChan/sc.ebooks/tree/master/arch)
