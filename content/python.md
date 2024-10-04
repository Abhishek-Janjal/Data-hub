# 1. Introduction to python
$\Large Easy\ to\ Learn \newline$
Python is a simple and minimalistic language. Reading a good Python program feels almost like reading English, although very strict English! This pseudo-code nature of Python is one of its greatest strengths. It allows you to concentrate on the solution to the problem rather than the language itself.

$\Large Free\ and\ Open\ Source \newline$
Python is an example of a FLOSS (Free/Libre and Open Source Software). In simple terms, you can freely distribute copies of this software, read its source code, make changes to it, and use pieces of it in new free programs. FLOSS is based on the concept of a community which shares knowledge. 

$\Large Object\ Oriented \newline$
Python supports procedure-oriented programming as well as object-oriented programming (OOP). In procedure-oriented languages, the program is built around procedures or functions which are nothing but reusable pieces of programs.

## Download Anaconda Distribution
Go to https://anaconda.com/ and select Anaconda Individual Edition to download the latest version of Anaconda

# 2. Variables
```python
# valid variable name
b='xyz'
a='dsfsf'
animal1="Cat"
animal2="Dog"
a1=2345234532532
a_123=13.5
_a_=8
_a=233
a_=343
```

```python
#case sensetive
y=5
Y=4
print(y,Y)
```
_5 4_

# 3. Data Types
```python 
#type() funtion
a=1
b=0.1
c='word'
print(type(a))
print(type(b))
print(type(c))
```
_<class 'int'>_
_<class 'float'>_
_<class 'str'>_

# 4. Operators
| Operators | code | output |
|:----------| :---:|-------:|
| addition|12+13|25|
|substraction|13-12|1|
|multiplication|11*2|22|
|division|10/2|5|
|floor division| 13//2| 6|
|power|12**3|1728|
|modulus|24%2|0|

# 5. Input/Output function
```python
#different way of printing string data
print('Hello world')

print("Hello world")

print('Hello','world')

print("""What is Bias?
• Error between average model prediction and ground truth
• The bias of the estimated function tells us the capacity of the underlying model to predict the values""")

```
_Hello world_
_Hello world_
_Hello world_
_What is Bias?_
_• Error between average model prediction and ground truth_
_• The bias of the estimated function tells us the capacity of the underlying model to predict the values_


```python
#printing variable using format method
s=57
a=5.6
print("sum:{}\nAverage:{}".format(s,a))
print(f"sum:{s}\nAverage:{a}")
```
_sum:57_
_Average:5.6_
_sum:57_
_Average:5.6_


```python
#input function
name=input('what is your name: ')
print(name)
```
# 6. Comparison & Logical Operators
| Comparison Operators | code | output |
|:---------------------| :---:|-------:|
|Equal|`10==11`|False|
|Not equal| `10!=10`|False|
|Greater than|`7>4`|True|
|Less than|`7<4`|False|
|Greater than or equal to|`12>=12`|True|
|Less than or equal to|`13<=13`|True|

| Logical Operators |Description|code | output |
|:----------------- |:---------:|:---:|-------:|
|and|Return True if both statements are true|`True and True`|`True`|
|or|Return True if one of the statemets is true|`True or False`|`True`|
|not|Reverse the result,returns False if the result is true|`not(True and False)`|`True`|

# 7. Conditional Statements  ,implicit & explicit
```python
#if-else
grade=40
if grade>50:
  print('pass')
else:
  print('fail')
```

```python
#if-elif-else
grade=85
if grade>=90:
  print('A')
elif grade>=80:
  print('B')
elif grade>=70:
  print('C')
elif grade>=60:
  print('D')
else:
  print('F')
```
# 8. Loops
```python
#---------For Loop----------------#
#example 1
for i in range(0,10,2): #range(start,end,step)
  print(i)

#example 2
for i in range(5):
  a=int(input('Enter first number'))
  b=int(input('Enter second number'))
  sum=a+b
  print(f"Sum of 2 no's {sum}")

#example 3
ls=['ram','karan',34,54 ,12.1]
for i in ls:
  print(i)

#---------While Loop----------------#
#example 1
n=10
i=1
while i<=10:
  print(i)
  i+=1 #i=i+1

#example 2
i=555
n=567
while i<=n:
  if i%2!=0:
    print(i)
  i+=1

#example 3
color=['vilot','indigo','blue','green','yellow','orange','red']
v=iter(color)
while True:
  print(next(v))
```
# 9. implicit & explicit
```python
#implicit , also known as automatic type conversion
#explicit propertie of python where we convert the type of variable as follow
a='7'
print(f'a = {type(a)}')
a=int(a)
print(f'a = {type(a)}')
a=float(a)
print(f'a = {type(a)}')
```
_a = <class 'str'>
a = <class 'int'>
a = <class 'float'>_
# 10 .List, Tuple, Dictionary, Set
```python
#List - Mutable
ls=[1,2,3,4,5]

#Tuple - Immutable
tp=(6,7,8)

#set
s={1,2,3,'ram'}

#Dictionary
dic={1:'Krishna',2:'Karan'} 
```
> ### List
```python
ls1=['ram',12,23,45.3,'seta','karan',34543,34]
ls2=[1,2,3]
print(type(ls1))
print(len(ls1))
```
_<class 'list'>
8_

```python
#indexing front2back
print(ls1[0])
#indexing back2front
print(ls1[-1])
#slicing
print(ls1[1:4])
```
_ram
34
[12, 23, 45.3]_

```python
l1=[1,2,3,"hello",34]
l1.insert(3,[4,5])
l1
#list is insert at index 3
```
_[1, 2, 3, [4, 5], 'hello', 34]_

```python
l1.reverse()
l1
```
_[34, 'hello', [4, 5], 3, 2, 1]_

```python
l1=[4,6,1,7,8,2,3]
l1.sort()
l1
```
_[1, 2, 3, 4, 6, 7, 8]_

> ### Tuple
```python
tp=()
type(tp)
```
_tuple_
```python
#two ways of writing tuple
tp=('john','green',3.3)
tp1='john','green',3.3
print(tp)
print(tp1)
```
('john', 'green', 3.3)
('john', 'green', 3.3)


```python
#changing the value of tuple at index 2 i.e list inside the tuple and inside the list index 1 is changed
tp=('john','blue',[98,75,87])
tp[2][1]=85
tp
```
_('john', 'blue', [98, 85, 87])_

```python
# unpacking sequences
student_tuple=('john',[98,85,87])
first_name,score=student_tuple
print(first_name)
print(score)
```
_john
[98, 85, 87]_


> ### Dictionary
```python
country_code={'Finland':'fi','South Africa':'za','nepal':'np'}
country_code['Finland']
```
_'fi'_

```python
country_code.keys()
```
_dict_keys(['Finland', 'South Africa', 'nepal'])_

```python
country_code.values()
```
_dict_values(['fi', 'za', 'np'])_

```python
country_code.items()
```
_dict_values(['fi', 'za', 'np'])_


> ### Set
```python
ss={'ram','karan','karan'}
ss
# that means it does not allow duplicate value
```
_{'karan', 'ram'}_

```python
ss.add(5)
ss
```
_{5, 'karan', 'ram'}_

```python
ss.update((2,'sita'))
ss
```
_{2, 'karan', 'ram', 'sita'}_

# 11. Functions
```python
def square(num):
  sq=num**2
  return sq
square(7)
```
_49_
```python
'''using parameter and also define the type of parameters
Note: if your function expects 2 arguments, you have to call the function with 2 arguments not more or less
also if you input the wrong type of parameter can cause error
'''
def my_function(name:str,age:int):
    print(f"My name is {name} and I am {age} year old")
my_function('John',50)
```
_My name is John and I am 50 year old_
```python
#Default Parameter Value
def my_function(country="Norway"):
    print("I am from " + country)

my_function('India')
my_function()
```
_I am from India_
_I am from Norway_
```python
#The function will receive a tuple of arguments, and can access the items accordingly
def my_function(*names):
    print(f"My name is {names[2]}")
my_function('John','Noah','Henry')
```
_My name is Henry_

# 12. Exception handling

```python
# if you put string or floating it will give you prompt `Please enter a number`
try:
  x=int(input())
except :
  print("Please enter a number")
finally:
  print('hello')
```
# 13.comprehension, lambda, map(), filter(), reduce()
```python
#example 1
ls=[i for i in range(1,21) if i%2==0]

#example 2
dic={}
for i in range(1,21):
  dic.update({i:i*i})
```
_[2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64, 9: 81, 10: 100}_


```python
#example 1
x=lambda a,b:a*b
print(x(5,6))

#example 2
x=lambda a,b,c:a+b+c
print(x(5,6,2))
```
_30
13_

```python
#map()
numbers=(1,2,3,4)
result = map(lambda x:x+x,numbers)
print(list(result))
```
_[2, 4, 6, 8]_

```python
#filter()
seq=[0,1,2,3,4,5,8,13]

result = filter(lambda x:x%2 !=0,seq)
print(list(result))
```
_[1, 3, 5, 13]_

```python
from functools import reduce
numbers=[1,2,3,4,5]
sum_result = reduce(lambda x,y:x+y,numbers)
print(sum_result)
```
_15_
