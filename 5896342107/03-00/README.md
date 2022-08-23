# 第 3 章 函数

|本期版本|上期版本
|:---:|:---:
`Tue Aug 23 18:26:25 CST 2022` | -


```javascript
Object.prototype.toString
    .call(value)
    .split(" ")[1]
    .slice(0, -1)
    .replace(/^[A-Z]{1}/, p => p.toLowerCase());
```


```javascript
toString.call(elem).replace(/[\[\]]/g, '').split(' ')[1].toLowerCase();
```