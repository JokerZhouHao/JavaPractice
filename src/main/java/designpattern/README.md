### 《Head First 设计模式》
---
ch1　[策略模式](./ch01strategy/duck)

> 设计原则
1. 封装变化
2. 少用继承，多用组合，个人理解继承就是拿刀水平砍竹子，覆盖面广，而组合是指定某些竹子砍，虽然覆盖面小，但是针对性强，便于需求变化后，对结构进行调整
3. 针对接口编程，不针对实现编程

> 策略模式

定义算法族，分别封装起来，让它们之间可以互相替换，此模式让算法的变换独立于使用算法的客户。个人理解就是把经常变化的部分提取出来，一一封装，变化的这部分功能，通过组合的方式来实现，这样当需求变化时，只需要调整封装类的实现，或者修改组合方式即可。


ch2　[观察者模式](./ch02Observer/subject)
> 设计原则

1. 封装变化
2. 少用继承，多用组合
3. 面向接口编程，而不是面向实现编程
4. 使交互对象之间松耦合

> 观察者模式

在对象之间定义一对多依赖，这样当一个对象改变状态，依赖它的对象都会收到通知，并自动更新。

ch3 [装饰者模式](./designpattern/ch03decorator)
> 设计原则

1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，不针对实现编程
4. 使交互对象之间松耦合
5. 对扩展开放，对修改关闭

> 装饰者模式

动态地将责任附加到对象上。想要扩展功能，装饰者模式提供有别于继承的另一种选择。

ch4 [工厂模式](./designpattern/ch04factory)

所有的工厂都是用来封装对象的创建。

> 设计原则

1. 多用组合，少用继承
2. 针对接口编程，不针对实现编程
3. 为交互的对象的松耦合设计而努力
4. 类应该对扩展开放，对修改关闭
5. 依赖倒置，即依赖抽象，不要依赖具体类

> 静态（简单）工厂

利用静态方法定义一个简单的工程。缺点是不能通过继承来改变创建方法的行为。

> 工厂方法

定义一个创建对象的接口，但由子类决定要实例化的类是哪一个。工作方法让类的实例化推迟到子类。可以把代码从需要实例化的具体类中解耦。将其继承成子类，并实现工厂方法。使用的是继承，即把对象的创建委托给子类，子类实现工厂方法来创建对象。

> 抽象工厂

提供一个接口，用于创建相关或依赖对象的家族，而不需要明确指定具体类。使用对象组合，对象的创建被实现在工厂接口所暴露出的方法中。

ch5 [单例模式](./designpattern/ch05singleton)

> 设计原则

1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，不针对实现编程
4. 为交互对象之间的松耦合而努力
5. 类应该对扩展开放，对修改关闭
6. 依赖抽象，不要依赖具体类

> 单例模式

确保一个类只有一个实例，并提供全局访问点。


ch6 [命令模式](./designpattern/ch06command)

> 设计原则
1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，不针对实现编程
4. 交互对象之间松耦合
5. 类对扩展开放，对修改关闭
6. 依赖倒置，依赖抽象，而不是依赖具体类

> 命令模式

将请求封装成对象，这可以使用不同的请求，队列，或者日志请求来参数或其他对象。


ch7 适配器模式与外观模式

> 设计原则
1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，而不是实现
4. 交互对象之间松耦合
5. 对象对扩展开发，对修改关闭
6. 依赖倒置，依赖抽象，而不是具体实现
7. 最少知识原则（墨忒尔法则）：只和你的密友谈话

> [适配器模式](./designpattern/ch07adapter)

将一个类的接口，转换成客户期望的另一个接口，适配器让原本不兼容的类可以无间合作。

> [外观模式](./designpattern/ch07facade)

提供了一个统一的接口，用来访问子系统中的一群接口。外观定义了一个高层接口，让子系统更容易使用。

ch8 [模板方法模式](./designpattern/ch08template)

> 设计原则
1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，而不是实现
4. 交互对象之间松耦合
5. 开闭原则：对扩展开放，对修改关闭
6. 依赖倒置：依赖抽象，而不是具体类
7. 最少知识原则（墨忒尔法则）：只和密友说话
8. 好莱坞原则：别找我，我会去找你

> 模板方法模式

在一个方法中定义算法的骨架，而将一些步骤延迟到子类中。模板方法使得子类可以在不改变算法结构的情况下重新定义算法中的某些步骤。

ch9 迭代模式与组合模式

> 设计原则

1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，而不是面向实现
4. 交互对象之间松耦合
5. 开闭原则：对扩展开放，对修改关闭
6. 依赖倒置：依赖抽象，而不是依赖实现
7. 最少知识原则：只和最亲密的人接触
8. 好莱坞原则：你别联系我，我会联系你
9. 类应该只有一个改变的理由

> [迭代器模式](./designpattern/ch09iterator)

提供一种方法顺序访问一个聚合对象中的各个元素，而不暴露其内部的表示。

> [组合模式](./designpattern/ch09Composite)

允许将对象组成树形结构来表现“整体/部分"的层次结构。组合能让客户以一致的方式处理个别对象和对象组合。

组合模式以单一责任设计原则换取透明性（transparency）。什么是透明性？通过组件的接口同时包含一些管理子节点和叶节点的操作，客户就可以将组合和叶节点一视同任。也就是说，一个元素究竟组合还是叶节点。对客户是透明的。


ch10 [状态模式](./designpattern/ch10state)

> 设计原则
1. 封装变化
2. 多用组合，少用继承
3. 针对接口编程，而不是实现
4. 交互对象之间松耦合
5. 开闭原则：对扩展开放，对修改关闭
6. 依赖倒置：依赖抽象，而不是实现
7. 最少知识原则：只和密友交谈
8. 好莱坞原则：别来找我，我会找你
9. 类应该只有一个改变的理由

> 状态模式

允许对象在改变内部状态时改变它的行为，对象看起来好像是修改了它的类。