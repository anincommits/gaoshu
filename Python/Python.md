# 1、函数
## print
### 示例
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
#### 输出
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
## input
```Python
"""
input("请输入你的年龄:")
# 先打印引号里的内容,再以字符串形式获取输入

ueser_age=input("请输入你的年龄:")
# 此时ueser_age为字符串

int(ueser_age)
# 类型转换
"""
ueser_age=int(input("请输入你的年龄:"))
print("当前年龄为"+str(ueser_age))
ueser_age_after_10_years=ueser_age+10
print("十年后年为"+str(ueser_age_after_10_years))
```
# 2、变量

 **命名规则**
1. 变量起名不能数字打头；不能有空格；不能用引号包裹；
2. 变量赋值：变量名="值"(这样在用print打印的时候不需要再给这个变量加引号，用+连接即可)；   变量="54188"   print(变量)即可
3. 变量转换赋值：变量1="54188"    变量2=变量1    变量1="114514"(一般定义三个变量，用以保存之前变量的同时调用新的变量)
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

# 3、数学运算
Python提供了
+(加)
-(减)
\*(乘)
/(除)
\*\*(次方)
更多操作需要包含math库
## 示例
```Python
import math
print(math.sin(math.pi/2))

# 值得注意的是,Python中表示某个变量属于某个区间很简单:
# 如10<a<20
# 而在C++中,则复杂的多:
# a>10&&a<20
```
### 输出
```Python
1.0
```
# 4、变量类型
## 字符串
```Python
"hello world" # 用单双引号扩起来

# len求字符串长度
print(len("hello world"))
print(len("hello world\n")) # 转义字符视为1个

# 用[]取出字符
print("hello world"[1])
```
### 输出
```Python
11
12
e
```
## 布尔类型
Ture(真)  False(假)
\# 注意大写
## 空值类型
None!=0
None!=""
None!=False
当你创建一个变量而不知道它的值时,初始化为None
## type函数
```Python
print(type("hello"))  
print(type(6))  
print(type(1.0))  
print(type(True))  
print(type(None))
```
### 输出
```Python
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
<class 'NoneType'>
```
# 5、if
if 条件:
   语句
elif 条件:
   语句
else :
   语句
**Python通过缩进判断语句是否属于if**
```Python
mood=int(input("请输入心情:"))
if mood>=60
   print("开心")
   
print("你好")
# 不论条件是否满足,该语句都会执行
# 该语句切断了else与if的联系,导致else报错

else:
    print("难过")
```
这里可以看出三引号("""*注释内容*""")与寻常注释(# *注释内容*)的[[注释#^4d753a|区别]]
将print("你好")放到三引号里,else仍会报错,而直接注掉则不会