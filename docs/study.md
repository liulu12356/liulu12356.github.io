## 1、polymorphic（多态）

- 多态就是一个行为在不同的条件下，有不同的运行效果

## 2、抽象类

- 抽象类当我们不想封装一个具体的类的时候，所封装出来的类，之所以不想封装出来，是因为它的行为比较抽象，无法编写出具体的逻辑
- 用**abstract**修饰**class**里面可以有抽象的方法，也可以没有抽象方法（情况较少），里面有抽象方法，它就一定是抽象类
- 从用法上，主要是用来被继承的，它的子类必须要实现父类中的抽象方法，否则它自己也必须声明为abstract class

## 3、修饰符

- **final**

1. 基本类型：值不能改变
2. 引用类型：地址不能改变（但凡是new了，地址一定改变了，如果通过setter进行修改，地址没有改变）
3. 修饰类、方法：类不能被继承了，方法不能被重写了，但是构造器可以进行第一次赋值

- **static**

1. 修饰属性：全局公用（这个类的所有实例共有的），它不依赖于某一个实例而存在，类只要一加载就存在了
2. 修饰方法：静态方法只能引用静态属性（在引用非静态属性的时候，这个this没有指向）
3. 静态代码块：只执行一次，并且时间点在构造器之前，在静态属性初始化之后



## 4.接口

主要是用来封装一揽子抽象方法的，它侧重在于对行为的一种抽象（动词）

- 必须使用**implements**关键字
- 实现接口的类，必须要实现其中所有的抽象方法，只要有一个没有实现，这个类本身必须声明为**abstract class**
- 接口也可以定义属性，但是它默认是**public final static**接口中不能有具体的方法实现，它只是一种行为的规约（规范和约定）
- 接口可以说是抽象类抽象到极致的一种特殊情况
- 接口中其实可以定义具体方法（默认方法，可以定义多个），前面必须加**default**修饰


未完待续...............


