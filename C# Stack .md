# C# Stack

### What is Stack in C#?
`The stack is a special case collection which represents a last in first out (LIFO) concept. To first understand LIFO, let's take an example. Imagine a stack of books with each book kept on top of each other.`

`The concept of last in first out in the case of books means that only the top most book can be removed from the stack of books. It is not possible to remove a book from between, because then that would disturb the setting of the stack.`

`Hence in C#, the stack also works in the same way. Elements are added to the stack, one on the top of each other. The process of adding an element to the stack is called a push operation. To remove an element from a stack, you can also remove the top most element of the stack. This operation is known as pop.`

`Let's look at the operations available for the Stack collection in more detail.`

**`Declaration of the stack`**
**`A stack is created with the help of the Stack Data type. The keyword "new" is used to create an object of a Stack. The object is then assigned to the variable st.`**
<pre>Stack st = new Stack()</pre>

**Adding elements to the stack**
`The push method is used to add an element onto the stack. The general syntax of the statement is given below.`
<pre>Stack.push(element)</pre>

**Removing elements from the stack**
`The pop method is used to remove an element from the stack. The pop operation will return the topmost element of the stack. The general syntax of the statement is given below`

<pre> Stack.pop()</pre>

**Count**
`This property is used to get the number of items in the Stack. Below is the general syntax of this statement.`
<pre>Stack.Count</pre>

**Contains**
`This method is used to see if an element is present in the Stack. Below is the general syntax of this statement. The statement will return true if the element exists, else it will return the value false.`

<pre>Stack.Contains(element)</pre>

`Now let's see this working at a code level. All of the below-mentioned code will be written to our Console application. The code will be written to our Program.cs file.`

`In the below program, we will write the code to see how we can use the above-mentioned methods.`

**Example 1**
`In this example, we will see`

- `How a stack gets created.`
- `How to display the elements of the stack, and use the Count and Contain methods.`
