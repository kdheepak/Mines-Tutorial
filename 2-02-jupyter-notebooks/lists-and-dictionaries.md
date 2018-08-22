
# Lists


```python
list_of_numbers = [1, 2, 3]
```


```python
list_of_numbers[0]
```




    1




```python
list_of_numbers[1]
```




    2




```python
list_of_numbers[2]
```




    3




```python
list_of_numbers[3]
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    <ipython-input-5-c55b5d747f50> in <module>()
    ----> 1 list_of_numbers[3]


    IndexError: list index out of range



```python
list_of_numbers[-1]
```


```python
list_of_numbers[-4]
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    <ipython-input-6-5e15d51d612c> in <module>()
    ----> 1 list_of_numbers[-4]


    IndexError: list index out of range



```python
list_of_numbers[0:2]
```




    [1, 2]




```python
list_of_numbers[0:100]
```




    [1, 2, 3]




```python
list_of_numbers[-100000:100]
```




    [1, 2, 3]




```python
list_of_numbers[0:3:1]
```




    [1, 2, 3]




```python
list_of_numbers[::-1]
```




    [3, 2, 1]




```python
len(list_of_numbers)
```




    3




```python
len("hello world")
```




    11




```python
list_of_numbers + list_of_numbers
```




    [1, 2, 3, 1, 2, 3]




```python
list_of_numbers * 3
```




    [1, 2, 3, 1, 2, 3, 1, 2, 3]




```python
for i in list_of_numbers:
    print(i)
```

    1
    2
    3



```python
"1" in list_of_numbers
```




    False




```python
1 in list_of_numbers
```




    True



### Methods


```python
list_of_numbers.append
```




    <function list.append>




```python
list_of_numbers.append(4)
```


```python
list_of_numbers
```




    [1, 2, 3, 4]




```python
list_of_numbers.insert(0, 0)
```


```python
list_of_numbers
```




    [0, 1, 2, 3, 4]




```python
list_of_numbers = list_of_numbers[::-1]
```


```python
list_of_numbers
```




    [4, 3, 2, 1, 0]




```python
list_of_numbers.sort()
```


```python
list_of_numbers
```




    [0, 1, 2, 3, 4]




```python
list_of_numbers.sort(reverse=True)
```


```python
list_of_numbers
```




    [4, 3, 2, 1, 0]




```python
names = [
    "JOHN",
    "JANE",
]
```


```python
for n in names:
    print(n)
```

    JOHN
    JANE



```python
for n in names:
    n.lower()
```


```python
names
```




    ['JOHN', 'JANE']




```python
for n in names:
    t = n.lower()
    print(f"t = {t}, n = {n}")

```

    t = john, n = JOHN
    t = jane, n = JANE



```python
"hello world".upper()
```




    'HELLO WORLD'




```python
def add_world(list_of_strings):

    list_of_strings.append("World")
```


```python
l = ["hello"]
```


```python
add_world(l)
```


```python
l
```




    ['hello', 'World']




```python
def add_world(string):

    string = string + "World"

```


```python
string = "Hello"
```


```python
add_world(string)
```


```python
string
```




    'Hello'




```python
def add_world(string):

    string = string + "World"
    print(string)
```


```python
"Dheepak".replace("D", "S")
```




    'Sheepak'



**Exercise**


```python
list_of_numbers = list(range(0, 100))
```

1) Create a `list_of_odd_numbers` from the `list_of_numbers`

2) Remove all multiples of `3` from `list_of_odd_numbers`

<!-- Show list comprehension here -->

# Dict


```python
myhouse1 = {"type": "apartment", "color": "white", "square_feet": 2000}
```


```python
myhouse1
```




    {'type': 'apartment', 'color': 'white', 'square_feet': 2000}




```python
myhouse2 = {"color": "white", "square_feet": 2000, "type": "apartment"}
```


```python
myhouse2
```




    {'color': 'white', 'square_feet': 2000, 'type': 'apartment'}




```python
myhouse1 == myhouse2
```




    True




```python
myhouse1["color"]
```




    'white'




```python
myhouse1[0] = 1
```


```python
myhouse1
```




    {'type': 'apartment', 'color': 'white', 'square_feet': 2000, 0: 1}




```python
"color" in myhouse1
```




    True




```python
animals = []
```


```python
while True:
    animal = {}
    name = input("Enter the name of a animal: ")
    color = input(f"Enter the color of the animal {name}: ")

    animal["name"] = name
    animal["color"] = color

    animals.append(animal)

    if len(animals) >= 3:
        break

```

    Enter the name of a animal: Dog
    Enter the color of the animal Dog: brown



    ---------------------------------------------------------------------------

    KeyboardInterrupt                         Traceback (most recent call last)

    ~/miniconda3/lib/python3.6/site-packages/ipykernel/kernelbase.py in _input_request(self, prompt, ident, parent, password)
        728             try:
    --> 729                 ident, reply = self.session.recv(self.stdin_socket, 0)
        730             except Exception:


    ~/miniconda3/lib/python3.6/site-packages/jupyter_client/session.py in recv(self, socket, mode, content, copy)
        802         try:
    --> 803             msg_list = socket.recv_multipart(mode, copy=copy)
        804         except zmq.ZMQError as e:


    ~/miniconda3/lib/python3.6/site-packages/zmq/sugar/socket.py in recv_multipart(self, flags, copy, track)
        394         """
    --> 395         parts = [self.recv(flags, copy=copy, track=track)]
        396         # have first part already, only loop while more to receive


    zmq/backend/cython/socket.pyx in zmq.backend.cython.socket.Socket.recv()


    zmq/backend/cython/socket.pyx in zmq.backend.cython.socket.Socket.recv()


    zmq/backend/cython/socket.pyx in zmq.backend.cython.socket._recv_copy()


    ~/miniconda3/lib/python3.6/site-packages/zmq/backend/cython/checkrc.pxd in zmq.backend.cython.checkrc._check_rc()


    KeyboardInterrupt:


    During handling of the above exception, another exception occurred:


    KeyboardInterrupt                         Traceback (most recent call last)

    <ipython-input-53-b603df2fd41f> in <module>()
          1 while True:
          2     animal = {}
    ----> 3     name = input("Enter the name of a animal: ")
          4     color = input(f"Enter the color of the animal {name}: ")
          5


    ~/miniconda3/lib/python3.6/site-packages/ipykernel/kernelbase.py in raw_input(self, prompt)
        702             self._parent_ident,
        703             self._parent_header,
    --> 704             password=False,
        705         )
        706


    ~/miniconda3/lib/python3.6/site-packages/ipykernel/kernelbase.py in _input_request(self, prompt, ident, parent, password)
        732             except KeyboardInterrupt:
        733                 # re-raise KeyboardInterrupt, to truncate traceback
    --> 734                 raise KeyboardInterrupt
        735             else:
        736                 break


    KeyboardInterrupt:



```python
animals = [{'name': 'dog', 'color': 'brown'},
 {'name': 'cat', 'color': 'white'},
 {'name': 'bear', 'color': 'black'},
 {'name': 'squirrel', 'color': 'red'}]
```

**Exercise**

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

