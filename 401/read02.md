# Testing and Modules

## In Tests We Trust

In the article Ana Paula Gomes talks about Test Driven Development(TDD) and how it can be useful to your code development. TDD is a strategy to write tests before you start writing the actual code for your project. She goes on to describe a method to structure a test which is the AAA convention:

- Arrange: organize the data needed to execute that piece of code
- Act: execute the code being tested
- Assert: Check the result to see if it is what you were expecting

The TDD cycle:

- Write a unit test
- Write a feature and make the test pass
- Refactor the code

## If name equals main

In the article written by Nirmi Shah and Nirmi describes using the following if statment `if __name__ =="main":` as a way to execute code only if the file was run directly and not imported.

## Recursion

Recursion is a process in which a function calls itself in order to accomplish its task. It has the potential to reduce the length of a project by providing an efficient iteration technique.

Properties of Recursion:

- Performing the same operation multiple times
- Trying smaller inputs to make the problem smaller
- A base condition is needed to stop the recursion  - preventing an infinite loop

Direct Recursion: a function that calls itself in the same function\
Indirect Recursion: a function that calls a different function in itself.

Below is an example from the article from geeksforgeeks.org:

```py
# A Python 3 program to
# demonstrate working of
# recursion
 
 
def printFun(test):
 
    if (test < 1):
        return
    else:
 
        print(test, end=" ")
        printFun(test-1)  # statement 2
        print(test, end=" ")
        return
 
# Driver Code
test = 3
printFun(test)
 
# This code is contributed by
# Smitha Dinesh Semwal
```

Recursion requires a stack, which is a series of functions dependent on a previous function and a finite answer.

## Things I want to know more about

Recursion: I am still quite confused about recursion and how it actually works
