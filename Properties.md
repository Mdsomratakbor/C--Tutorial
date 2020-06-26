# Properties in C#

### What is Properties in c#?
`Properties enable a class to expose a public way of getting and setting values, while hiding implementation or verification code. A get property accessor is used to return the property value, and a set property accessor is used to assign a new value. These accessors can have different access levels`

<img class="" data-src="/article/understanding-properties-in-C-Sharp/Images/Properties in CSharp.jpg" alt="C# Properties" longdesc="Properties in C# and .NET" src="https://www.c-sharpcorner.com/article/understanding-properties-in-C-Sharp/Images/Properties%20in%20CSharp.jpg">

### What is the use of get and set properties in C#?
`In c#, properties will enable class variables to expose in public way using get and set accessors by hiding implementation details. In properties, a get accessor is used to return a property value and a set accessor is used to assign a new value.`

### What is the difference between field and property in C#?
`A field is a variable that is declared directly in a class or struct. ... A property is a member that provides a flexible mechanism to read, write, or compute the value of a private field. Properties can be used as if they are public data members, but they are actually special methods called accessors.`

### What is Readonly Property in C#?
`We can also create a read only property. Read only means that we can access the value of a property but we can't assign a value to it. When a property does not have a set accessor then it is a read only property.`

### What advantages of Property in C#?
`Answer: The advantages of using properties are: Before allowing a change in data, the properties can validate the data. Properties can evidently make visible of data on a class from where that data is actually retrieved such as a database.`

### In c#, the properties are categorized as three types, those are.
<table class="table table-striped table-bordered">
<thead>
<tr class="info"><th>Type</th><th>Description</th></tr>
</thead>
<tbody>
<tr>
<td>Read-Write</td>
<td>A property which contains a both <code>get</code> and <code>set</code> accessors, then we will call it as read-write property.</td>
</tr>
<tr>
<td>Read-Only</td>
<td>A property which contains only <code>get</code> accessor, then we will call it as a read-only property.</td>
</tr>
<tr>
<td>Write-Only</td>
<td>A property which contains only <code>set</code> accessor, then we will call it as write-only property.</td>
</tr>
</tbody>
</table>

<div class="codeBlock">
<p><span style="color: blue;">class</span><span> <span style="color: #2b91af;">User</span></span></p>
<p><span>{</span></p>
<p><span>&nbsp;&nbsp;&nbsp; <span style="color: blue;">private</span> <span style="color: blue;">string</span> name;</span></p>
<p><span>&nbsp;&nbsp;&nbsp; <span style="color: blue;">public</span> <span style="color: blue;">string</span> Name</span></p>
<p><span>&nbsp;&nbsp;&nbsp; {</span></p>
<p><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color: blue;">get</span> { <span style="color: blue;">return</span> name; }</span></p>
<p><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color: blue;">set</span> { name = <span style="color: blue;">value</span>; }</span></p>
<p><span>&nbsp;&nbsp;&nbsp; }</span></p>
<p><span>}</span></p>
</div>
