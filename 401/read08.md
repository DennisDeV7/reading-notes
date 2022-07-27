# Ten Thousand 3

## List Comprehension

List comprehension is a powerful way to create lists in Python and the general syntax is as follows: `new_list = [expression for item in list]`

The list can be broken down:

1. The first item is the expression to be carried out
2. Second is the object to be worked on
3. Third is the iterable component

example:

`squares = [x**2 for x in range(10)]`

produces

[0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

## PySnooper

[c-sharpcorner.com](https://www.c-sharpcorner.com/article/inspecting-pysnooper/)

PySnooper is a convenient way to debug Python code. It is implemented simply by importing the library and adding a decorator to a feature of your code, example:

```py
import pysnooper
@pysnooper.snoop()
def printList(nums):
    for i in nums:
        print(i)

nums = [10,20,30,40]
print(printList(nums))
```

The report that is printed by using PySnooper as a lot of machine related data. You can remove that by adding normalize=True.

`(@pysnooper.snoop(normalize=True))`

## Things I want to learn more about

For list comprehension is nested loops possible?