# 前端概述：技能

![前端图谱](/documents/assets/img/tech.jpeg)
[来源：笼统的前端](http://www.vichily.com/2017/02/28/%E7%AC%BC%E7%BB%9F%E7%9A%84%E5%89%8D%E7%AB%AF/)

# 前端概述：主要语言

---

1. HTML： 页面结构
2. CSS： 页面样式
3. JavaScript： 页面行为

# HTML

## HTML 是用来描述网页的一种语言。

- HTML 指的是超文本标记语言 (Hyper Text Markup Language)
- HTML 不是一种编程语言，而是一种标记语言 (markup language)
- 标记语言是一套标记标签 (markup tag)
- HTML 使用标记标签来描述网页

```html
<html>
  <body>
    <p>hello world</p>
  </body>
</html>
```

# CSS

## CSS(Cascading Stylesheet)用于设置页面样式。

```html
// 1. 外部样式表
<head>
  <link rel="stylesheet" type="text/css" href="style.css" />
</head>

// 2. 内部样式表
<head>
  <style type="text/css">
    p {
      margin: 10px;
    }
  </style>
</head>

// 3. 内嵌样式(可在动态效果中同 JavaScript 一同使用)
<p style="color: red">Sample Text</p>
```

# CSS 选择器

1. 简单选择器：标签、类、id、通配符、属性、伪类
2. 伪元素：first-letter、before、after
3. 组合选择器：后代、 子选择器、 兄弟选择器

```css
a:hover {
}
a:after {
}
div a {
} // 后代
div > a {
} // 子选择器
div ~ a {
} // 兄弟选择器
```

```html
<html>
  <head>
    <style>
      p {
        background-color: purple;
      }
      .hello {
        background-color: blue;
      }
      #hello {
        background-color: red;
      }
    </style>
  </head>
  <body>
    <p id="hello" class="hello">one, hello world</p>
    <p id="hello" style="background-color: green">two, hello world</p>
    <p class="hello">three, hello world</p>
  </body>
</html>
```

[效果展示](http://jsbin.com/sufucep/2/edit?html,output)

# CSS 选择器优先级

---

- 行内样式 == 1000
- id 选择器的数量 == 100
- 类、伪类的属性选择器的数量 == 10
- 标签选择器和伪元素选择器的数量 == 1

# JavaScript

![内容](/documents/assets/img/javascript-env.png)
[来源：JavaScript 介绍](http://chanshuyi.github.io/frontend_notebook/chapter2/01_javascript_intro.html)

# JavaScript: 数据类型

---

1. 字符串（String）
2. 数字（Number）
3. 布尔值（Boolean）
4. Null
5. Undefined
6. 数组（Array）
7. 对象（Object）

# JavaScript: 变量声明

1. var、 let、 const
2. 字面量 or 构造函数

```js
var a = []
var b = new Array()
```

# JavaScript: 作用域

1. 局部作用域
2. 全局作用域

```js
var foo = 'foo'
var x = 'foobar'
function bar() {
  var foo = 'bar'
  console.log(foo, x) // bar, foobar
}
bar()
console.log(foo, x) // foo, foobar
```

# JavaScript: 作用域经典问题

```js
var arry = []
for (var i = 0; i < 5; i++) {
  arry[i] = function () {
    console.log(i)
  }
}
arry.forEach(function (func, idx) {
  console.log('arry[' + idx + ']执行结果:')
  func()
})
// 预期结果是 0, 1, 2, 3, 4
// 实际结果是 5, 5, 5, 5, 5
```

# JavaScript: 作用域经典问题

```js
var arry = []
var wrapper = function (i) {
  return function () {
    console.log(i)
  }
}
for (var i = 0; i < 5; i++) {
  arry[i] = wrapper(i)
}
arry.forEach(function (func, idx) {
  console.log('arry[' + idx + ']执行结果:')
  func()
})
```

# JavaScript: 闭包

1. 函数内部可以引用函数外部的变量
2. 前提：

- 函数是一等公民，可以当做参数传递也可以当做返回值
- 如果变量被引用，即使函数结束变量也不会被清空

# JavaScript: 闭包作用

---

1. 模拟私有方法

```js
var Person = (function() {
    var age;
    var name;
    return {
        setAge: function(nAge) {age = nAge},
        getAge: function () {return age};
    }
})(); // 立即执行函数
```

2. 实现单例模式

```js
// 传入一个构造函数，只生成一个实例
var Singleton = function (ConstructFunc) {
  var instance
  return function () {
    if (!instance) {
      instance = new ConstructFunc()
    }
    return instance
  }
}
```

# JavaScript: 函数

---

1. 普通函数
2. 对象属性
3. 匿名函数
4. 构造函数

# JavaScript: 原型

```js
var Person = function () {}
Person.prototype.type = 'Person'
Person.prototype.maxAge = 100

var p = new Person()
console.log(p.maxAge)
p.name = 'rainy'
```

# JavaScript: 原型链

![prototype](http://7xiijd.com1.z0.glb.clouddn.com/js-proto.jpg)
[来源:图解 Javascript 原型链](http://blog.rainy.im/2015/07/20/prototype-chain-in-js/)

# JavaScript: 原型链

- 原型和原型链是 JS 实现继承的一种模型。
- 原型链的形成是真正是靠`__proto__` 而非`prototype`

# DOM

![dom tree](/documents/assets/img/dom-tree.jpg)

# DOM 事件模型

1. 捕获阶段
2. 冒泡阶段

# DOM 事件示例

```js
// 以按钮的点击事件为例
var btnId = '#btn' // 需要点击按钮的ID
var handler = function () {
  alert('you click me')
} //点击事件处理函数
// 使用jquery
$(btnId).on('click', handler)
$(bntId).off() // 解绑事件

// 不使用jquery
// 元素属性方式
var btn = document.querySelector(btnId)
btn.onclick = handler // 绑定
btn.onclick = null // 解绑

// 注册事件
btn.addEventListener('click', handler)
btn.removeEventListener('click', handler)
```

# JavaScript 运行机制简介

![event loop](/documents/assets/img/event-loop.jpg)

# Thanks

Q&A

# 参考

1. [Web 前端发展简史](https://wenku.baidu.com/view/35f72bc1cf84b9d529ea7a7f.html)
2. [w3school](http://www.w3school.com.cn/h.asp)
3. [笼统的前端](http://www.vichily.com/2017/02/28/%E7%AC%BC%E7%BB%9F%E7%9A%84%E5%89%8D%E7%AB%AF/)
4. [前端开发笔记本](http://chanshuyi.github.io/frontend_notebook/index.html)
5. [JavaScript 介绍](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Guide/Introduction)
6. [ECMAScript 和 JavaScript 的关系](http://es6.ruanyifeng.com/#docs/intro#ECMAScript-和-JavaScript-的关系)
7. [来源:图解 Javascript 原型链](http://blog.rainy.im/2015/07/20/prototype-chain-in-js/)
8. [avaScript 运行机制详解：再谈 Event Loop](http://www.ruanyifeng.com/blog/2014/10/event-loop.html)

# 拓展阅读

1. [First-class function](https://en.wikipedia.org/wiki/First-class_function)
2. [Null prototype, Object.prototype and Object.create](http://stackoverflow.com/a/18198310)
3. [闭包](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Closures)
