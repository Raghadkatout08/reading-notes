# Python Operations and Exeption Handling

## Python File Operation

Python file operations refer to the set of actions performed on files, including opening, reading, writing, and closing files. These operations are essential for manipulating data stored in files on a computer's file system using Python programming language.

- **Opening function**: Files are opened using the `open()` function, specifying the file name and mode (e.g., read, write, append).

```python
file1 = open("file.txt")
```
- **Reading method**: Content from files is read using methods like read(), readline(), or readlines().

```python
content = file.read()
content = file.readlines()
content = file.readline()
content = file.readable()
```

- **Writing method**: Data can be written to files using the write() method.

```python
file.write("Hello, world!")
```

- **Closing method**: After operations, files should be closed using the close() method.

```python
file.close()
```

- **Using with Statement**: The with statement ensures proper cleanup by automatically closing files.

```python
with open("file.txt") as file:
    content = file.read()
```

## Exception Handling

Exception handling in Python helps manage errors gracefully during program execution.

- **try...except Block**: Handles exceptions that may occur in a block of code.

 ```python
  try:
      result = 10 / 0
  except ZeroDivisionError:
      print("Cannot divide by zero!")
```
- **Handling Specific Exceptions**: Different types of exceptions can be handled separately.

```python 
try:
    num = int(input("Enter a number: "))
    print("Reciprocal:", 1 / num)
except ValueError:
    print("Please enter a valid number.")
```

- **try...finally Block**: Cleanup code can be placed in a finally block, ensuring its execution regardless of exceptions.

```python 
try:
    file = open("file.txt")
    content = file.read()
except FileNotFoundError:
    print("File not found.")
finally:
    file.close()

``` 

- **Raising Exceptions**: Custom exceptions can be raised using the raise keyword.

```python 
x = -1
if x < 0:
    raise ValueError("Negative numbers not allowed.")

```

## Resources

- [File Operation - Programiz](https://www.programiz.com/python-programming/file-operation)
- [Exception Handling - Programiz](https://www.programiz.com/python-programming/exception-handling)
- [Python Try Except - W3Schools](https://www.w3schools.com/python/python_try_except.asp)
- [Reading and Writing Files in Python - Real Python](https://realpython.com/lessons/reading-and-writing-files-python-overview/)
