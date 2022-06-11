# Node

## Basic

1. **What are the advantages of using promises instead of callbacks?**
   - They are composable, unlike callbacks, therefore we can avoid callback hells
   - You can easily execute code with Promise.all when multiple responses are returned
   - You can wait for only one result from concurrent pending promises with the help of Promise.race
   - You can write asynchronous code in a synchronous manner if you use it in conjunction with async / await.
2. **Explain the concept of middleware in Node.js?**
   - A middleware is basically a function that will the receive the Request and Response objects, just like your route Handlers do. As a third argument you have another function which you should call once your middleware code completed. This means you can wait for asynchronous database or network operations to finish before proceeding to the next step.
3. **What is === operator? what is the Difference between "==" and "==="?**
   - Double equals (==) is a comparison operator, which transforms the operands having the same type before comparison.
   - === (Triple equals) is a strict equality comparison operator in JavaScript, which returns false for the values which are not of a similar type. This operator performs type casting for equality. If we compare 2 with “2” using ===, then it will return a false value.
4. **Explain the steps how “Control Flow" controls the functions calls?**
   - Control the order of execution
   - Collect data
   - Limit concurrency
   - Call the following step in the program.
5. **How many types of API functions are there in Node.js?**

   - Asynchronous, non-blocking functions - mostly I/O operations which can be fork out of the main loop.

   - Synchronous, blocking functions - mostly operations that influence the process running in the main loop.
