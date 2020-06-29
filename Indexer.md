# Indexer in C#

### What is Indexer?
`An indexer is a special type of property that allows a class or a structure to be accessed like an array for its internal collection. C# allows us to define custom indexers, generic indexers, and also overload indexers.`

### Syntax :
<div class="dp-highlighter"> <div class="bar"></div> <ol start="1" class="dp-c"> <li class="alt"><span><span>&lt;modifier&gt;&nbsp;&lt;</span><span class="keyword">return</span><span>&nbsp;type&gt;&nbsp;</span><span class="keyword">this</span><span>&nbsp;[argument&nbsp;list]&nbsp;&nbsp;</span></span></li> <li class=""><span>{&nbsp;&nbsp;</span></li> <li class="alt"><span><span class="keyword">get</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>{&nbsp;&nbsp;</span></li> <li class="alt"><span><span class="comment">//&nbsp;your&nbsp;get&nbsp;block&nbsp;code</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>}&nbsp;&nbsp;</span></li> <li class="alt"><span><span class="keyword">set</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>{&nbsp;&nbsp;</span></li> <li class="alt"><span><span class="comment">//&nbsp;your&nbsp;set&nbsp;block&nbsp;code</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>}&nbsp;&nbsp;</span></li> <li class="alt"><span>}&nbsp;&nbsp;</span></li> </ol> </div>

**In the above code:**

**modifier**
`can be private, public, protected or internal.`
 
**return type**
`can be any valid C# types.`
 
**this**
`this is a special keyword in C# to indicate the object of the current class.`
 
**[argument list]**
`The formal-argument-list specifies the parameters of the indexer.`

### Important points to remember on indexers: 
- Indexers are always created with this keyword.
- Parameterized property are called indexer.
- Indexers are implemented through get and set accessors for the [ ] operator.
- ref and out parameter modifiers are not permitted in indexer.
- The formal parameter list of an indexer corresponds to that of a method and at least one parameter should be specified.
- Indexer is an instance member so can't be static but property can be static.
- Indexers are used on group of elements.
- Indexer is identified by its signature where as a property is identified it's name.
- Indexers are accessed using indexes where as properties are accessed by names.
- Indexer can be overloaded.
