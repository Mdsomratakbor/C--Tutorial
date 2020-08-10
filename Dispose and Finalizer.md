### What is a Dispose method?
`In the context of C#, dispose is an object method invoked to execute code required for memory cleanup and release and reset unmanaged resources, such as file handles and database connections. ... The Dispose method, provided by the IDisposable interface, implements Dispose calls.`

<img src="https://techdifferences.com/wp-content/uploads/2016/07/dispose-and-finalize.jpg"/>
`Methods dispose() and finalize() are the methods of C# which are invoked to free the unmanaged resources held by an object. The dispose() method is defined inside the interface IDisposable whereas, the method finalize() is defined inside the class object. The main difference between dispose() and finalize() is that the method dispose() has to be explicitly invoked by the user whereas, the method finalize() is invoked by the garbage collector, just before the object is destroyed.`

`Let us study some other differences between them with the help of a comparison chart shown below.`

### Difference Between Dispose and Finalizer?
<table id="tablepress-65" class="tablepress tablepress-id-65">
<thead>
<tr class="row-1 odd">
	<th class="column-1">Basis for Comparison</th><th class="column-2">dispose( )</th><th class="column-3">finalize( )</th>
</tr>
</thead>
<tbody class="row-hover">
<tr class="row-2 even">
	<td class="column-1">Defined</td><td class="column-2">The method dispose( ) is defined in the interface IDisposable interface.</td><td class="column-3">The method finalize( ) id defined in java.lang.object class.</td>
</tr>
<tr class="row-3 odd">
	<td class="column-1">Syntax</td><td class="column-2">public void Dispose( ){<br>
// Dispose code here<br>
}</td><td class="column-3">protected void finalize( ){<br>
// finalization code here<br>
}</td>
</tr>
<tr class="row-4 even">
	<td class="column-1">Invoked </td><td class="column-2">The method dispose( ) is invoked by the user.</td><td class="column-3">The method finalize( ) is invoked by the garbage collector.</td>
</tr>
<tr class="row-5 odd">
	<td class="column-1">Purpose</td><td class="column-2">Method dispose( ) is used to free unmanaged resources whenever it is invoked.</td><td class="column-3">Method finalize( ) is used to free unmanaged resources before the object is destroyed.</td>
</tr>
<tr class="row-6 even">
	<td class="column-1">Implementation</td><td class="column-2">The method dispose( ) is to be implemented whenever there is a close( ) method.</td><td class="column-3">The method finalize( ) is to be implemented for unmanaged resources.</td>
</tr>
<tr class="row-7 odd">
	<td class="column-1">Access specifier</td><td class="column-2">The method dispose( ) is declared as public.</td><td class="column-3">The method finalize( ) is declared as private.</td>
</tr>
<tr class="row-8 even">
	<td class="column-1">Action </td><td class="column-2">The method dispose( ) is faster and instantly disposes an object.</td><td class="column-3">The method finalize is slower as compared to dispose</td>
</tr>
<tr class="row-9 odd">
	<td class="column-1">Performance</td><td class="column-2">The method disposes( ) performs the instantaneous action hence, does not effect the performance of websites. </td><td class="column-3">The method finalize( ) being slower affects the performance of the websites.</td>
</tr>
</tbody>
</table>
