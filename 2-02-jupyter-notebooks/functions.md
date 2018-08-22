
### Functions


```python
def function_name():
    print("hello world")
```


```python

function_name()
```

    hello world



```python
function_name()
```

    hello world



```python
def add_two_numbers(x, y):

    print(x + y)


```


```python
add_two_numbers(1, 2)
```

    3



```python
def add_two_numbers_and_return_result(x, y):

    print(x + y)

    z = x + y

    return z
```


```python
add_two_numbers_and_return_result(1, 2)
```

    3





    3




```python
variable = add_two_numbers_and_return_result(1, 2)
```

    3



```python
variable = add_two_numbers(1, 2)
```

    3



```python
variable == 3
```




    False




```python
variable == None
```




    True




```python
def add_two_strings_with_a_space(s1, s2):

    return s1 + " " + s2

```


```python
add_two_strings_with_a_space("hello", "world")
```




    'hello world'




```python
add_two_strings_with_a_space(s1="hello", s2="world")
```




    'hello world'




```python
s1
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-15-d0257f733e5e> in <module>()
    ----> 1 s1


    NameError: name 's1' is not defined



```python
s2
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-16-630081a5992e> in <module>()
    ----> 1 s2


    NameError: name 's2' is not defined



```python
add_two_strings_with_a_space(s3="hello", s2="world")
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-17-abdfc691fda2> in <module>()
    ----> 1 add_two_strings_with_a_space(s3="hello", s2="world")


    TypeError: add_two_strings_with_a_space() got an unexpected keyword argument 's3'



```python
add_two_strings_with_a_space(s1="hello", s2="world")
```




    'hello world'




```python
add_two_strings_with_a_space(s2="world", s1="hello")
```




    'hello world'




```python
def add_two_strings(s1, s2, delimiter=" "):

    return s1 + delimiter + s2
```


```python
add_two_strings("hello", "world")
```




    'hello world'




```python
add_two_strings("hello", "world", "_______")
```




    'hello_______world'




```python
add_two_strings("hello", "world", delimiter="_______")
```




    'hello_______world'




```python
add_two_strings?
```


```python
# Redefine functions
```

### Scopes and Functions


```python
def function():
    name = "John Doe"
    print(name)
```


```python
function()
```

    John Doe



```python
name
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-27-9bc0cb2ed6de> in <module>()
    ----> 1 name


    NameError: name 'name' is not defined

