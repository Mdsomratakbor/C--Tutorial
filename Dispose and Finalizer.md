### What is a Dispose method?
`In the context of C#, dispose is an object method invoked to execute code required for memory cleanup and release and reset unmanaged resources, such as file handles and database connections. ... The Dispose method, provided by the IDisposable interface, implements Dispose calls.`

<img src="https://techdifferences.com/wp-content/uploads/2016/07/dispose-and-finalize.jpg"/>
`Methods dispose() and finalize() are the methods of C# which are invoked to free the unmanaged resources held by an object. The dispose() method is defined inside the interface IDisposable whereas, the method finalize() is defined inside the class object. The main difference between dispose() and finalize() is that the method dispose() has to be explicitly invoked by the user whereas, the method finalize() is invoked by the garbage collector, just before the object is destroyed.`

`Let us study some other differences between them with the help of a comparison chart shown below.`
