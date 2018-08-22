# Exercises

[Exercise 1](./introduction.md#exercise)

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

[Exercise 2](./introduction.md#exercise-2)

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

[Exercise 3](./lists-and-dictionaries.md#exercise-1)

** Exercise 3**

```python
list_of_numbers = list(range(0, 100))
```

1) Create a `list_of_odd_numbers` from the `list_of_numbers`

2) Remove all multiples of `3` from `list_of_odd_numbers`


[Exercise 4](./lists-and-dictionaries.md#exercise-2)

** Exercise 4**

Can you print a table that has both name and color of every animal listed in `animals`


```python
spaces = 4

print(f"Name {' ' *spaces} | Color |")

for animal in animals:

    print(f"{animal['name']} | {animal['color']}")



```

    Name      | Color |
    dog | brown
    cat | white
    bear | black
    squirrel | red



