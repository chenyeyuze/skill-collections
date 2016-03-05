#JavaScript编码风格
1. 基本的格式化  
1.1 缩进层级  
1.2 语句结尾和行长度  
1.3 换行和空行  
1.4 命名  
1.5 直接量 
2. 注释  
2.1 单行注释  
2.2 多行注释  
2.3 使用注释 
3. 语句和表达式  
3.1 花括号对齐方式  
3.2 块语句间隔  
3.3 switch语句  
3.4 with  
3.5 for-in
4. 变量、函数和运算符  
4.1 变量声明  
4.2 函数声明  
4.3 函数调用间隔  
4.4 相等  
4.5 eval()  
4.6 原始包装类型  
4.7 属性

-----

1 基本的格式化   

1.1 缩进层级  
  
> 一个tab代表缩进层级 

1.2 语句结尾和行长度  
  
> 语句结尾不可省略分号 
> 行长度建议是80/100个字符 

1.3 换行和空行  
   
> 逗号/冒号/小括号/当行注释符后面留一个空格  

```
// bad
function test(){
  console.log('test');
}

// good
function test() {
  console.log('test');
}

// bad
dog.set('attr',{
  age: '1 year',
  breed: 'Bernese Mountain Dog'
});

// good
dog.set('attr', {
  age: '1 year',
  breed: 'Bernese Mountain Dog'
});
```

> 在文件的最后留一个空行
> 在每一个代码块后留有一行

```
// bad
if (foo) {
  return bar;
}
return baz;

// good
if (foo) {
  return bar;
}

return baz;

// bad
var obj = {
  foo: function() {
  },
  bar: function() {
  }
};
return obj;

// good
var obj = {
  foo: function() {
  },

  bar: function() {
  }
};

return obj;

```
**对于有运算符的换行** 

> ,和&&等运算符在上一行，下一行需有两个层级的缩进  

```js
if (a === 0 &&
		bb === 1) {
	var bird = {
		name: 'wing',
		location: 'America',
		type: 'bird'
}

```

**对于方法之间的换行** 

* 在方法中的局部变量和第一条语句之间
* 在多行或单行注释之前
* 在方法内的逻辑片段之间插入空行，提高可读性  

1.4 命名  


* 变量和函数以驼峰式命名规则命名，变量命名为与上下文有关系的名称，不使用保留字
* 静态变量名称全部大写，使用下划线分隔单词
* 构造函数首字母大写
* 私有变量和方法以_开头
* this使用_this变量名代替
* 函数表达式也需要命名
* 参数多，传递hash对象，而不是一个一个的传递
* jQuery对象名称以$开头并且该缓存对象  

函数命名第一个单词为动词，比如

动词 | 含义
--------- | -------------
set | 保存值
get | 获取值 
is/has  | 是否存在
event | 事件处理
listen | 监听
load | 加载
do | 处理事件


```
var STATIC_VALUE = 'static',
    DYNAMIC_VALUE = 'dynamic',
    numbers = 0,
    userName = '',
    isFlag = false,
    items = [],
    bird = null;

// bad
function bird(){

}

// good
function Bird(){

}

// bad
var log = function(msg) {
  console.log(msg);
};

// good
var log = function log(msg) {
  console.log(msg);
};
```

1.5 直接量  

* 数字以十进制表示
* null的使用
> 用来初始化一个变量，这个变量可能赋值为一个对象
> 用来和一个已经初始化的变量比较，这个变量可以是也可以不是一个对象
> 当函数的参数期望是对象时，用作参数传入
> 当函数的返回值期望是对象时，用作返回值传出
> 不要使用null来检测是否传入了某个参数
> 不要用null来检测一个为初始化的变量
> 理解null最好的方式是将它当做对象的占位符

* 数组
数组初始化使用［］，不要使用new Array()
缓存数组长度
转换伪数组

```
var len = items.length,
      itemsCopy = [];
      
itemsCopy = items.slice();

function execute() {
      var args = [].slice.call(arguments);
}

```

2 注释  

2.1 单行注释  

* 独占一行的注释  
 用来解释下一行代码，这行注释之前总是有一个空行，且缩进层级和下一行代码保持一致
* 在代码行的尾部的注释  
 代码结束到注释之间至少有一个缩进。注释（包括之前的代码部分)不应当超过单行最大字符数限制，如果超过了，就将这条注释放置于当前代码行的上方
 单行注释不应该以连续多行注释的形式出现，除非你注释掉一大段代码  

2.2 多行注释  

多行注释以/\*开头，以\*/结束。其他行每一行前面以\*开头，\*后有一个空格，注释和代码之间没有空行间隔
和单行注释一样，多行注释之前应该有一个空行，且缩进层级和其他描述的代码保持一致

2.3 使用注释  

难于理解的代码
可能被误认为错误的代码
浏览器特性hack

2.4 文档注释  

jsDoc风格  

3 语句和表达式
  
3.1 花括号对齐方式  
块状语句都使用花括号
> if
> for
> while
> do ...while
> try catch finally

第一个花括号在第一句的末尾 

3.2 块语句间隔  

在左圆括号和右圆括号之后各添加一个空格

3.3 switch语句  


```
switch (condition) {
	case "A":
		break;
	case "B":
     break;
	//default 没有
｝

```
3.4 with  

禁止使用with

3.5 for-in  

遍历时使用hasOwnProperty判断,除非遍历原型属性

4 变量、函数和运算符  

4.1 变量声明  

var声明，禁止不使用var声明的变量，以防止全局变量污染
给出变量的初始值以确定变量类型
每个变量的声明以逗号结尾另起一行（参见1.4节）
数组声明使用普通数组，对象声明使用普通对象
一元运算符前后留有一个空格的距离
对变量赋值，要在一个作用域的顶部赋值，避免变量提升

```
// bad
function fly(){
	doSomething();
	var goods = new Array();
	var weapon = new Object();
	oil = 'none';
	var doSomething = function(){
		
	};	
}

// good
function fly(){
  var oil = 'none',
  		goods = [],
  		weapon = {};
	var doSomething = function(){
	
	};
	doSomething();
}
```
4.2 函数声明  

**在if/for循环中，不要使用函数声明，可以使用函数表达式**
一些浏览器可能的确可以在语句中使用函数声明。但是在解析方面的处理各不相同，各种浏览器下兼容性很不好。

```
// bad
if (currentUser){
  function test() {
    console.log('Nope.');
  }
}

// good
if (currentUser){
  var test = function test() {
    console.log('Yup.');
  }
}
```

4.3 函数调用间隔  

函数名和左括号之间没有间隔

```
// bad
doSomething (item);

// good
doSomething(item);
```

4.4 相等  

使用 === 和 !== 代替 == 和 !=
条件表达式 会通过 ToBoolean 来进行强制转化，而且遵循以下的规则：  

* 对象被转化为true
* Undefined被转化为false
* Null被转化为false
* 布尔值被转化为相应的布尔值
* 数字当值为+0,-0或NaN时转化为false，其他的转化为true
* Strings类型如果为空时转化为false,否则转化为true

```
if ([0]) {
    // true    
    // 因为数组是对象，对象会被转化为 true
}

var flag = new Boolean(false);

if (flag) {
	console.log('true'); // true,因为flag是Boolean的实例对象
}

```
4.5 eval()  

禁止使用

4.6 原始包装类型

不要使用包装类初始化变量

```
// bad
var num = new Number(1);
var strBird = new String('bird');

// good
var num = Number('1');
var strBird = 'bird';
num = parseInt('1');
num = parseFloat('1.2');
strBird = 'bird';
```

4.7 属性

* 访问对象属性时，使用点形式
* 需要变量访问一个属性时，使用[]来取值

```
var luke = {
  jedi: true,
  age: 28
};

// bad
var isJedi = luke['jedi'];

// good
var isJedi = luke.jedi;
／／－－－－－－－
var luke = {
  jedi: true,
  age: 28
};

function getProp(prop) {
  return luke[prop];
}

var isJedi = getProp('jedi');
```

