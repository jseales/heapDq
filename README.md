heapDq
======

provides the python class HeapDq which is uses heapq to implement a heap, and adds support for deletion of entries.

Heaps are a good choice of data structure whenever you are repeatedly finding minima in a collection of objects. 
Python's heapq is great, but there is no built in way to delete items from the heap in an efficient manner. 

The solution given here uses code on the doc page for heapq, wrapped in a class to make it easy to reuse in another project. 

In your project, import the HeapDq class:
>from heapDq import HeapDq

and then instantiate it:
>myHeap = HeapDq()

then you can add tasks with different priority levels, remove them, or pop from the heap to get the one with the
lowest-number (i.e. most important) priority.

>myHeap.add_task(2, priority = 7)

>myHeap.add_task(12, priority = 3)

>myHeap.remove_task(2)

>myHeap.pop_task()
