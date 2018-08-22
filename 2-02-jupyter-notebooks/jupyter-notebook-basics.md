

```python
print("hello world")
```

    hello world


### Introduction to Jupyter Notebooks

There are two modes: normal mode and insert mode.

See whether the cursor is visible. Press `ESC` to enter normal mode. Press `Enter` to enter insert mode.

In normal mode,

- Use `j` to move down.
- Use `k` to move up.
- Use `m` to convert to a markdown cell
- Use `y` to convert to a code cell
- Use `l` to add line numbers to a code cell
- Use `a` and `b` to add cells before and after the current cell when in normal mode

There are also two types of cells, code cells and markdown cells

This is a markdown cell. Double click on me to edit the cell.


```python
print("This is a code cell")
```

    This is a code cell


### Convert cells


```
print("""
Convert this cell from a code cell to a markdown cell by pressing `m` in normal mode.
Convert it back to a code cell by pressing `y` in normal mode.
""")
```
