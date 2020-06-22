# CLR(Common Language Runtime) 

### What is CLR?
- Is the foundation of the .NET Framwork.
- Acts as an execution engine for the .NET Framework.
- Manages the execution of programs and provides a suitable environment for programs to run.
- Provides a multi-language execution enviroment.
**The following figure shows a more detailed look at the workingt of the CLR:**

<img alt="CLR Diagram" class="" data-src="/UploadFile/9582c9/what-is-common-language-runtime-in-C-Sharp/Images/CLR.jpg" src="https://www.c-sharpcorner.com/UploadFile/9582c9/what-is-common-language-runtime-in-C-Sharp/Images/CLR.jpg">

### When a code is executed for the first time?
- The CIL(COMMON INTERMEDIATE LANGUAGE) code is converted to a code native to the operation system.
- This is done at runtime by Just-In-Time(JIT) compiler present in the CLR.
- The CLR converts the CIL code to the machine language code.
- Once this is done, the code can be directly executed by the CPU(Central Processing Unit).
