# 第 3.11 章 纯函数

|本期版本|上期版本
|:---:|:---:
`Tue Aug 23 20:43:46 CST 2022` | -


## 纯函数的可缓存性

* 如果函数内部计算非常复杂，当我们发现输入与上一次相同时，可以直接返回结果而不用经过内部的计算。这是一种性能优化的策略。