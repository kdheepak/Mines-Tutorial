
# Lists and Dictionaries

### Lists


```python
list_of_numbers = [1, 2, 3]
```


```python
list_of_numbers[0]
```


```python
list_of_numbers[1]
```


```python
list_of_numbers[2]
```


```python
list_of_numbers[3]
```


```python
list_of_numbers[-1]
```


```python
list_of_numbers[-4]
```


```python
list_of_numbers[0:2]
```


```python
0:2
```


```python
(0:2)
```


```python
list_of_numbers[0:10]
```


```python
list_of_numbers[0:100]
```


```python
list_of_numbers[0:]
```


```python
list_of_numbers[:]
```


```python
list_of_numbers[-100:100]
```


```python
list_of_numbers[0:3:1]
```


```python
list_of_numbers[0:3:2]
```


```python
list_of_numbers[::-1]
```


```python
list_of_numbers + list_of_numbers
```


```python
list_of_numbers * 5
```


```python
len(list_of_numbers)
```


```python
list_of_characters = "hello world"
```


```python
len(list_of_characters)
```


```python
list_of_characters[0]
```


```python
list_of_characters[0:5]
```


```python
list_of_characters[5:]
```


```python
list_of_characters[:5] + list_of_characters[5:]
```


```python
for i in list_of_numbers:
    print(i)
```


```python
for c in list_of_characters:
    print(c)
```


```python
if 1 in list_of_numbers:
    print("1 is in the list_of_numbers")
```


```python
if "hello" in list_of_characters:
    print("hello is part of the string")
```

### Methods


```python
list_of_numbers = [1, 2, 3]
```


```python
list_of_numbers.append(5)
```


```python
list_of_numbers
```


```python
list_of_numbers.insert(3, 4)
```


```python
list_of_numbers
```


```python
list_of_numbers.insert(0, 0)
```


```python
list_of_numbers
```


```python
list_of_numbers[::-1]
```


```python
list_of_numbers.sort()
```


```python
list_of_numbers
```


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


```python
for n in names:
    print(n.lower())
```


```python
for n in names:
    n.lower()
    print(n)
```


```python
for n in names:
    t = n.lower()
    print(n, t)
```


```python
def append(list_of_strings):
    list_of_strings.append("World")
```


```python
l = ["hello"]
```


```python
append(l)
```


```python
l

```


```python
def append(string):
    string = string + "World"
```


```python
s = "hello"
```


```python
append(s)
```


```python
s
```

### Exercise


```python
list_of_numbers = list(range(0, 100))
```

### Dictionaries


```python
myhouse1 = {"type": "apartment", "color": "white", "square_feet": 2000}
```


```python
myhouse1
```


```python
myhouse1["color"]
```


```python
myhouse2 = {'color': 'white', 'square_feet': 2000.0, 'type': 'apartment'}
```


```python
myhouse2
```


```python
myhouse1 == myhouse2
```


```python
animals = []

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


```python
animals
```

### Exercise


```python
SPACES = 10
spaces = (SPACES - len("Name"))
header = f"Name {' ' * spaces} | Color"
print(header)
print(len(header) * "-")
for animal in animals:
    spaces = SPACES - len(animal["name"])
    print(f"{animal['name']} {' ' * spaces} | {animal['color']}")
```

See string formatting in Python
