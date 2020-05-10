**js**中**let**关键字，定义一条语句，声明一个具有**块生命周期的本地变量**，定义的时候可以初始化值，也可以不初始化。

## 使用let关键字
这是[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)的一段例子：
```

let x = 1;

if (x === 1) {
  let x = 2; // 这里定义的x只在这个定义块中有效（这里是只这个大括号内，出了大括号，还是原来的值）

  console.log(x);
  // expected output: 2
}

console.log(x);
// expected output: 1

```

## 不使用let关键字

作为比较，我们把上面例子中的let去掉

```

x = 1; // 这里没有let关键字，x作用域整个script，所以出来大括号，值已经被改变

if (x === 1) {
  x = 2; 

  console.log(x);
  // expected output: 2
}

console.log(x);
// expected output: 2

```

# Reference
MDN web docs [let](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)
