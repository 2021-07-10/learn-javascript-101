|本期版本| 上期版本
|:---:|:---:
`Thu Jan 13 23:46:12 CST 2022` | -


# 第 6 章 面向对象的程序设计

## 6.1 立即对象



### 6.1.1 属性类型

* 数据属性: `[[Configurable]]`、`[[Enumerable]]`、`[[Writable]]`、`[[Value]]`
* 访问器属性: `[[Configurable]]`、`[[Enumerable]]`、`[[Get]]`、`[[Set]]`
* `Object.defineProperty()` / 默认值是 `false`
* 下划线是一种常用的记号，用于表示只能通过对象方法访问的属性

**6.1.2 定义多个属性**

* `Object.defineProperties()`

**6.1.3 读取属性的特性**

* `Object.getOwnPropertyDescriptor()`

## 6.2 创建对象


### 6.2.2 构造函数模式

* 按照惯例，构造函数始终都应以一个大写字母开头, 而非构造函数的则应该以一个小写字母开头
* 对象的 `constructor` 属性最初是用来标识对象的类型的。但是，提到检测对象类型，还是 `instanceof` 操作符要更可靠一些
* 任何函数，只要通过`new` 操作符调用，那它就可以作为构造函数

### 6.2.3 原型模式

* 每个函数都有一个 `prototype` 属性, 这个属性是一个指针，指向一个对象，而这个对象的用途是包含可以由特定类型的所有实例共享的属性和方法
* 在默认情况下，所有原型对象都自动获得一个 `constructor` 属性，这个属性是一个指向 `prototype` 属性所在函数的指针
* 原型对象默认只会取得 `constructor` 属性；至于其他方法，则都是从 `Object` 继承而来的。
* 实例内部将包含一个指针，指向构造函数的原型对象: `[[Prototype]]` / `__proto__`
* `Person.prototype.isPrototypeof()` / `Object.getPrototypeof()`
* 执行一次搜索: 对象实例、原型对象
* 当为对象实例添加一个属性时，这个属性会屏蔽原型对象中保存的同名属性
* `hasOwnProperty` 方法可以检测一个属性是存在于实例中，还是存在于原型中

**原型与in操作符**

* 在单独使用时，in操作符会在通过对象能够访问给定的属性时返回true，无论该属性存在于实例中还是原型中
* 在使用 for-in 循环时，返回的是所有能够通过对象访问的、可枚举的属性
* 所有开发人员定义的属性都是可枚举的
* `Object.keys()` / `Object.getOwnPropertyNames()`


### 6.2.4 组合使用构造函数模式和原型模式

* 构造函数模式用于定义实例属性，而原型模式用于定义方法和共享属性


## Ref

* [Javascript 的 this 用法](https://www.ruanyifeng.com/blog/2010/04/using_this_keyword_in_javascript.html)
* [JavaScript 的 this 原理](https://www.ruanyifeng.com/blog/2018/06/javascript-this.html)