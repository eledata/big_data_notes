# Scala Object与Class

## 1. Object

object的特点是：

- 可以拥有属性和方法，且默认都是"static"类型，可以直接用object名直接调用属性和方法，不需要通过new出来的对象（也不支持）。
- object里的main函数式应用程序的入口。
- object和class有很多和class相同的地方，可以extends父类或Trait，但object不可以extends object，即object无法作为父类。

## 2. class

在scala中，类名可以和对象名为同一个名字，该对象称为该类的伴生对象，类和伴生对象可以相互访问他们的私有属性，但是他们必须在同一个源文件内。类只会被编译，不能直接被执行，类的申明和主构造器在一起被申明，在一个类中，主构造器只有一个所有必须在内部申明主构造器或者是其他申明主构造器的辅构造器，主构造器会执行类定义中的所有语句。scala对每个字段都会提供getter和setter方法，同时也可以显示的申明，但是针对val类型，只提供getter方法，默认情况下，字段为公有类型，可以在setter方法中增加限制条件来限定变量的变化范围，在scala中方法可以访问改类所有对象的私有字段


