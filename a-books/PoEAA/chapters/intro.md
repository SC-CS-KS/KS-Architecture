# 引言
## 架构
* 什么是“架构”？
```md
1. 最高层次的系统分解
2. 系统中不易改变的决定
```
```md
Ralph Johnson 认为:
架构是一种主观上的东西，是专家级项目开发人员对系统设计的一些可共享的理解。
一般地，对可共享的理解表现为系统中主要的组成部分以及它们的交互关系。

架构还是一些决定，开发者们希望这些决定能尽早做出，因为在开发者看来它们是难以改变的。
架构的主观性也来源于此 —— 如果你发现某些决定并不像你想象的难以决定，那么它就不再与架构相关。
```
* 分层设计模式
```md
大多数重要的企业应用都是按照某种形式的层次分层设计的。层次方式是应用最广泛的设计方式。
```
## 企业应用
```md
1. 涉及数据持久化
2. 涉及大量数据
3. 涉及很多人同时访问数据
4. 涉及大量操作数据的用户界面屏幕
```
```md
企业应用很少独立存在，通常需要与散步在企业周围的其他企业应用集成。
风格迥异的系统有时候也是实现集成，即使统一了集成技术，也还会遇到业务过程中的差异以及数据中概念的不一致。
```
```md
业务逻辑带来的问题，
成千上万的“一次性特殊情况”，最终导致复杂的业务“无逻辑”，使得软件开发那么困难。
这种情况下必须将这些业务逻辑组织成有效的方式，因为可以确定的说，这些“逻辑”一定会随着时间不断变化。
```
* 大型系统与小型系统
```md
如果小型系统能够进行某些改善，那么一些这些改善措施成功运用到大型项目，带来的效果就会非常大。
实际上，最好通过简化架构和过程，将一个大型项目简化成小型项目。
```
## 企业应用种类
```md
企业应用是多样性的，不同的问题将导致不同的解决方法。
我认为设计中最具挑战性的地方就是了解有哪些候选的设计方法以及它们之间的优劣。
```
* B2C（Business to Customer）
```md
必须能应用大量客户，所以其解决方案必须考虑资源利用的有效性，系统的可伸缩性。
```
## 关于性能的考虑
```md
很多架构的设计决策和性能有关。有些架构上的决定对性能的影响，有可能是后期优化难以弥补的。
```
## 可伸缩性 
### 术语
* 响应时间
* 响应性 - 系统响应请求的速度有多快
* 等待时间
* 吞吐率
* 负载 - 系统当前负荷的表述
* 负载敏感度 - 响应时间随负载变化的情况
* 效率 - 性能除以资源
```md
可伸缩性度量的是向系统中增加资源对系统性能的影响。
一个可伸缩的系统，允许在增加了硬件资源后，系统能够有性能上的合理提升。

通常评价的指标为系统的容量，指最大有效负载或吞吐率。
```
* 垂直可伸缩（垂直延展）
```md
指提供单个服务器的性能，例如增加内存。
```
* 水平可伸缩（水平延展）
```md
通常指增加服务器数目。
```
* 总结
```md
当构建企业应用系统时，关注硬件的可伸缩性往往比关注容量和效率更重要。
```
## 模式
```md
每一个模式描述了一个在我们周围不断重复发生的问题以及该问题解决方案的核心。
这样，你就能一次又一次地使用该方案二不必做重复劳动。
```
```md
模式的核心就是特定的解决方案，它有效而且有足够的通用性，能解决重复出现的问题。
```
```md
模式的另一个视角是把它看成是一组建议，而创造模式的艺术是把很多建议分解开来，
形成相互独立的组，在此基础上可以相对独立的讨论它们。
```
```md
模式的关键点是它源于实践。
```
```md
模式的边界是模糊的，每个模式相对独立，但又不是彼此孤立的。
```
```md
模式能够帮助你更好的交流。
```
### 模式的结构

