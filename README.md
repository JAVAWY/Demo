# Demo
学生疫情填报系统 学生疫情填报系统 
开发环境：eclipse 和mysql 
主要内容： 
excel包下主要实现数据导出到excel文件中 
hiai.dao包下写入学生以及教职工等实体 
hiai.model包下声明各个实体的私有变量 
hiai.util包下实现数据库的连接以及各二级部门浏览所有信息 
hiai.view包下主要是登录界面，以及信息录入，修改，查询等 
mail包下实现定时发送QQ邮箱提醒填报信息代
代码规范：单一职责，一个类或者一个接口，最好只负责一项职责。 
开闭原则：一个软件实体如类、模版和函数应该对扩展，对修改关闭； 
里氏替换原则：子类可以实现父类的抽象方法，但不能覆盖父类的非抽象方法；
子类可以增加自己特有的方法；
当子类的方法重载父类的方法时，方法的形参要比父类方法的输入参数更佳宽松；
当子类的方法实现父类的抽象方法时，方法的返回值要比父类更加严格； 依赖倒置原则 低层模块尽量都要有抽象类或者接口，或者两者都有；
变量的声明类型尽量是抽象类或者接口；
使用继承时遵循里氏替换原则； 接口隔离原则
一个接口只服务于一个子模块或业务逻辑，服务定制；
通过业务逻辑压缩接口中的public方法，让接口看起来更加精悍；
已经被污染了的接口，尽量修改，如果变更风险太大，则用适配器模式进行转化；
根据具体的业务，深入了解逻辑，用心感知去控制设计思路； 迪米特原则 定义：一个对象应该对其他对象保持最少的了解，其核心精神就是：不和陌生人说话，通俗之意就是一个对象对自己需要耦合关联调用的类应该知道的少；这会导致类之间的耦合度降低，每个类都尽量减少对其他类的依赖。
