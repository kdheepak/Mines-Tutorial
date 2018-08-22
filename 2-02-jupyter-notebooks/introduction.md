
# Introduction to Python




```python
print("hello world")
```

    hello world


**Math**


```python
2 + 2
```




    4




```python
( 2 + 2 )
```




    4




```python
( 3 + 3 )
```




    6




```python
( 2 + 2 ) * ( 3 + 3 )
```




    24




```python
2 + 2 * 3 + 3
```




    11




```python
22 / 7
```




    3.142857142857143




```python
22 // 7
```




    3




```python
22 /                  7
```




    3.142857142857143




```python
1 - 1
```




    0




```python
1 -
```


      File "<ipython-input-11-0af37b9fe585>", line 1
        1 -
           ^
    SyntaxError: invalid syntax



Get used to seeing errors, reading and understanding what they say. The errors in Python are usually very good at pointing out what you did incorrectly.


```python
1 + - 1
```

** Strings **


```python
"Hello World"
```




    'Hello World'




```python
'Hello World'
```




    'Hello World'




```python
"Hello'
```


      File "<ipython-input-105-a8b70a2a59ab>", line 1
        "Hello'
               ^
    SyntaxError: EOL while scanning string literal




```python
"I'm at a Python Tutorial"
```




    "I'm at a Python Tutorial"




```python
"I'm at a \"Python Tutorial\". "
```




    'I\'m at a "Python Tutorial". '




```python
"Hello" + 5
```


```python
"Hello" * 5
```


```python
"Hello" + " " + "World"
```




    'Hello World'



** Variables **


```python
var1 = 1
```


```python
var2 = 2
```


```python
var3 = 3

```


```python
var1 + var2 + var3
```




    6



Variables can be redefined


```python
var1 = "Python"
```


```python
var2 = "Is"
```


```python
var3 = "Fun"
```


```python
var1 + var2 + var3
```




    'PythonIsFun'




```python
var4 = var1 + var2 + var3
```


```python
var4
```

### Exercise

**Exercise**

1) What does `"2" + "3"` give you in Python?

<!--

2) Can you figure out how to make the following string all lowercase?

*Hint: You can might need to check the documentation*

https://docs.python.org/3.6/library/stdtypes.html#string-methods

-->

2) Interchange the values in `variable1` and `variable2`  

```

variable1 = 10
variable2 = 20

```



*Hint: You can use a separate new variable*


```python
variable1 = 10
variable2 = 20
```


```python
print(variable1, variable2)
```

    20 10


### Python Types


```python
int(2)
```




    2




```python
int(2.0)
```




    2




```python
int("2")
```




    2




```python
float(2)
```




    2.0




```python
float("2")
```




    2.0




```python
float("2.5")
```




    2.5




```python
str(2.5)
```




    '2.5'




```python
# str(float(int(2.5)))
```


```python
type(2.5)
```




    float




```python
type(2)
```




    int




```python
type("2")
```




    str




```python
list_of_numbers = [1, 2, 3, 4, 5]
```


```python
list_of_numbers
```




    [1, 2, 3, 4, 5]




```python
type(list_of_numbers)
```




    list




```python
list("12345")
```




    ['1', '2', '3', '4', '5']




```python
1 + 1
```




    2




```python
type(1)
```




    int




```python
type(2.0)
```




    float




```python
1 + 2.0
```




    3.0




```python
type(1 + 2.0)
```




    float




```python
type("1")
```




    str




```python
"1" + 3.0
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-96-a0ccfb6c9743> in <module>()
    ----> 1 "1" + 3.0


    TypeError: must be str, not float


### Valid variable names

Do you know what the difference between a variable and a string is?

Which one is a string and which one is a variable?

```python
string
"variable1"
```

A variable in Python has to always point to something.


```python
variable1 = "valid"
```


```python
1variable = "invalid"
```


      File "<ipython-input-82-a4bf5222a638>", line 1
        1variable = "invalid"
                ^
    SyntaxError: invalid syntax




```python
variable_1 = "valid"
```


```python
variable _ 1 = "invalid"
```


      File "<ipython-input-84-4cec3a9fff68>", line 1
        variable _ 1 = "invalid"
                 ^
    SyntaxError: invalid syntax




```python
variable-1 = "invalid"
```


      File "<ipython-input-85-d604e964a8fa>", line 1
        variable-1 = "invalid"
                              ^
    SyntaxError: can't assign to operator




```python
variable_________1 = "valid"
```


```python
__variable1__ = "valid"
```

**f strings**


```python
month = "Aug"
date = "22nd"
```


```python
f"The month is {month}, and the date is {date}"
```




    'The month is Aug, and the date is 22nd'



** Exercise 2 **

Find what is wrong with the following expression. Can you fix it?


```python
age = 99
```


```python
"I am " + age + " years old."
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-104-552dcf048967> in <module>()
    ----> 1 "I am " + age + " years old."


    TypeError: must be str, not int


Can you make the expression work without changing the expression?

What happens when you use f strings to create the string above?
