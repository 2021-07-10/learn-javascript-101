# 第 3.10 章 函数是一等公民

|本期版本|上期版本
|:---:|:---:
`Tue Aug 23 20:35:38 CST 2022` | -


```javascript
function fn(callback) {
  const a = 20
  return callback(20, 30) + a
}

function add(a, b) {
  return a + b
}

fn(add)
```