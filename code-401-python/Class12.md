# Stack and Queue
## Stack
A **Stack** is a linear data structure that follows the **LIFO** ***(Last-In-First-Out)*** principle. Stack has one end, whereas the Queue has two ends **(front and rear)**. It contains only one pointer top pointer pointing to the topmost element of the stack. Whenever an element is added in the stack, it is added on the top of the stack, and the element can be deleted only from the stack. In other words, a stack can be defined as a container in which insertion and deletion can be done from the one end known as the top of the stack.
* The following are some common operations implemented on the stack:

- push(): When we insert an element in a stack then the operation is known as a push. If the stack is full then the overflow condition occurs.
- pop(): When we delete an element from the stack, the operation is known as a pop. If the stack is empty means that no element exists in the stack, this state is known as an underflow state.
- isEmpty(): It determines whether the stack is empty or not.
- isFull(): It determines whether the stack is full or not.'
- peek(): It returns the element at the given position.
- count(): It returns the total number of elements available in a stack.
- change(): It changes the element at the given position.
- display(): It prints all the elements available in the stack.
## Queue
A **queue** is defined as a linear data structure that is open at both ends and the operations are performed in First In First Out (FIFO) order.

* We define a queue to be a list in which all additions to the list are made at one end, and all deletions from the list are made at the other end.  The element which is first pushed into the order, the operation is first performed on that.
### Example
A **Queue** is like a line waiting to purchase tickets, where the first person in line is the first person served.

- Position of the entry in a queue ready to be served, that is, the first entry that will be removed from the queue, is called the front of the queue(sometimes, head of the queue), similarly, the position of the last entry in the queue, that is, the one most recently added, is called the rear (or the tail) of the queue

- Variables used in this case are:
* Queue: the name of the array storing queue elements.
* Front: the index where the first element is stored in the array representing the queue.
* Rear: the index where the last element is stored in an array representing the queue.