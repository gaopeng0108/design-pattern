在工厂方法模式中，每一个具体的工厂可以创建一个具体的产品，但是有的时候，我们希望一个工厂具有创建多个产品的能力。
### 抽象工厂模式
抽象工厂模式提供一个创建一系列相关或相互依赖的接口，而无需指定具体的类。和工厂方法模式的区别在于，工厂方法模式针对的是同一个产品结构的对象创建，而抽象工厂方法模式则针对不同的产品结构

#### 优势
* 隔离了具体类的生成，使得客户并不知道什么被创建了
* 增加新的工厂和产品结构很方便
#### 劣势
* 在添加新的产品类时，难以扩展抽象工厂来产生新的产品类，因为对接口进行修改会造成需要对所有子类进行修改的情况，会带来非常多的不便
* 开闭原则的倾向性（增加新的工厂和产品族较容易，增加新的产品等级结构麻烦）