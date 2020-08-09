# 6 Effective Ways To Concatenate Strings In C#

<img src="https://www.c-sharpcorner.com/article/6-effective-ways-to-concatenate-strings-in-c-sharp-and-net-core/Images/6-Effective-Ways-Concatenate-String-Csharp.jpg"/>

### Here are the 6 ways to concatenate strings in C#. 
- `Using + operator`
- `String Interpolation`
- `String.Concatenate() method`
- `String.Join() method`
- `String.Format() method`
- `StringBuilder.Append() method`

**1. Concatenate String Using + Operator**
`The simplest method of adding two strings in C# is using + or += operators.`

`The following code example in Listing 1 concatenates two strings and a special character.`

<pre>// Simple string concatenation     
Console.WriteLine("Hello" + " " + "String " + "!");</pre>

**2. String Interpolation in C#**
`String interpolation is a method to concatenate variables as a part of a string. Syntax of string interpolation starts with a ‘$’ symbol and code variables are within a bracket {}.`

`The following code example in Listing 2 concatenates strings to create a longer string.`

<pre>// String Interpolation    
string author = "Mahesh Chand";    
string book = "C# Programming";    
// Use string interpolation to concatenate strings.    
string bookAuthor = $"{author} is the author of {book}.";    
Console.WriteLine(bookAuthor);
</pre>

**3. Concatenate string using String.Concate method in C#**
`String.Concate() method concatenates two strings, two objects, and two arrays of strings and combinations of them. `

`The following code example in Listing 3 concats two strings.`
  
  <pre>
// String.Concat method    
string fName = "Mahesh";    
string lName = "Chand";    
string Name = string.Concat(fName, lName); 
  </pre>
**4. Concatenate string using String.Join method**
`String.Join() method concatenates the elements of an array or the members of a collection, using the specified separator between each element or member. The array or the collection can be any data type including numbers and objects. String.Join method also allows you to concatenate string items of any data types with a range.` 

`The following code example in Listing 7 concatenates an array of int values to a string separated by a comma and space.`

<pre>// Using String.Join(String, String[])    
int[] intArray = { 1, 3, 5, 7, 9 };    
String seperator = ", ";    
string result = "Int, ";    
result += String.Join(seperator, intArray);    
Console.WriteLine($"Result: {result}"); </pre>

**5. Concatenate string using String.Format method in C#**

`String.Format() method formats strings in a desired format by inserting objects and variables with specified space and alignments into another strings and literals. It is also often used to format strings into specific formats.`

`String.Format() method has 8 overloaded formats to provide options to format various objects and variables that allow various variables to format strings.` 

`Note: In C# 6 or later versions, String Interpolation is recommended. Sting interpolation is more flexible and more readable and can achieve the same results without composite formatting.`

**Insert a single object in a string** 

`We can insert one or more objects and expressions in a string at a specified position using the String.Format method. The position in the string starts at the 0th index.` 

`For single object formatting, the first argument is the format and the second argument is the value of the object. The object is replaced at the {0} position in the string.` 

**`public static string Format (string format, object arg0);`**
`The following code example in Listing 9 inserts a DateTime object in an existing string format.`

<pre>
/* *** Simple String.Format **/    
string date = String.Format("Today's date is {0}", DateTime.Now);    
Console.WriteLine(date);
</pre>

`As you can see from the above code example, {0} is at the last portion in the string and the second argument is a DateTime.Now. In this case, string portion {0} will be replaced by the value of DateTime.Now in the string. Figure 2 is the result of the above code. `

<img src="https://www.c-sharpcorner.com/article/6-effective-ways-to-concatenate-strings-in-c-sharp-and-net-core/Images/InsertStringObjectCSharp.jpg" />

**6. StringBuilder.Append method in C#**
`String object in .NET is immutable. What does that mean? It means every time you use one of the String class methods, no matter if you use the same variable or a new variable, a new string object is created in memory. That means, a memory space is allocated for that new string in your computer memory. The more string methods you use to manipulate strings, the more memory space will be allocated in memory. That means in a string manipulation heavy code, if strings are not used wisely, it could lead to some serious app performance issues. `

`.NET provides the System.Text.StringBuilder class that can be used to modify strings without creating new string objects. StringBuilder is highly recommended if you have more than a few hundred string concatenation operations in your code. StringBuilder is not recommended for a few string concatenation operations. `

`StringBuilder class is defined in the System.Text namespace. You must either import this namespace in your class or reference is direct in the object instantiation.`

`using System.Text;`
 
S`tringBuilder constructor can take a string or can be no arguments. 
The following code snippet creates a StringBuilder and appends 3 strings. `

<pre>System.Text.StringBuilder builder = new System.Text.StringBuilder("Mahesh Chand");    
builder.Append(", ");    
builder.Append("Chris Love");    
builder.Append(", Praveen Kumar");</pre>

