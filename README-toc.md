
# [What Is Software Architecture ?](WhatIs.md)

# [Architect (架构师)](Architect/README.md)

# Architecture Framework
## [TOGAF](TOGAF/README.md)

# Architecture Style
## 1
### [C/S](CS/README.md)
### B/S

## 2
### [Layered](../Layered/README.md)
### [Event Driven (事件驱动架构，EDA)](../arch-event-driven/README.md)
### [Micro-Kernel](microkernel/README.md)
### [Cloud Native](cloud-native/README.md)

## 3
### [Distributed](KS-Distributed/README.md)
### [SOA](KS-SOA/README.md)
### [Micro-Service](KS-MicroService/README.md)
### [Decentralized](0_arch-style/decentralized/README.md)
### [Serverless](0_arch-style/serverless/README.md)

## 4
### [中台](KS-Arch-MiddleGround/README.md)

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

## DDD
### CQRS
### EventSourcing

# [High Availability Architectures](Arch_HA/README.md)

# [Architecture Design Practice](Arch-Design/README.md)

# References
* [O'Reilly《Software Architecture Patterns》]()

* [互联网公司架构演进之路汇总](https://www.jianshu.com/p/49ddf2f5c165)
* [Book Reading Note](https://github.com/SunnnyChan/sc.ebooks/tree/master/arch)
