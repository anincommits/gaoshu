for 变量名 in 可迭代对象
   \# 执行语句
通过缩进判断是否属于for循环

# 列表
```Python
num=[1,2,3,4,5,6]
for i in num:
  if i<3:
   print(i)
```
**输出**
```Python
1
2
```
# 字典
```Python
temperature={"1号":36.4,
"2号":37,
"3号":36.6}

for id,tem in temperature.items():
   if tem >36.5:
    print(id)
    print(tem)
# items方法返回键值对,id被key赋值,tem被value赋值
# keys方法返回key
# values方法返回value

"""
for tuple in temperature.items():
    id=tuple[0]
    tem=tuple[1]
    if tem>36.5:
       print(id)
       print(tem)
"""

```
**输出**
```Python
2号
37
3号
36.6
```
# range
```Python
sum=0
for i in range(1,101):
  sum=sum+i
print(sum)
# i从1开始,到100停止,每次+1

for i in range(1,10,2):
  print(i)
# i从1开始,到9停止,每次+2

str="hello"
for i in range(len(str)):
  print(str[i])
# i从0开始,到len(str)-1结束,每次+1
```
**输出**
```Python
5050
1
3
5
7
9
h
e
l
l
o
```
# 求平均值
```Python
sum=0  
n=0  
i=input("输入数字(输入e退出)")  
while i!="e":  
   sum+=float(i)  
   n+=1  
   i = input("输入数字(输入e退出)")  
if n==0:  
   result=0  
else :  
   result=sum/n  
print(result)
```