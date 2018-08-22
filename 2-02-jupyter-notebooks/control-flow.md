
# Control Flow






**Basic control flow primitives**

```python
True
```


```python
False
```


```python
variable = True
```


```python
variable
```


```python
True
```


**Comparison operators**

```python
variable == True
```


```python
1 == 1
```


```python
1 == 1.0
```


```python
type(1) == type(1.0)
```


```python
1 == "1"
```


```python
True == True
```


```python
True != "True"
```


```python
"hello" == "world"
```


```python
"hello" == "Hello"
```


```python
"hello" == "hello"
```


```python
"hello " == "hello"
```


```python
10 < 20
```


```python
"a" < "b"
```


```python
"a" < "aa"
```


```python
5 < 5
```


```python
5 <= 5
```


```python
None == None
```


**Binary operators**


```python
True and True
```


```python
True and False
```


```python
False and True
```


```python
True or False
```


```python
not True
```


```python
not not True
```


```python
myage = 30
```


```python
15 < myage and myage < 60
```


```python
15 < myage < 60
```


**If else conditions**


```python
if myage >= 21:

    print("Age is over 21")

print("This is always be printed because it is not indented")
```


```python
name = "John Doe"
```


```python
if name == "John Doe":

    print("My first name is John")

else:

    print("My first name is NOT John")
```


```python
from time import sleep

counter = 5

while True:

    print(f"Counter is {counter}")
    sleep(1)
    counter = counter - 1
```


```python
from time import sleep

counter = 5

while True:

    print(f"Counter is {counter}")
    sleep(1)
    counter = counter - 1

    if counter == 0:
        break
```


```python
from time import sleep

counter = 5

while counter != 0:

    print(f"Counter is {counter}")
    sleep(1)
    counter = counter - 1

```


```python
while True:

    myname = input("What is your name: ")
    if myname != "John":
        continue
    print("This will only be printed when the name is John")
    break
```


```python
for i in range(10):

    print(f"The value of i is {i}")
```


```python
for c in "abcdef":
    print(c)
```


```python
for i in range(10, -10, -1):

    try:
        print(f"10/{i} = {10/i}")
    except:
        print(f"#### Unable to perform operation for {i}")

    # sleep(1)

```

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
