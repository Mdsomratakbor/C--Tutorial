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
