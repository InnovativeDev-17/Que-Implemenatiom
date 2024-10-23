# Que-Implemenatiom
Queue Implementation
Objective:
To utilize exception handling in a queue implementation.

Overview:
Definition: A queue is a linear data structure that operates on the First In, First Out (FIFO) principle, meaning the first element added will be the first one removed. Queues are commonly used in various applications, including process scheduling, managing service requests, and handling asynchronous data.

Key Characteristics:

FIFO Structure: The first element added is the first to be removed.
Operations:
Enqueue: Adds an element to the rear of the queue.
Dequeue: Removes and returns the front element of the queue.
Peek/Front: Returns the front element without removing it.
isEmpty: Checks if the queue is empty.
isFull: Checks if the queue is full (applicable for fixed-size queues).
Algorithm:

Data Structure

Define a class Queue with:
An array arr of size MAX to store queue elements.
Two integers, front and rear, initialized to -1 to track the front and rear indices.
Operations

Insert(value):

If the queue is full (check with isFull()), print "Queue overflow! Cannot insert."
If the queue is empty (check with isEmpty()), set both front and rear to 0.
Otherwise, increment rear using circular indexing: rear = (rear + 1) % MAX.
Store value at arr[rear].
Print "Value inserted into queue."
DeleteElement():

If the queue is empty (check with isEmpty()), print "Queue underflow! Cannot delete."
Print the element at arr[front].
If front equals rear, set both front and rear to -1 (the queue becomes empty).
Otherwise, increment front using circular indexing: front = (front + 1) % MAX.
Display():

If the queue is empty (check with isEmpty()), print "Queue is empty."
Otherwise, iterate from front to rear, printing the elements in the queue, using circular indexing to handle wrap-around.
Main Function

Create an instance of Queue.
Repeat the following until the user chooses to exit:
Display a menu with options: Insert, Delete, Display, Exit.
Read the user choice.
Perform the corresponding operation based on the user's select
