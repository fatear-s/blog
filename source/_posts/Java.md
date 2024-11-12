---
title: Java
---



# Java

## Point

容器

不能存基本数据类型，只能存引用数据类型和包装类

ArrayList

泛型<Type>



### static(修饰词)

变量：相同类型不同对象之间的数据共享

public static int a;

可以类名调用

内存：堆中，静态区

类内存分配（字节码到方法区）

![image-20241111121638273](/Users/liutao/Library/Application Support/typora-user-images/image-20241111121638273.png)

方法：

javabean类

描述一类事物

测试类

带有main方法，用于测试

工具类

帮助实现的工具，Math等（私有化构造方法）

工具类就使用static修饰词

static 注意事项

静态方法只能访问静态变量



### 继承

class Student extends Person{}

默认父类:Object()



子类能继承父类

构造方法不能继承

this.name 本类

super.name 父类

this,super 都符合就近原则，本类找不到就父类找，直到找到

成员变量

private 继承但不可直接使用

成员方法

虚方法表（非private，非static，非final）继承



内存分析工具

jps  查看类的ID

jhsdb 内存查看



重新，就是覆盖虚方发表中的方法。



父类构造方法

Super()父类无参构造，可以有参构造

this()本类构造方法

类的基本方法，ClassLayout.praseInstance(calss s )

### 多态

子类对象赋值给父类引用

继承关系

父类引用

方法重写

Person  p = new Student()

成员变量，与成员方法区别：

成员变量没有重写这一个说法，就近原则，而成员方法会调用子类重写的方法。

编译的时候看父类的声明，父类没有就报错

成员变量，编译看左边，运行看左边

成员方法，编译看左边，运行看右边

使用：

定义方法，传入参数是父类，就可以接受所有子类的传入



类型强制转换

(Student) p;

判断引用是不是某类型

引用 instanceof type

引用 instanceof type 引用1

