### 责任链模式
责任链模式是一种行为设计模式，允许你将请求沿着处理者链进行发送。收到请求后，每个处理者都可以对请求进行处理，或将其传递给链上的其他处理者

#### 优势
* 单一职责原则，可以对发起操作和执行操作的类进行解耦
* 开闭原则，可以在增加新功能的情况下，不改变现有代码
* 可以控制请求处理顺序

#### 劣势
* 部分请求可能未被处理

#### 模式扩展
* 在这里每个处理者会持有下一个处理的引用，在坦克大战中有一个更骚的处理手段，那就是利用一个 linkedlist 来保存所有处理者。
* 客户端可以自行组装链，甚至可以像坦克大战一样根据配置或者环境来设置链
* 部分请求可能无法到达链尾，甚至到达链尾之后也不被处理
* 责任链模式、命令模式、中介者模式、观察者模式都是用于处理请求发送者和接受者之间不同的连接方式
  * 责任链按照顺序将请求动态传递给一系列的潜在接收者， 直至其中一名接收者对请求进行处理
  * 命令模式在请求者何接收者之间建立单向链接
  * 中介者模式清楚了请求者和接收者之间的链接，强制使用中介者进行
  * 观察者允许接受者动态地订阅或者取消接收请求
* 责任链模式通常和组合模式使用
* 责任链模式的管理者可以使用命令模式来实现
* 责任链模式和装饰者模式的类结构非常相似，但是责任链的管理者可以独立执行操作，还可以随时终止请求；装饰者则无法终止请求的传递