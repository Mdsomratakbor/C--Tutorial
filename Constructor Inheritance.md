# Inheritance And Constructors In C#

### What is Constructor Inheritance in C#?

`Constructor Inheritance means just that, A derived class inherit base class constructor.  The syntax is as follows: struct B { B(int); // normal constructor 1 B(string); // normal constructor 2 }; struct D : B { using B::B; // inherit constructors from B }`
### Which Constructor is called first in inheritance in C#?
`Base Constructor gets called first. The Exception Constructor will be called, then your Child class constructor will be called.`

### Why Constructor is not Overriding?
`Constructor Overriding is never possible in Java. This is because, Constructor looks like a method but name should be as class name and no return value. Overriding means what we have declared in Super class, that exactly we have to declare in Sub class it is called Overriding`

### Can a constructor be final ?
`No, a constructor can't be made final. A final method cannot be overridden by any subclasses. As mentioned previously, the final modifier prevents a method from being modified in a subclass. ... In other words, constructors cannot be inherited in Java therefore, there is no need to write final before constructors`

### How to Inheritance base class constructor ?
` I want to manually call the constructor of the base class from the derived class constructor. We need to do this, using base keyword.only the default constructors of the base class will be called automatically, when we create an instance of the derived class, as we have seen in the first example. If we want to call parameterized constructor of the base class, you need to use a base keyword. One thing to note is, in inheritance from the derived class constructor, the base class constructor will be called either automatically or manually (using base keyword)`

`If we create a constructor in the derived class, no constructor in the base class compiler will flag an error. Thus, when you create a constructor in the derived class, you must create a constructor in the base class as well.`
