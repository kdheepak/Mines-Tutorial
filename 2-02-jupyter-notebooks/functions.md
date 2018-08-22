# Functions

### Functions


```python
print("hello world")
```


```python
print
```


```python
type(print)
```


```python
sleep
```


```python
type(sleep)
```


```python
def function_name():
    print("hello world")
```


```python
function_name
```


```python
type(function_name)
```


```python
function_name()
```


```python
def add_two_numbers(x, y):
    print(x + y)
```


```python
add_two_numbers(1, 2)
```


```python
z = add_two_numbers(1, 2)
```


```python
z
```


```python
z == None
```


```python
def add_two_numbers_and_return_result(x, y):
    print(x + y)
    return x + y
```


```python
add_two_numbers_and_return_result(1, 2)
```


```python
z = add_two_numbers_and_return_result(1, 2)
```


```python
z
```


```python
def add_two_strings_with_a_space(s1, s2):

    return s1 + " " + s2
```


```python
add_two_strings_with_a_space("hello", "world")
```


```python
add_two_strings_with_a_space(s1="hello", s2="world")
```


```python
s1
```


```python
add_two_strings_with_a_space(s3="hello", s2="world")
```


```python
add_two_strings_with_a_space(s2="world", s1="hello")
```


```python
def add_two_strings(s1, s2, delimiter=" "):

    return s1 + delimiter + s2
```


```python
add_two_strings("hello", "world")
```


```python
add_two_strings("hello", "world", "_______")
```


```python
add_two_strings("hello", "world", delimiter="_______")
```

### Scopes


```python
def function():
    my_name_inside_function = "John Doe"
    print(my_name_inside_function)
```


```python
function()
```


```python
my_name_inside_function
```


```python
age = 100
```


```python
def function():
    print(age)
```


```python
function()
```
