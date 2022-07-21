# Classes, Objects, Recursion

## Classes and Objects

Information from https://www.learnpython.org/en/Classes_and_Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects (learnpython).

How to access vaiables of an object:

```py
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable
```

init()

init is a function that is used to asign values in a class. This function is called when a class is initiated. See below for an example:

```py
class NumberHolder:

   def __init__(self, number):
       self.number = number
```

## Thinking Recursively

The basis of recursion is to solve a problem if it is a simple case. If it is not a simple case, divide it into subproblems and apply the same strategy to them. Here is an example of a recursive function from realpython.com:

```py
houses = ["Eric's house", "Kenny's house", "Kyle's house", "Stan's house"]

# Each function call represents an elf doing his work 
def deliver_presents_recursively(houses):
    # Worker elf doing his work
    if len(houses) == 1:
        house = houses[0]
        print("Delivering presents to", house)

    # Manager elf doing his work
    else:
        mid = len(houses) // 2
        first_half = houses[:mid]
        second_half = houses[mid:]

        # Divides his work among two elves
        deliver_presents_recursively(first_half)
        deliver_presents_recursively(second_half)
```

Recursive functions is a function which repeats a behavior by calling itself until a condition is met to return a result. The function can be broken down into two cases. The base case, which will return an immediate result if it can. The second is the recursive case, which will iterate through the base case until the desired condition is met. Here is a good example:

```py
# Calculates factorial of n
def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:
        return n * factorial_recursive(n-1)
```

## Pytest Fixtures and Coverage

Fixtures

Fixtures are objects that contain data that can be used on many different tests. You can define a fixture by using a decorator:

`@pytest.fixture`

Coverage

Coverage is a concept of ensuring that you have tested all possible paths of a function. There is a package that can help with this called pytest-cov from PyPi. This is invoked by calling pytest with a --cov option. This will provide a report for every part of the Python library that you used.


## Things I want to know more about

Testing: I still find myself running the code and using print outs to test rather than using the tests that are written. I am curious if I can combine this into my tests to make them more efficient. 