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
