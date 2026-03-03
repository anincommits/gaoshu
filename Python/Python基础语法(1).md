# 一，汉语简单释义
1. **print**
实现打印输出功能·。
2. 变量
储存或者指代某个值（与C语言含义类似）
3. 数学运算（和c++差不多）
4. 注释（就是标注干啥的）
5. 数据类型：字符（str），整数型（int），浮点型（float），


# 二，语法演示
# 1、print

## 示例

```python

# 单双引号均可

print("hello world")

print('hello world')

  

# 字符串拼接

print("hello"+"world")

print("hello "+"world")

#空格需手动添加

  

# 使用反斜杠"\"打印单双引号

print("I say Let\'s go!")

  

# "\n"为换行

print("第一行\\n\n第二行")

  

# 使用连续三个双(单)引号自动换行

print("""第一行  

第二行""")

```

### 输出

```Python

hello world

hello world

helloworld

hello world

I say Let's go!

第一行\n

第二行

第一行  

第二行

```

# 2、变量

  

 **命名规则**

1. 变量起名不能数字打头；不能有空格；不能用引号包裹；

2. 变量赋值：变量名="值"(这样在用print打印的时候不需要再给这个变量加引号，用+连接即可)；   变量="54188"   print(变量)即可

3. 变量转换赋值：变量1="54188"    变量2=变量1    变量1="114514"(一般定义三个变量，用以保存之前变量的同时调用新的变量)

## 示例

```Python

my_phone="136"  

print(my_phone)  

my_phone_two=my_phone  

my_phone="137"  

print(my_phone)  

print(my_phone_two)

```

### 输出

```Python

136

137

136

```

## 交换两个变量的值

```Python

a="1"

b="2"

print("交换前")

print("a: "+a+",b: "+b)

tem=a

a=b

b=tem

print("交换后")

print("a: "+a+",b: "+b)

```

### 输出

```Python

交换前

a: 1,b: 2

交换后

a: 2,b: 1

```
# 3、数学运算（首先导入math“import math”）


**常量**

1. 不加引号，防止变成字符串

2. 整数类型（6）和浮点类型类型（6.0）

**运算符号**

1. 基础运算符（和C语言一样）
+，-，*，/.
2. 进阶运算符
* 乘方：“\*\*”；2\*\*3：2的三次方
* 三角函数：首先引入math，之后使用“math.sin(?)”再进行print打印就可以显示出所求结果。
* 根号：（1）可以用乘方思想，如2\*\*（1/2）就是√2；
        （2）引用函数math.sqrt(?)计算；
# 示例(求根公式)
输入
```Python
improt math

a=1
b=9
c=20

result_1=(-b+((b**2-4*a*c))**(1/2))/(2*a)
result_2=(-b-((b**2-4*a*c))**(1/2))/(2*a)
print(result_1)
print(result_2)
```

输出
```Python
-4.0
-5.0
```

# 注释

\#这是一个注释，代表我学到了注释
\#这是第二行注释
\#选择，然后按住“control+\”，可以为所有选择的代码加上注释
\#要撤销注释，重复上一个步骤
\#过于简单因此不再加上代码演示谢谢


# 数据类型

1. 字符串（str）

* 用单引号或双引号包围：“hello”
* len（“hello“）可以看长度
* 索引：”hello“\[?],显示第？+1个位置的字符（代码从0开始数）

2. 整型(int)和浮点型(float)

* 整型：6
* 浮点型：6.0

3. 布尔型(bool)

* 真：True
* 假：False

4. 空值类型（NoneType）
* None（空值）

补：type：显示数据类型
    eg：type(6)=<class'int'>