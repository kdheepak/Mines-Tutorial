
# Control Flow






**Basic control flow primitives**


```python
True
```




    True




```python
False
```




    False




```python
variable = True
```


```python
variable
```




    True



**Comparison operators**


```python
variable == True
```




    True




```python
1 == 1
```




    True




```python
1 == 1.0
```




    True




```python
2 == 1
```




    False




```python
1 == int(1.5)
```




    True




```python
True == True
```




    True




```python
1 != 2
```




    True




```python
"hello" == "world"
```




    False




```python
"hello" != "world"
```




    True




```python
"hello" == "Hello"
```




    False




```python
10 < 20
```




    True




```python
10 >= 5
```




    True




```python
5 >= 5
```




    True




```python
5 > 5
```




    False



**Binary operators**


```python
# `and`
```


```python
True and True
```




    True




```python
True and False
```




    False




```python
False and True
```




    False




```python
False and False
```




    False




```python
# `or`
```


```python
True or False
```




    True




```python
False or False
```




    False




```python
# `not`
```


```python
not True
```




    False




```python
not False
```




    True




```python
not not True
```




    True




```python
not (not True)
```




    True




```python
myage = 30
```


```python
(15 < myage) and (myage < 60)
```




    True




```python
15 < myage < 60
```




    True



** If else conditions **


```python
if myage >= 21:

    print("Age is over 21")

print("This will always be printed because it is not indented.")
```

    Age is over 21
    This will always be printed because it is not indented.


Python is whitespace sensitive.

Convention is to leave 4 spaces for a block of code.


```python
name = "John Doe"
```


```python
if name == "John Doe":

    print("My first name is John.")

else:

    print("My first name is NOT John.")
```

    My first name is John.


**while conditions**


```python
from time import sleep

counter = 5

while True:

    print("Counter is " + str(counter))

    sleep(1)

    counter = counter - 1
```

    Counter is 5
    Counter is 4
    Counter is 3
    Counter is 2
    Counter is 1
    Counter is 0
    Counter is -1
    Counter is -2



    ---------------------------------------------------------------------------

    KeyboardInterrupt                         Traceback (most recent call last)

    <ipython-input-81-78a2d3fec4d6> in <module>()
          7     print("Counter is " + str(counter))
          8
    ----> 9     sleep(1)
         10
         11     counter = counter - 1


    KeyboardInterrupt:



```python
from time import sleep

counter = 5

while True:

    print("Counter is " + str(counter))

    sleep(1)

    counter = counter - 1

    if counter == 0:

        break
```

    Counter is 5
    Counter is 4
    Counter is 3
    Counter is 2
    Counter is 1
    End



```python
from time import sleep

counter = 5

while counter != 0:

    print("Counter is " + str(counter))

    sleep(1)

    counter = counter - 1

```

    Counter is 5
    Counter is 4
    Counter is 3
    Counter is 2
    Counter is 1



```python
while True:

    myname = input("Enter your name: ")

    if myname != "John Doe":
        continue

    break


print("Hello John Doe, I've been expecting you.")
```

    Enter your name: Dheepak
    Enter your name: Alice
    Enter your name: John Doe
    Hello John Doe, I've been expecting you.


** for loops **


```python
for i in range(10):

    print("The value of i is " + str(i))
```

    The value of i is 0
    The value of i is 1
    The value of i is 2
    The value of i is 3
    The value of i is 4
    The value of i is 5
    The value of i is 6
    The value of i is 7
    The value of i is 8
    The value of i is 9


**Exceptions**


```python
1 / 0
```


    ---------------------------------------------------------------------------

    ZeroDivisionError                         Traceback (most recent call last)

    <ipython-input-1-bc757c3fda29> in <module>()
    ----> 1 1 / 0


    ZeroDivisionError: division by zero



```python
try:

    1 / 0

except ZeroDivisionError:

    print("Cannot divide 1 by 0")
```

    Cannot divide 1 by 0



```python
for i in range(10, -10, -1):

    print(10 / i)

```

    1.0
    1.1111111111111112
    1.25
    1.4285714285714286
    1.6666666666666667
    2.0
    2.5
    3.3333333333333335
    5.0
    10.0



    ---------------------------------------------------------------------------

    ZeroDivisionError                         Traceback (most recent call last)

    <ipython-input-6-acc88be3f428> in <module>()
          1 for i in range(10, -10, -1):
          2
    ----> 3     print(10 / i)


    ZeroDivisionError: division by zero



```python
for i in range(10, -10, -1):

    try:
        print(10 / i)
    except:
        print(f"##### Unable to perform operation for {i} #####")
```

    1.0
    1.1111111111111112
    1.25
    1.4285714285714286
    1.6666666666666667
    2.0
    2.5
    3.3333333333333335
    5.0
    10.0
    ##### Unable to perform operation for 0 #####
    -10.0
    -5.0
    -3.3333333333333335
    -2.5
    -2.0
    -1.6666666666666667
    -1.4285714285714286
    -1.25
    -1.1111111111111112


### Falseness in Python


```python
if "":
    print("hello")
```


```python
if None:
    print("hello")
```


```python
if 0:
    print("hello")
```


```python
if []:
    print("hello")
```
