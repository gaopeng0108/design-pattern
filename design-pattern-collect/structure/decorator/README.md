### 装饰者模式
动态地给对象增加一些额外的职责，就增加对象功能来说，装饰者模式比继承更加灵活。

#### 优势
* 与继承关系相比，关联关系的主要优势在于不会破坏类的封装性，而且继承一种耦合度较大的静态关系，无法在程序运行时动态扩展。
* 不需要用户创建更多的子类来扩展功能
* 具体构建类和装饰者类可以独立变化，符合开闭原则

#### 劣势
* 在进行系统设计时会产生很多小对象，这些对象以不同的方式排列组合，增加系统的复杂度
* 如果装饰的层级过多，在排查错误时会比较多困难

#### 模式应用
* IO 流
