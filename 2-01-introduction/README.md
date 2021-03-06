# Python

Python refers to the Python programming language.
Python also refers to the interpreter software [CPython](https://github.com/python/cpython).
CPython is the reference implementation of Python language written in C.
CPython is the most widely-used implementation of the language.
Other implementations of Python include Jython, IronPython, PyPy etc.

### Why choose Python?

Python is very popular.
It ranks 1 in [IEEE Spectrum's top ten languages of 2018](https://spectrum.ieee.org/at-work/innovation/the-2018-top-programming-languages).
It ranks 7 in [StackOverflow's most popular technolgies](https://insights.stackoverflow.com/survey/2018).

You can use Python for almost anything.
A good quote I've heard is that Python is the second best language for everything.
It is used in data science, scientific and mathematical computing, web development, automation and more.

Python is simple, easy and fun to learn. It is also free.

See [dbader](https://dbader.org/blog/why-learn-python) post for more on why Python?

### How do you run Python?

Open a Terminal or the Command Prompt.

*Note: We’ll be showing number of commands as code snippets in the following presentation using a terminal, and those lines all start with `$`.
You don’t need to type in the `$` character; they are there to indicate the start of each command.
Lines that don’t start with `$` are typically showing the output of the previous command.*

Type `python` and hit enter.

```bash
$ python
Python 3.6.4 |Anaconda, Inc.| (default, Jan 16 2018, 12:04:33)
[GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
>>>
>>>
>>> print("hello world")
hello world
>>>
```

The three `>` is the prompt. Anything you type after the prompt must be valid Python code.
Go on, try to print the string `hello world` on to the screen.

You can also create a file on your computer, for example `main.py`, add the text `print("hello world")` and run it using Python by typing:

```
$ python main.py
```

There is also `ipython`.

### Exercise 1

```python
>>> 1 + 1

>>> 2 - 1

>>> 1 - 2

>>> 22 / 7

>>> 2 ** 10

>>> 2 ** 1000
```

### Exercise 2

- Try multiplication and division.
- What rules does Python follow for ordering?
- Try to figure out what `%` does

<!--

Fun fact:

The name Python comes from the British comedy group Monty Python, and not from the snake.
Python programmers are usually called Pythonistas.
There are many Monty Python and snake references peppered around Python tutorials and documentation. Can you find them?

-->

