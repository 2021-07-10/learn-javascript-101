# 第 3.12 章 高阶函数

|本期版本|上期版本
|:---:|:---:
`Tue Aug 23 15:24:34 CST 2022` | -


* 高阶函数，就是让当前函数获得额外能力的函数。
* 如果简单粗暴一点的理解，凡是接收一个函数作为参数的函数，都是高阶函数
* 在封装函数时，一个不确定的变量，我们可以往函数中传入`参数`的方式来指定它
* 个不确定的处理过程，我们可以往函数中传入另外一个`函数`的方式来自定义这个处理过程
* 高阶函数的使用思路正是在于此，他其实是一个封装公共逻辑的过程