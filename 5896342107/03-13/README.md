# 第 3.13 章 科里化

|本期版本|上期版本
|:---:|:---:
`Tue Aug 23 15:28:49 CST 2022` | -

* 柯里化是指这样一个函数(假设叫做createCurry)，他接收函数A作为参数，运行后能够返回一个新的函数。并且这个新的函数能够处理函数A的剩余参数。