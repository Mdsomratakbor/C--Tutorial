# STATIC CLASS IN C#

### What is static class?
`A C# static class is a class that can't be instantiated. The sole purpose of the class is to provide blueprints of its inherited classes. A static class is created using the "static" keyword in C#. A static class can contain static members only. You can‘t create an object for the static class.`

- If you declare any member as a non-static member, you will get an error. 
When you try to create an instance to the static class, it again generates a compile time error, because the static members can be accessed directly with its class name.
- The static keyword is used before the class keyword in a class definition to declare a static class.
- A static class members are accessed by the class name followed by the member name. 

