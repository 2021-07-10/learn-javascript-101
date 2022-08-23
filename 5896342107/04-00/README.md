# 第 4 章 面向对象

* 除了使用输出是否为 undefined 来判断属性是否还存在与对象中，还可以使用 in 操作符。

## 属性描述对象

* 我们可以通过 `Object.defineProperty` 来修改属性的描述对象
* 当我们想要同时设置多个属性的特性值时，需要使用 `Object.defineProperties`

**读取属性的描述对象**

* `Object.getOwnPropertyDescriptor` 方法读取某一个属性的特性值。