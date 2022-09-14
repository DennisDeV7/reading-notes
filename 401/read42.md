# Pythonisms

## Dunder Methods

Dunder is a shortening of "double under" which represents functions in Python that have double underscores. These functions are predefined methods that use to add functionality to classes in Python. For example: `__init__` and `__str__` are commonly used. These methods are part of what is known as the Python data model which gives the Python language rich features natively to manipulate data.

Other dunders:

- __init__
- __str__
- __repr__
- __len__
- __getitem__
- __reversed__

## Iterators

The __iter__ and __next__ methods are the key to making Python objects iterable. 

example:

```py
repeater = Repeater('Hello')
for item in repeater:
    print(item)
```

what Python is doing in the background is actually this:

```py
repeater = Repeater('Hello')
iterator = repeater.__iter__()
while True:
    item = iterator.__next__()
    print(item)
```

## Generators

A generator is a function that returns an object which can be iterated over. Generators appear like normal functions, but do not behave the same. Calling a generator function does not run the function. It only creates and returns an object of the generator.

In the generator is a yield statement which allows a temporary suspension of the execution of the function and pass back values from it. 

## Things I want to learn more about