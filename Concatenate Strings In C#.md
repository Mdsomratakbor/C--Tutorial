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
