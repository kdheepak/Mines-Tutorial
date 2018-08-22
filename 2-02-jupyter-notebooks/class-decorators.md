
### decorators


```python
def main_function(x, y):

    print(x, y)


```


```python
main_function(3, 4)
```

    3 4



```python
def always_use_1(y):

    main_function(1, y)
```


```python
always_use_1(3)
```

    1 3



```python
def always_use_1_2():
    always_use_1(2)
```


```python
always_use_1_2()
```

    1 2



```python
def decorator_function(function):

    def function(x, y):
        print(1, y)

    return function
```


```python
def hello(x, y):
    print(x, y)
```


```python
hello = decorator_function(hello)
```


```python
hello(10, 4)
```

    1 4



```python
@decorator_function
def hello(x, y):
    print(x, y)
```


```python
hello(100, 4)
```

    1 4


### classes


```python
class Animal(object):

    def __init__(self, name, color, kind):

        self.name = name
        self.color = color
        self.kind = kind

    def make_sound(self):
        if self.kind == "dog":
            print("woof!")
        else:
            raise NotImplementedException("I don't know what kind of Animal this is")

    def __repr__(self):
        return f"<{self.__class__.__name__}(name='{self.name}', color='{self.color}')>"


```


```python
a = Animal("einstein", "white", "dog")
```


```python
a
```




    <Animal(name='einstein', color='white')>




```python
a.name
```




    'einstein'




```python
a.color
```




    'white'




```python
a.kind
```




    'dog'




```python
a.make_sound()
```

    woof!



```python
class Dog(Animal):

    def __init__(self, name, color):

        super().__init__(name, color, "dog")

```


```python
d = Dog("rudolf", "pink")
```


```python
d
```




    <Dog(name='rudolf', color='pink')>




```python
d.name
```




    'rudolf'




```python
d.color
```




    'pink'




```python
d.kind
```




    'dog'




```python
d.make_sound()
```

    woof!



```python
class Cat(Animal):

    def __init__(self, name, color):

        super().__init__(name, color, "cat")

    def make_sound(self):
        print("meow")
```


```python
c = Cat("kitty", "black")
```


```python
c
```




    <Cat(name='kitty', color='black')>




```python
c.make_sound()
```

    meow

