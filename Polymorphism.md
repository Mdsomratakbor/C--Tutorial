# Polymorphism in C#?

### What is Polymorphism in C#?

`Polymorphism is one of the primary pillars of object-oriented programming. It allows us to invoke derived class methods through a base class reference variable during runtime.`

`In the base class, the method is declared as virtual and in the derived class, we override the same method. The virtual keyword indicates that the method can be overridden in any derived class.`

`The word Polymorphism is derived from the Greek word, where Poly means many and morph means faces/ behaviors. So polymorphism means the ability to take more than one form.`

`The same function/ operator will show different behaviors when passed different types of values or the different number of values. So in the simple word we can say that behaving in different ways depending upon the input received is known as polymorphism i.e. whenever the input changes automatically the output or the behavior also changes.`

### What is polymorphism C# example?
`Dynamic / runtime polymorphism is also known as late binding. Here, the method name and the method signature (number of parameters and parameter type must be the same and may have a different implementation). Method overriding is an example of dynamic polymorphism. Method overriding can be done using inheritance.`

### What types of Polymorphism available in c#?

**There are two type of polymorphism :**
- Static polymorphism (Compile time polymorphism)
- Daynamic polymorphism (Run time polymorphism)

<img alt="polymorphism" class="" data-src="/UploadFile/ff2f08/understanding-polymorphism-in-C-Sharp/Images/ploymorphism.jpg" src="https://www.c-sharpcorner.com/UploadFile/ff2f08/understanding-polymorphism-in-C-Sharp/Images/ploymorphism.jpg">

### How many approach in implemention Polymorphism in a application ?
- Overloading
- Overriding
- Hiding

**Overloading is  three types**
- Method Overloading.
- Operator Overloading.
- Constructor Overloading.

### What is compile-time Polymorphism in C#?
`In the case of compile-time polymorphism, the object of class recognizes which method to be executed for a particular method call at the time of program compilation and binds the method call with method definition.
This happens in case of overloading because in case of overloading each method will have a different signature and basing on the method call we can easily recognize the method which matches the method signature.
It is also called as static polymorphism or early binding. Static polymorphism is achieved by using function overloading and operator overloading`

### What is Run-time Polymorphism in C#?
`In the case of runtime polymorphism for a given method call, we can recognize which method has to be executed exactly at runtime but not in compilation time because in case of overriding and hiding we have multiple methods with the same signature. So which method to be given preference and executed that is identified at runtime and binds the method call with its suitable method.
It is also called as dynamic polymorphism or late binding. Dynamic polymorphism is achieved by using function overriding.`

### What is Method Overloading in C#?
`Function overloading and method overloading terms are used interchangeably. Method overloading allows a class to have multiple methods with the same name but with a different signature. So in C# functions can be overloaded based on the number, type (int, float etc) and kind (Value, Ref or Out) of parameters.
The signature of a method consists of the name of the method and the type, kind (value, reference, or output) and the number of its formal parameters. The signature of a method does not include the return type and the params modifiers. So it is not possible to overload a method just based on the return type and params modifier.
A function overloading can be compared with person overloading. If a person has already some work to do and if we are assigning additional work to the person then the person will be overloaded.

In the same way, a function will have already some work to do and if we assign different work to the same function, then we say the function is overloaded. It is an approach of defining multiple methods with the same method name by changing the signature. Changing the signature means we can either change the no of parameters being passed to the method or type of parameters being passed to the method or order of parameters being passed to the function`

### When should we overload methods?
`To execute the same logic with different types of argument we should overload methods. For example to add two integers, two floats and two strings we should define three methods with the same name as shown in the below application`

### What are the advantages of using overloading OR what are the disadvantages if we define methods with a different name?
`If we overload the method, the user of our application gets comfort feeling in using the method with the impression that he/she calling one method by passing different types of values.`

`The best example for us is the “WriteLine()” method. It is an overloaded method, not a single method of taking different types of values.`

### When is a method considered as an overloaded method?
`If two methods have the same method name those methods are considered as overloaded methods.`

`Then the rule we should check is both methods must have different parameter types/list/order. But there is no rule on return type, non-accessibility modifier and accessibility modifier means overloading methods can have its own return type, non-accessibility modifier, and accessibility modifier because overloading methods are different methods`

### Can we overload methods in the same class?
`Yes, it is possible no CE, no RE. Methods can be overloaded in the same or in super and subclasses because overloaded methods are different methods.`

`But we can’t override the method in the same class it leads to CE: “method is already defined” because overriding methods are the same methods with a different implementation.`

### What is the function/method overriding?

`Redefining the superclass non-static method in the subclass with the same prototype is called method overriding. The overriding method is always executed from the current objects class.`

`In object-oriented programming method overriding is a language feature that allows a subclass to provide a specific implementation of a method that is already provided by one of its superclasses.`

`The implementation of the subclass overrides (replaces) the implementation of superclass methods. So the overridden method is always executed from the object whose object is stored in the reference variable. The superclass method is called the overridden method and the sub-class method is called the overriding method.`

### When must a method be overridden?
`If superclass method logic is not fulfilling sub-class business requirements, the subclass should override that method with required business logic. Usually, superclass methods are defined with generic logic which is common for all sub-classes.`

### How can we override a parent class method under child class?
`If we want to override a parent class method in its child class, first the method in the parent class must be declared as virtual by using the keyword virtual then only the child classes get the permission for overriding that method. Declaring the method as virtual is marking the method is overridable.`

`If the child class wants to override the parent class virtual method then the child class can do it with the help of the override modifier. But overriding the method under child class is not mandatory for the child classes. The Syntax is given below:`

`Class1:`
`Public virtual void show() //virtual function (overridable)`

`Class2: Class1`
`Public override void show() //overriding`

`Even if the method declared as virtual the child class may or may not override the method`

`In overriding, the parent class defines a method as virtual and gives it to child class to consume that method. So the child class now consume the method as it is or override that method as per the requirement of the child class. So overriding parent class virtual method under a child class is only optional.`
