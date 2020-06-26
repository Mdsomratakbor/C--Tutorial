# Inheritance And Constructors In C#

### What is Constructor Inheritance in C#?

`Constructor Inheritance means just that, A derived class inherit base class constructor.  The syntax is as follows: struct B { B(int); // normal constructor 1 B(string); // normal constructor 2 }; struct D : B { using B::B; // inherit constructors from B }`
### Which Constructor is called first in inheritance in C#?
`Base Constructor gets called first. The Exception Constructor will be called, then your Child class constructor will be called.`

### Why Constructor is not Overriding?
`Constructor Overriding is never possible in Java. This is because, Constructor looks like a method but name should be as class name and no return value. Overriding means what we have declared in Super class, that exactly we have to declare in Sub class it is called Overriding`
