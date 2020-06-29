# Indexer in C#

### What is Indexer?
`An indexer is a special type of property that allows a class or a structure to be accessed like an array for its internal collection. C# allows us to define custom indexers, generic indexers, and also overload indexers.`

### About of Indexer?
- Indexer Concept is object act as an array.
- Indexer an object to be indexed in the same way as an array.
- Indexer modifier can be private, public, protected or internal.
- The return type can be any valid C# types.
- Indexers in C# must have at least one parameter. Else the compiler will generate a compilation error.

### Syntax :
<ol start="1" class="dp-c"> <li class="alt"><span><span class="keyword">this</span><span>&nbsp;[Parameter]&nbsp;&nbsp;</span></span></li> <li class=""><span>{&nbsp;&nbsp;</span></li> <li class="alt"><span>&nbsp;&nbsp;&nbsp;&nbsp;<span class="keyword">get</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;</span></li> <li class="alt"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="comment">//&nbsp;Get&nbsp;codes&nbsp;goes&nbsp;here</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>&nbsp;&nbsp;&nbsp;&nbsp;}&nbsp;&nbsp;</span></li> <li class="alt"><span>&nbsp;&nbsp;&nbsp;&nbsp;<span class="keyword">set</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;</span></li> <li class="alt"><span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="comment">//&nbsp;Set&nbsp;codes&nbsp;goes&nbsp;here</span><span>&nbsp;&nbsp;</span></span></li> <li class=""><span>&nbsp;&nbsp;&nbsp;&nbsp;}&nbsp;&nbsp;</span></li> <li class="alt"><span>}&nbsp;&nbsp;</span></li> </ol>
