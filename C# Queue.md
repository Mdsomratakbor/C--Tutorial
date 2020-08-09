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

<pre>Queue.enqueue(element)</pre>

**Removing elements from the queue**

`The dequeue method is used to remove an element from the queue. The dequeue operation will return the first element of the queue. The general syntax of the statement is given below`

<pre>Queue.dequeue()</pre>

**Count**

`This property is used to get the number of items in the queue. Below is the general syntax of this statement.`

<pre>Queue.Count</pre>

**Contains**

`This method is used to see if an element is present in the Queue. Below is the general syntax of this statement. The statement will return true if the element exists, else it will return the value false.`

<pre>Queue.Contains(element)</pre>

`Now, let's see this working at a code level. All of the below-mentioned code will be written to our Console application.`

`The code will be written to our Program.cs file. In the below program, we will write the code to see how we can use the above-mentioned methods.`

**Example**
`In this example, we will see how a queue gets created. Next, we will see how to display the elements of the queue, and use the Count and Contain methods.`

<img src="https://www.guru99.com/images/c-sharp-net/052616_1306_CCollection9.png"/>

<pre>using System;
using System.Collections;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace DemoApplication
{
 class Program
 {
  static void Main(string[] args)
  {
   Queue qt = new Queue();
   qt.Enqueue(1);
   qt.Enqueue(2);
   qt.Enqueue(3);

   foreach (Object obj in qt)
   {
    Console.WriteLine(obj);
   }
    Console.WriteLine(); Console.WriteLine();
    Console.WriteLine("The number of elements in the Queue " + qt.Count);
    Console.WriteLine("Does the Queue contain " + qt.Contains(3));
    Console.ReadKey();
   }
 }
} </pre>

**Output**

<img src="https://www.guru99.com/images/c-sharp-net/052616_1306_CCollection10.png"/>
