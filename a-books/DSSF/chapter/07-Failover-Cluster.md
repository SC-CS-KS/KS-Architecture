# 集群容错

集群服务调用失败后，服务框架需要能够在底层容错。  

## 集群容错场景
### 通信链路故障

指的是消费者和服务提供者之间的链路（通常为长连接）故障。

### 服务端超时
### 服务端调用失败

## 容错策略  

### 失败自动切换（Failover）

通常应用于幂等性服务。
失败重试会增加服务的调用时延。

### 失败通知（Failback）

不重试，直接将异常返回给消费者，由消费者进行后续处理。

### 失败缓存（Failcache）

是失败自动恢复的一种。

* 应用场景
服务有状态路由
对延时要求不高的服务
通知类服务

* 可靠性考虑
缓存时间、缓存对象上限
缓存淘汰算法的选择
定时重试的周期、重试最大次数等

### 快速失败（Failfast）

在业务高峰期，对于一些非核心业务，希望只调用一次，失败也不再重试，
为重要的核心业务节约宝贵的运行资源。此时，快速失败策略是一个不错的选择。

* 设计：
获取到服务调用异常后，直接忽略异常，记录异常日志。

### 容错策略扩展

以上策略不满足业务的实际场景时，提供容错策略接口，以支持用户自定义扩展容错策略。

