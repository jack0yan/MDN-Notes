# Getter/Setter

`get`语法将对象属性绑定到查询该属性时将被调用的函数。

```javascript
var obj = {
  log: ['a', 'b', 'c'],
  get latest() {
    if (this.log.length == 0) {
      return undefined;
    }
    return this.log[this.log.length - 1];
  }
}

console.log(obj.latest);
// expected output: "c"

```

Getter/Setter是一个规定好参数和context的函数标准。

```javascript
let obj = {
  a:1,
  b:0
}
```

取a的值 `obj.a` 就是`getter` 设置a的值`obj.a=10` 就是`setter`

