# FileIO and Exceptions

## Read and Write files in python

Information from https://realpython.com/read-write-files-python/

A file is a contiguous set of bytes used to store data. To make a long story short these files are translated into binary 1 and 0 so it can be processed by the computer

Three main parts of a file:

1. Header: metadata about the file
2. Data: contents of the file
3. End of file (EOF): character that indicates the end of the file

Files can be formatted for different use cases. These formats are indicated by the file extension for example: .svg, .txt, .csv, .jpg just to name a few.

If you want to work with a file in Python you first have to open it

`file = open('file.txt')`

When a file is opened it is best practice to close it after your tasks are complete. One way to do this is through a try-finally block:

```py
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

A second way is by using a with block which will automatically close the file after the code block is executed

```py
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

Files can be opened in different modes which will enable different features. The most common are the following:

- 'r': reading
- 'w': writing, (overwriting the existing contents)
- 'rb' or 'wb': binary mode

## Exceptions in python

Exception errors are errors that occur when syntactically correct code results in an error. When an error occurs, the script is usually terminated. In order to prevent the script from terminating you can implement an excpetion to catch a potential error. There are many ways to implement an exception:

### Raise exception

```py
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

### Assert

```py
import sys
assert ('linux' in sys.platform), "This code runs on Linux only."
```

### Try - except

```py
try:
    linux_interaction()
except:
    pass
```

### try - except - else

```py
try:
    linux_interaction()
except AssertionError as error:
    print(error)
else:
    print('Executing the else clause.')
```

### try - except - else - finally

```py
try:
    linux_interaction()
except AssertionError as error:
    print(error)
else:
    try:
        with open('file.log') as file:
            read_data = file.read()
    except FileNotFoundError as fnf_error:
        print(fnf_error)
finally:
    print('Cleaning up, irrespective of any exceptions.')
```

## Things I want to know more about

How to automate document creating and editing using python