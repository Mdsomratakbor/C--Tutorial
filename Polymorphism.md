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
