
### Import

** Standard library **


```python
import random
```


```python
random.randint(0, 10)
```




    9




```python
random.seed(0)
random.randint(0, 10)
```




    6




```python
random.randint(0, 10)
```




    5




```python
import time
```


```python
time.sleep(2)
print("hello")
```

    hello



```python
sleep(2)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-14-26d13dbb1ac8> in <module>()
    ----> 1 sleep(2)


    NameError: name 'sleep' is not defined



```python
from time import sleep
```


```python
sleep(2)
print("hello")
```

    hello



```python
import math
```


```python
math.sin(90)
```




    0.8939966636005579




```python
math.sin(0 * math.pi / 180)
```




    0.0




```python
import os
```


```python
os.listdir(".")
```




    ['.ipynb_checkpoints',
     'control-flow.ipynb',
     'importing-modules.ipynb',
     'introduction.ipynb',
     'jupyter-notebook-basics.ipynb',
     'README.md']




```python
os.path.
```


      File "<ipython-input-43-09d4214343d6>", line 1
        os.path.
                ^
    SyntaxError: invalid syntax




```python
import mymath
```


    ---------------------------------------------------------------------------

    ModuleNotFoundError                       Traceback (most recent call last)

    <ipython-input-1-7ec2ad592c70> in <module>()
    ----> 1 import mymath


    ModuleNotFoundError: No module named 'mymath'



```python
import mymath
```


```python
mymath.sin(90)
```




    1.0


