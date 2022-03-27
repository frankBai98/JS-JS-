# JS数据类型(浅析一)

* JavaScript 语言的每一个值，都属于某一种数据类型。JavaScript 的数据类型，共有八种。
1.  number 数值  
2.  string 字符串
3. boolean   布尔
 4. symbol 符号
5. Object 对象
 6. null   空
 7. undefined 空
 8. bigint 内置对象
## 一、字符串
1. 语法
* '你好'
* "你好" 
* `你好`

引号不属于字符串的一部分。

2. 转义写法，如果要在单引号字符串的内部，使用单引号，就必须在内部的单引号前面加上反斜杠，用来转义。双引号字符串内部使用双引号，也是如此。
```javascript
'Did she say \'Hello\'?'
// "Did she say 'Hello'?"

"Did she say \"Hello\"?"
// "Did she say "Hello"?"
```
* 用另一种写法表示你想要的东西
* \'表示'
* \"表示"
* \n表示换行
* \r表示回车
* \t表示tab 制表符
* \ \ 表示 \
* \uFFFF表示对应的Unicode字符
* \xFF表示前256个Unicode字符
* `多行字符串(反引号)

3. length 属性
* length属性返回字符串的长度，该属性也是无法改变的。

```javascript
var s = 'hello';
s.length // 5

s.length = 3;
s.length // 5

s.length = 7;
s.length // 5
```
4. Base64 转码


## 二、布尔值
1. 布尔值代表“真”和“假”两个状态。“真”用关键字true表示，“假”用关键字false表示。布尔值只有这两个值。

    下列运算符会返回布尔值：
* 否定运算： !value
* 相等运算： 1 == 2、1!=2、3 === 4、3!==4
* 比较运算： 1 > 2 、1 >= 2、3 < 4、3 <= 4 
2. 五个falsy值

falsy相当于false但又不是false的值，他们分别是
* undefined
* null
* 0
* NaN
* ''

注意''和'  '不一样
## 三、undefined和null

null与undefined都可以表示“空”，null表示"空值"，undefined表示"未定义"。将一个变量赋值为undefined或null，语法效果几乎没有本质区别。


* 条件一:如果一个变量声明了 ，但它没有赋值，那么默认值就是undefined，而不是null
* 条件二：如果一个函数，没有写return，那么默认 return undefined,而不是null
* 一般前端程序员习惯会把非对象的空值写为undefined,把对象的空值写为null(习惯)
## 四、类型转换

* number=> string

String(x);x + ''
* string=> number

Number(x);s-0

* X=> bool

Boolean(x);!!(x)

* X=> string

String(x);x.toString()







