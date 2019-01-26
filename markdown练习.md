# Node.js第一天

## 上午总结

+ Node.js是什么
  + JavaScript运行时的环境
  + 既不是语言，也不是框架，它是一个平台

+ Node.js中的 Javascript
  + 没有BOM、DOM
  + EcmaScript 基本的 JavaScript 语言部分
  + 在 Node 中为 JavaScript 提供了一些服务器级别的 API
    + 文件操作的能力
    + http服务的能力

## 总结

- Node 中的JavaScript 

  + EcmaScript

    + 变量
    + 方法
    + 数据类型
    + 内置对象
    + Array
    + Object
    + Date
    + Math

  + 模块系统

    1. 在 Node 中没有全局作用域的概念
    2. 在 Node 中，只能通过 require 方法来加载执行多个 JavaScript 脚本文件
    3. require 加载只能是执行其中的代码，文件与文件之间由于是模块作用域，所以不会有污染的问题
       1. 模块完全是封闭的
       2. 外部无法访问内部
       3. 内部也无法访问外部
    4. 模块作用域固然带来了一些好处，可以加载执行多个文件，可以完全避免变量命名冲突污染的问题
    5. 但是某些情况下，模块与模块是需要进行通信的
    6. 在每个模块中，都提供了一个对象：`exports`
    7. 该对象默认是一个空对象

  + 核心模块

    ​     核心模块是由 Node 提供的一个个的具名的模块，它们都有自己特殊的名称标识，例如

    ```javascript
    fun main(args: Array<String>) {
       println("Hello World!")
    
       println("sum = ${sum(34, 67)}")
       println("sum = ${sum(34, 67)}")
       println("sum = ${sum(34, 6, 57, 34)}")
    
       printSum(237, 57)
       printSum(234, 567, 8)
       vars(1, 4, 6, 78, 0, 6, 9, 8)
    
    
       val sumLambda: (Int, Int) -> Int = { x, y -> x + y }
       println("sumLambda = ${sumLambda(3, 6)}")
    ```

*通过网络发送文件*

**Node 中的其它的核心模块**

_做一个小管理系统：_

***

---

========











