# Exercises

### Exercise 1

**Exercise - Part 1**

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

** Exercise - Part 2 **

3) Find what is wrong with the following expression. Can you fix it?


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

### Exercise 2

FizzBuzz programming challenge

Write a program that prints the numbers from 1 to 100. But for multiples of three print "Fizz" instead of the number and for the multiples of five print "Buzz". For numbers which are multiples of both three and five print "FizzBuzz".

### Exercise 3

1) Define a function which can compute the sum of two numbers.
2) Define a function that can convert a integer into a string and print it in console.
3) Define a function that can convert a integer into a string and returns the string.
4) Define a function that can accept two strings as input and print the string with maximum length in console. If two strings have the same length, then the function should print all strings line by line. Can you make this function work for `N` number of strings, i.e. an arbitrary number of strings?
5) Can you write a function that calculates the factorial of any number?

### Exercise 4

1) Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included).
Can you print the numbers in a comma-separated sequence on a single line?

2) Write a program to print the list after removing the value 24 in [12,24,35,24,88,120,155].

Can you do the above two with list comprehension?

3) With two given lists [1,3,6,78,35,55] and [12,24,35,24,88,120,155], write a program to make a list whose elements are intersection of the above given lists.

### Exercise 5

Can you print a table that has both name and color of every animal listed in `animals`

    Name      | Color |
    dog | brown
    cat | white
    bear | black
    squirrel | red


### Exercise 6

Can you make a hangman game?

```
>>> Welcome to Hangman!
_ _ _ _ _ _ _ _ _
>>> Guess your letter: S
Incorrect!
>>> Guess your letter: E
E _ _ _ _ _ _ _ E
```

### Exercise 7

How would you go about making a tic tac toe game in Python? Can you describe the algorithm on paper? What data structures in Python could you use to accomplish this task?

### Exercise 8

Write a XKCD random comic generator.

