# Software Architecture

## 什么是架构？  

Wikipedia:
Architecture is both the process and the product of planning, designing,   
and constructing buildings or any other structures.   
The term architecture is also used metaphorically to refer to   
the design of organizations and other abstract concepts.  

架构就是对系统中的实体以及实体之间的关系所进行的抽象描述。  
架构始于建筑，是因为人类发展（原始人自给自足住在树上，也就不需要架构）分工协作的需要，  
将目标系统按某个原则进行切分，切分的原则，是要便于不同的角色进行并行工作。  

百度百科：  
是有关软件整体结构与组件的抽象描述，用于指导大型软件系统各个方面的设计。  

* 架构=要素+结构+连接  

* * 架构要素可以是子系统、模块、应用服务  
* * 结构，是架构的产物  
不同的软件系统会有不同的结构，这些结构是为解决不同场景而设计的。  
* * 连接，通过定义架构元素之间的接口和交互关系、集成机制，实现架构元素之间的连接。  
连接可以是分布式调用、进程间调用、组件之间的交互关系等。  

## 为什么需架构  

《系统架构：复杂系统的产品设计与开发》: **结构良好的创造活动要优于毫无结构的创造活动**  

## 什么是软件架构？
软件架构是一个系统的草图
    软件架构描述的对象是直接构成系统的抽象组件，各个组件之间的连接则明确和相对细致地描述组件之间的通信。

软件架构为软件系统提供了一个结构、行为和属性的高级抽象。
    由构件的描述、构件的相互作用、指导构件集成的模式以及这些模式的约束组成。

软件架构的核心价值应该只围绕一个核心命题：控制复杂性。
    他并不意味着某个特定的分层结构，某个特定的方法论（贫血、DDD等）。

架构的本质就是对系统进行有序化重构，不断减少系统的“熵”，使系统不断进化。


## Reference
![应用架构之道：分离业务逻辑和技术细节](https://blog.csdn.net/significantfrank/article/details/94593620)

