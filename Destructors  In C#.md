# DESTRUCTORS IN C# PROGRAMMING

### What is Destructors ?
`A destructor is a special method which has the same name as the class but starts with the character ~ before the class name and immediately de-allocates memory of objects that are no longer required.`

###  Characteristics of  Destructor

- Destructors (~) cannot be defined in Structs.

- Destructors (~) are only used with classes.

- Destructor cannot be inherited or overloaded.

- Destructor does not take modifiers or have parameters.

- Destructor cannot be called. They are invoked automatically.

- An instance becomes eligible for destruction when it is no longer possible for any code to use the instance.

- The Programmer has no control over when destructor is called because this is determined by Garbage Collector.

- Destructor is called when program exits.

- Execution of the destructor for the instance may occur at any time after the instance becomes eligible for destruction.

- Destructor implicitly calls Finalize on the base class of object.
