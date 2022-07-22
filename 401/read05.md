
# Linked Lists

## Why

When making applications there will be a need to cycle through linear data and access data that came before or after the current set you are on. An example is an image viewer. If you have an album of images you can view them by pressing a forward or back arrow. Another example is going from the current page to a previous page or the next page in a web browser.

## What

Cycling through lists is possible through a linked list. A linked list is a sequence of data elements connected together by links. The connection between lists is from a pointer.

## How

You can implement a linked list into your code by making a Node class and a Linked list class. You have to first instantiate the linked list class and then create the nodes by using the node class. See below for an example from tutorialspoint.com (https://www.tutorialspoint.com/python_data_structure/python_linked_lists.htm#:~:text=A%20linked%20list%20is%20a,lists%20in%20its%20standard%20library (Links to an external site.).)

```py
class Node:
   def __init__(self, dataval=None):
      self.dataval = dataval
      self.nextval = None

class SLinkedList:
   def __init__(self):
      self.headval = None

list1 = SLinkedList()
list1.headval = Node("Mon")
e2 = Node("Tue")
e3 = Node("Wed")
# Link first Node to second node
list1.headval.nextval = e2

# Link second Node to third node
e2.nextval = e3
```
