# SEALED CLASS IN C# 

### What is Sealed class in C#?
`Sealed classes are used to restrict the inheritance feature of object oriented programming. Once a class is defined as a sealed class, this class cannot be inherited. `

### Why Sealed Classes?

`We just saw how to create and use a sealed class in C#. The main purpose of a sealed class is to take away the inheritance feature from the class users so they cannot derive a class from it. One of the best usage of sealed classes is when you have a class with static members. For example, the Pens and Brushes classes of the System.Drawing namespace.`

`The Pens class represents the pens with standard colors. This class has only static members. For example, Pens.Blue represents a pen with blue color. Similarly, the Brushes class represents standard brushes. The Brushes.Blue represents a brush with blue color.`
 
`So when you're designing a class library and want to restrict your classes not to be derived by developers, you may want to use sealed classes.`

<img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.interviewsansar.com%2Fwhat-is-a-sealed-class-and-a-sealed-method-in-c%2F&psig=AOvVaw3lOQi1moEcCvotWmjt_zso&ust=1593354633331000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCOje4NyaouoCFQAAAAAdAAAAABAn" />
