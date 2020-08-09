# C# Queue

### What is Queue in C#?

`The Queue is a special case collection which represents a first in first out concept. Imagine a queue of people waiting for the bus. Normally, the first person who enters the queue will be the first person to enter the bus. Similarly, the last person to enter the queue will be the last person to enter into the bus. Elements are added to the queue, one on the top of each other.`

`The process of adding an element to the queue is the enqueuer operation. To remove an element from a queue, you can use the dequeuer operation. The operation in queues is similar to stack we saw previously.`

`Let's look at the operations available for the Queue collection in more detail.`

**Declaration of the Queue**

`The declaration of a Queue is provided below. A Queue is created with the help of the Queue Data type. The "new" keyword is used to create an object of a Queue. The object is then assigned to the variable qt.`

<pre>Queue qt = new Queue()</pre>

**Adding elements to the Queue**

`The enqueue method is used to add an element onto the queue. The general syntax of the statement is given below.`

<pre>Queue.enqueue(element)<pre>

**Removing elements from the queue**

`The dequeue method is used to remove an element from the queue. The dequeue operation will return the first element of the queue. The general syntax of the statement is given below`

<pre>Queue.dequeue()</pre>
