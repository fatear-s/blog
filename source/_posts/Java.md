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

成员变量

private 继承但不可直接使用

成员方法

虚方法表（非private，非static，非final）

内存分析工具

