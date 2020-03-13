# Reading Notes 10   

[Reading-01](reading-notes.md  

**Error Handling & Debugging**  

- To find the source of an error, it helps to understand the process of a script and the way it is processed.  
- The way JS interprets the code is in one global context. Plus it goes through to each function and creates a new execution context.  
 _The stack_  
 - One line of code at a time is processed. When it comes across a function it then piles that code into the stack and processes it. This is on top of the function that it is already reading.   
_Errors_  
- Understanding an error can be tough.  
- When JS reads an error it stops at that point to try to interpret the error and then looks for exceptions for handling the code.  
 _Error objects_ can help you find where your mistakes are . We use tools in the browser to help identify and single out points of failure. The following are some types of errors that you may come across.  
    - Syntax Error
    - Reference
    - Eval Error  
    - URI Error  
    - Type Error  
    - Error  
    - NaN  
    - Range Error  

_Debugging_  

- Debugging can be a pain but if you use the tools that you have in the browser you can find the point of error. Usually this will tell you the type of error and the line it was found on. At times you may go back to the code to reference it and find that you may not feel like there is anything wrong. So you need to start looking at some of the syntax and other simple things. It can literally be something as simple as a typo or and extra space.