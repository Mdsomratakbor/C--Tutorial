### 1. What is C#? Write its features?
`C# is an object-oriented programming language that was developed by Microsoft in 2000. It is supported by different operating systems. C# is the primary language that is used to create .Net software applications. It allows us to create Windows UI apps, backend services, controls, libraries, android apps, and even blockchain applications. C# works on the concept of classes and objects just like Java.`
**Some of the C# features are as follows:**

- Follows structured approach
- Parameters passing is easy
- Code can be compiled on a different platform
- Open-source
- Object-oriented
- Flexible and scalable 

### 2. Explain what are classes and objects in C#?

` C# is an object-oriented language and classes are its foundation. A class generally depicts the structure of data, how data is stored and managed within a program. A class has its own properties, methods, and other objects that define the class.`

`Objects are the real-world entity having some characteristics and is created using the class instance. These classes define the type of the defined object.`

`For example, if we consider a program that covers the object related to the book. We call the class a Book which has two properties: name and the author. In real programming, Vedas is an object and an instance of the class Book.`



### 3. What difference between Convert.toString and .toString() method?

`Here both the methods are used to convert the string but the basic difference between them is: "Convert" function handles NULLS, while "i.ToString()" does not it will throw a NULL reference exception error. So as good coding practice using "convert" is always safe.`

### 4. Describe the different C# classes in detail?

**here are 4 types of classes that we can use in C#:**

- **Static Class:** It is the type of class that cannot be instantiated, in other words, we cannot create an object of that class using the new keyword and the class members can be called directly using their class name.
- **Abstract Class:** Abstract classes are declared using the abstract keyword. Objects cannot be created for abstract classes. If you want to use it then it must be inherited in a subclass. You can easily define abstract or non-abstract methods within an Abstract class. The methods inside the abstract class can either have an implementation or no implementation.
- **Partial Class:** It is a type of class that allows dividing their properties, methods, and events into multiple source files, and at compile time these files are combined into a single class.
- **Sealed Class:**  One cannot inherit a sealed class from another class and restricts the class properties. Any access modifiers cannot be applied to the sealed class.

### 5. Explain different access modifiers in C#?

`These are the keywords that help to define the accessibility of class, member, and data type in the program. These keywords are used to restrict the use of some data manipulation done by other classes. There are 4 types of access modifiers- public, private, protected, and internal. These modifiers define 6 other accessibility levels when working together- public, protected, internal, protected internal, private, and private protected.`

### 6. How can you describe object-oriented concepts in detail?

`C# is an object-oriented programming language that supports 4 OOP concepts.`

- **Encapsulation:** defines the binding together code and the data and keeps it safe from any manipulation done by other programs and classes. It is a container that prevents code and data from being accessed by another program that is defined outside the container.
- **Abstraction:** this concept of object-oriented protects everything other than the relevant data about any created object in order to increase efficiency and security within the program.
- **Inheritance:** Inheritance is applied in such a way where one object uses the properties of another object. 
- **Polymorphism:** is a feature that allows one interface to act as a base class for other classes. This concept is often expressed as a "single interface but multiple actions". 

### 7.  Explain how code gets compiled in C#?

**It takes 4 steps to get a code to get compiled in C#. Below are the steps:**
- First, compile the source code in the managed code compatible with the C# compiler.
- Second, combine the above newly created code into assemblies.
- Third, load the CLR.
- Last, execute the assembly by CLR to generate the output.

### 8. What is break and continue statements in C#, explain?
**Below are the differences:**
<table>
<tbody>
<tr>
<td><strong>Break</strong></td>
<td><strong>Continue</strong></td>
</tr>
<tr>
<td>You can use break statements in both switch and loop (for, while, and do-while ) statements.</td>
<td>You can use continue statements only in the loop (for, while, do) statements.</td>
</tr>
<tr>
<td>The switch or loop statements terminate at the moment the break statement is executed and it ends abruptly from there.</td>
<td>You cannot make a continue statement terminate the loop, it carries on the loop to go to the next iteration level without executing the immediate next step.</td>
</tr>
<tr>
<td>The loop or switch exits immediately from the inner loop when the compiler encounters a break statement and comes out of the inner loop.</td>
<td>A continue that is placed inside a nested loop within a switch causes the next loop iteration.</td>
</tr>
</tbody>
</table>

### 9. What is the difference between public, static, and void?

`Public declared variables or methods are accessible anywhere in the application. Static declared variables or methods are globally accessible without creating an instance of the class. Static member are by default not globally accessible it depends upon the type of access modified used. The compiler stores the address of the method as the entry point and uses this information to begin execution before any objects are created. And Void is a type modifier that states that the method or variable does not return any value.`

### 10. How you can explain the use of ‘using’ statements in C# in detail?\

`The using statement is used to control the usage of one or more resources that are being used within the program. The resources are continuously consumed and released. The main function of this statement is to manage unused resources and release them automatically. Once the object is created which is using the resource and when you are done you make sure that the object’s dispose method is called to release the resources used by that object, this is where using statements works well.`

**For example:**
<pre style="background: #c5c5c5;">
using (MyResource abc = new MyResource())
{
 abc.program();
}
Gets translated to,
MyResource abc= new MyResource();
try
{
 myRes.program();
}
finally
{
 // Check for a null resource.
 if (abc!= null)
     // Call the object's Dispose method.
     ((IDisposable)abc).Dispose();
}
</pre>

### 11. Describe the C# dispose of the method in detail?

`The disposeof() method releases the unused resources by an object of the class. The unused resources like files, data connections, etc. This method is declared in the interface called IDisposable which is implemented by the class by defining the interface IDisposable body. Dispose method is not called automatically, the programmer has to implement it manually for the efficient usage of the resources.`

### 12. Explain in detail the finalize method in C#?

`The finalize () method is defined in the object class which is used for cleanup activities. This method is generally called by the garbage collector whenever the reference of any object is not used for a long time. Garbage collector frees that managed resources automatically but if you want to free the unused resources like filehandle, data connection, etc., then you have to implement the finalize method manually.`

### 13. How you can define the exception handling in C#?

`An exception is a raised problem that may occur during the execution of the program. Handling exceptions offers a simple way to pass the control within the program whenever an exception is raised. C# exceptions are handled by using 4 keywords and those are try, catch, finally, throw.`

**try:** `a raised exception finds a particular block of code to get handled. There is no limit on the number of catch blocks that you will use in your program to handle different types of exception raised.`

**catch:** `you can handle the raised exception within this catch block. You can mention the steps that you want to do to solve the error or you can ignore the error by suppressing it by the code.`

**Finally:** `irrespective of the error, if you still want some set of instructions to get displayed then you can use those statements within the finally block and it will display it on the screen.`

**throw:** `you can throw an exception using the throw statement. It will display the type of error you are getting.`

**Syntax :**

<pre>
try {
//exception handling starts with try block
} catch( ExceptionName ea1 ) {
   // errors are handled within the catch block
} catch( ExceptionName e2 ) {
   // more catch block
} catch( ExceptionName eN ) {
   // more catch block to handle multiple exception raised
} finally {
   // last block of the exception handling
} 
</pre>

### 14. Explain the concept of Destructor in detail. Explain it with an example?

`A destructor is a member that works just the opposite of the constructor. Unlike constructors, destructors mainly delete the object. The destructor name must match exactly with the class name just like a constructor. A destructor block always starts with the tilde (~) symbol.`

**Syntax : **
<pre>
~class_name()
{
//code
}
</pre>

**A destructor is called automatically:**

- when the program finishes its execution.
- Whenever a scope of the program ends that defines a local variable.
- Whenever you call the delete operator from your program.

### 15. Define method overloading with example?
`Method overloading allows programmers to use multiple methods but with the same name. Every defined method within a program can be differentiated on the basis of the number and the type of method arguments. It is a concept based on polymorphism.`

**Method overloading can be achieved by the following:**

- By changing the number of parameters in the given method
- By changing the order of parameters passed to a method
- By using different data types as the passed parameters

**For example:**
<pre>
public class Methodoveloading    
  {    
    public int sum(int a, int b)  //two int type Parameters method  
    {    
        return a + b;    
            }    
    public int sum(int a, int b,int c)  //three int type Parameters with same method same as above  
    {   
        return a + b+c;    
    }    
    public float sum(float a, float b,float c,float d)  //four float type Parameters with same method same as above two method 
    {    
        return a + b+c+d;    
    
    }    
  }   
</pre>

### 16. Explain the concept of boxing and unboxing of the value type and object type in C#?

**Boxing-** `is a process of converting a value type to an object type where value type is placed on the stack memory, and the object type is placed in the heap memory. This conversion is an implicit conversion and you can directly assign any value to an object, and C# will handle the rest of the conversion on its own.`

**Example :**

<pre>public void function()
{
Int a=111;
Object b=a; //implicit conversion
Console.WriteLine(b);
}</pre>

**Unboxing-** `it is the reverse process of the boxing process. It is a conversion of the object type to the value type and the value of the boxed object type placed on the heap memory which will be transferred to the value type which is placed on the stack. This conversion of the unboxing process has to be done explicitly.`

**Example :**

<pre>
public void function()
{
Object b=111;
Int a=(int)b; //implicit conversion
Console.WriteLine(a);
}
</pre>

### 17. Can multiple catch blocks be executed?
`No, Multiple catch blocks can't be executed. Once the proper catch code executed, the control is transferred to the finally block, and then the code that follows the finally block gets executed.`

### 18. What is Jagged Arrays?

`The Array which has elements of type array is called jagged Array. The elements can be of different dimensions and sizes. We can also call jagged Array as an Array of arrays.`
### 19. What is Managed or Unmanaged Code? 

- **Managed Code -** `The code, which is developed in .NET framework is known as managed code. This code is directly executed by CLR with the help of managed code execution. Any language that is written in .NET Framework is managed code.`

- **Unmanaged Code -** `The code, which is developed outside .NET framework is known as unmanaged code. Applications that do not run under the control of the CLR are said to be unmanaged, and certain languages such as C++ can be used to write such applications, which, for example, access low - level functions of the operating system. Background compatibility with the code of VB, ASP and COM are examples of unmanaged code.`

### 20. What is the difference between a struct and a class in C#? 

`Class and struct both are the user defined data type but have some major difference:`

**Struct :**

- `The struct is value type in C# and it inherits from System.Value Type.`
- `Struct is usually used for smaller amounts of data.`
- `Struct can't be inherited to other type.`
- `A structure can't be abstract.`
- `No need to create object by new keyword.`
- `Do not have permission to create any default constructo.`

**Class :**

- `The class is reference type in C# and it inherits from the System.Object Type.`
- `Classes are usually used for large amounts of data.`
- `Classes can be inherited to other class.`
- `A class can be abstract type.`
- `We can't use an object of a class with using new keyword.`
- `We can create a default constructor.`

### 21. Why can't you specify the accessibility modifier for methods inside the interface? 

`In an interface, we have virtual methods that do not have method definition. All the methods are there to be overridden in the derived class. That's why they all are public.`

### 22. Can you return multiple values from a function in C#? 

`Yes! Using output parameters. A return statement can be used for returning only one value from a function. However, using output parameters, you can return two values from a function.`

### 23. How to Return Multiple Values From a Function in C#?

**We can return multiple values from a function using the following 3 approaches:**

- `Reference parameters`
- `Output parameters`
- `Returning an Array`
- `Returning an object of class/struct type`
- `Returning a Tuple`

**Reference parameters :**

`Reference parameters also known as “ref” parameters are one of the most common and oldest way of returning multiple values from a function. As the name suggests, they are passed as reference to the function and after the function executes, the updated value of the passed reference variable is returned back to the calling method. It is important to note that reference parameters must be defined, initialized and assigned before they are passed to function else you may encounter a compile time error. Reference parameters are defined in the function signature as`

**public int MultipleReturns(int a, int b, out int max) {  
 if(a<b) {  
     max=a;  
     return b;  
 }  
 else{  
     max=b;  
     return a;  
 }  
}**

`In the above snippet we have defined the function signature using 2 integer parameters a & b and a ref parameter max. The function returns the minimum value between a & B and also assigns the maximum value to the output parameter. You can call the function as below`

<pre>
int a=10, b=20,max=0;  
int min = MultipleReturns(a,b,ref max);  
Console.WriteLine("Minimum Value: " + min);  
Console.WriteLine("Maximum Value: " + max); 
</pre>


**Cons of using ref parameters**
- `ref parameters do not work if you plan to use async/await functionality.`
- `Not very friendly in terms of reading the code.`


**Output Parameters**


`Output parameters also known as “out” parameters and are similar to reference parameters. As the name suggests, they are passed to the function as parameters and the calling method expects some values to be passed back in the parameter from the function. Output parameters are defined in the function signature as`



**public int MultipleReturns(int a, int b, out int max)  
{  
 if(a<b)  
 {  
     max=a;  
     return b;  
 }  
 else  
 {  
     max=b;  
     return a;  
 }  
}**


`In the above snippet we have defined the function signature using 2 integer parameters a & b and an out parameter max. The function returns the minimum value between a & B and also assigns the maximum value to the output parameter. If the function MultipleReturns() does not set any value to max variable inside the body, a compile time error generates. Hence, it is mandatory to assign values to out parameters in the function body. This is also to be noted that you cannot define 2 functions with same signature but having difference of only ref & out parameters, else the compiler will throw an error. You can call the function as below`


<pre>
int a=10, b=20,max=0;  
int min = MultipleReturns(a,b,out max);  
Console.WriteLine("Minimum Value: " + min);  
Console.WriteLine("Maximum Value: " + max);
</pre>

**Const of using out parameters**

- `out parameters do not work if you plan to use async/await functionality.`
- `Not very friendly in terms of reading the code.`


### 24: What is lambda expressions in C#?

`A lambda expression is an anonymous function that you can use to create delegates or expression tree types. By using lambda expressions, you can write local functions that can be passed as arguments or returned as the value of function calls. Lambda expressions are particularly helpful for writing LINQ query expressions.`

### 25: What is difference between constants and readonly?

`Constant variables are declared and initialized at compile time. The value can't be changed afterwards. Readonly is used only when we want to assign the value at run time.`


### 26: What is the difference between Interface and Abstract Class?

**There are some differences between Abstract Class and Interface which are listed below:**

- `A class can implement any number of interfaces but a subclass can at most use only one abstract class.`
- `An abstract class can have non-abstract methods (concrete methods) while in case of interface all the methods has to be abstract.`
- `An abstract class can declare or use any variables while an interface is not allowed to do so.`
- `In an abstract class all data member or functions are private by default while in interface all are public, we can't change them manually.`
- `In an abstract class we need to use abstract keyword to declare abstract methods while in an interface we don't need to use that.`
- `An abstract class can't be used for multiple inheritance while interface can be used as multiple inheritance.`
- `An abstract class use constructor while in an interface we don't have any type of constructor.`

### 27: Can we have only “try” block without “catch” block in C#?

`Yes we can have only try block without catch block but we have to have finally block.`

### 28: What interface should your data structure implement to make the "Where" method work?
<pre>
IEnumerable
</pre>

### 29: What are pointer types in C#?

**Pointer type** `variables store the memory address of another type. Pointers in C# have the same capabilities as the pointers in C or C++.`
