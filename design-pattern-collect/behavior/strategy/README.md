策略模式定义一系列算法，将每一个算法封装起来，并让它们可以互换，实现算法的变化独立于客户对象的变化。

#### 优势
* 策略模式提供了对开闭原则的完美支持，用户可以在不修改客户代码的情况下，选择相应的算法，并且可以灵活的增加新算法
* 策略模式提供了代替对象继承的方式（组合优于继承）

#### 劣势
* 客户端必须知道所有策略类，并选择合适的策略类
* 可以通过使用享元模式在一定程度上减少对象的数量
