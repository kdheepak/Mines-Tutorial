
# Introduction to Python

```python
print("hello world")
```


```python
1 + 1
```


```python
2 * 4
```

This is a markdown cell




```python
This is a code cell
```

Use `m` and `y` to convert between code cells and markdown cells


```python
"This is a code cell"
```

## Expressions

### Math


```python
2 + 2
```


```python
( 2 + 2 )
```


```python
( 2 + 2 ) * ( 3 + 3 )
```


```python
2 + 2 * 3 + 3
```


```python
22 / 7
```


```python
22 /              7
```


```python
1 - 1
```


```python
1 -
```


```python
1 -

print( 2 ** 10 )
```


```python
1 + - 1
```

### Strings


```python
"Hello World"
```


```python
'Hello World'
```


```python
"Hello'
```


```python
"I'm at a Python Tutorial"
```


```python
'I\'m at a Python Tutorial'
```


```python
"I\'m at a Python Tutorial"
```


```python
"Hello" + 5
```


```python
"Hello" * 5
```


```python
"Hello" + " " + "World"
```


```python
"na" * 10 + " Batman"
```


```python
("na" * 10) + " Batman"
```

### Variables


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


```python
var1 = "Python"
```


```python
var2 = "is"
```


```python
var3 = "Fun"
```


```python
var1 + var2 + var3
```


```python
var4 = var1 + var2 + var3
```


```python
var4
```

### Exercise


```python
variable1 = 10
```


```python
variable2 = 20
```


```python
print(variable1, variable2)
```


```python
variable2, variable1 = variable1, variable2
```


```python
print(variable1, variable2)
```

### Python types


```python
2
```


```python
type(2)
```


```python
int(2)
```


```python
int(2.0)
```


```python
int(2.5)
```


```python
int("2")
```


```python
int("2.0")
```


```python
float(2.0)
```


```python
float(2)
```


```python
float("2")
```


```python
type("2")
```


```python
type(2.0)
```


```python
type(2)
```


```python
type(int)
```


```python
type(type)
```


```python
variable = "this is a string"
```


```python
type(variable)
```


```python
variable = 2
```


```python
type(variable)
```


```python
variable = 2.0
```


```python
type(variable)
```


```python
[1, 2, 3, 4, 5]
```


```python
variable = [1, 2, 3, 4, 5]
```


```python
type(variable)
```


```python
1 + 2.0
```


```python
"1" + 3.0
```


```python
int("1") + 3.0
```

### Valid variable names


```python
string
"variable1"
```


```python
string = ""
```


```python
string
"variable1"
```


```python
variable1 = "valid"
```


```python
1variable = "invalid"
```


```python
#variable = "invalid"
```


```python
variable_1 = "valid"
```


```python
variable_______1 = "valid"
```


```python
______variable______ = "valid"
```


```python
variable = None
```


```python
variable
```


```python
print(variable)
```

### f strings


```python
month = "Aug"
date = "22nd"
```


```python
"The month is " + month + ", and the date is " + date
```


```python
f"The month is {month}, and the date is {date}"
```


```python
"The month is {month}, and the date is {date}"
```

### Exercise


```python
age = 99
```


```python
"I am " + age + "years old."
```





### Exercise-1

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

### Exercise-2

** Exercise **

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
