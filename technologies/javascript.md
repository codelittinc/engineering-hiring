# JavaScript questions

## Basic

1.  **What is an arrow function?**

    - Arrow functions have a few important distinctions in how they work that distinguish them from traditional functions, as well as a few syntactic enhancements. The biggest functional differences are that arrow functions do not have their own this binding or prototype and cannot be used as a constructor. Arrow functions can also be written as a more compact alternative to traditional functions, as they grant the ability to omit parentheses around parameters and add the concept of a concise function body with implicit return.

2.  **What is the difference between `let`, `const` and `var`?**
    * var: The scope of a var variable is functional scope, it can be updated and re-declared into the scope, it can be declared without initialization, It can be accessed without initialization as its default value is “undefined”.
    * let: The scope of a let variable is block scope, it can be updated but cannot be re-declared into the scope, it can be declared without initialization, it cannot be accessed without initialization, as it returns an error.
    * const: The scope of a const variable is block scope, it cannot be updated or re-declared into the scope, it cannot be declared without initialization, it cannot be accessed without initialization, as it cannot be declared without initialization.

3.  **What is the ES6 destructuring assignment?**
    * The destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects into distinct variables.

4.  **What is the spread operator and what it does in arrays, and in objects?**
    * The spread operator is denoted by three dots (…).
    * The spread operator unpacks elements of iterable objects such as arrays, sets, and maps into a list.
    * The rest paramter is also denoted by three dots (…). However, it packs the remaining arguments of a function into an array.
    * The spread operator can be used to clone an iterable object or merge iterable objects into one.

5.  **What are Promises, and when to use async/await?**
    * Promises in javascript are a way to handle asynchronous operations. It allows us to return a value from an asynchronous function like synchronous functions. When we return something from an asynchronous method it returns a promise which can be used to consume the final value when it is available in the future with the help of then() method or await inside of async functions. The syntax to create a promise is mentioned below.
    * Async/Await makes it easier to write promises. The keyword ‘async’ before a function makes the function return a promise, always. And the keyword await is used inside async functions, which makes the program wait until the Promise resolves.


6.  **What does `.map()` do? And `.reduce()`?**
    * map creates a new array by transforming every element in an array individually.
    * reduce, on the other hand, takes all of the elements in an array and reduces them into a single value.

7.  **What is the callback hell and how to avoid it?**
    * Callback hell is the situation in which we have complex nested callbacks. In this, each callback takes arguments that have been obtained as a result of previous callbacks. This kind of callback structure leads to lesser code readability and maintainability. We can avoid the callback hell with the help of Promises.

## Advanced

8. **What does the `static` keyword mean in a ES6 class?**
    * The static keyword defines a static method for the class. Static methods are not called on class instances. Instead, they are called on the class itself. These are usually utility functions, such as functions to create or clone objects.

9. **What does the `this` keyword mean in an ES6 arrow function, and what in a ES5 function?**
 * While in ES5 ‘this’ referred to the parent of the function, in ES6, arrow functions use lexical scoping — ‘this’ refers to it’s current surrounding scope and no further. Thus the inner function knew to bind to the inner function only, and not to the object’s method or the object itself.
10. **How would you make a deep clone of an object?**
    * Spread
    * Object.assign
    * JSON
    * Libraries

11. **What is a Generator function, and what does the `yield` keyword do?**
    * It's a function that can stop midway and then continue from where it stopped.
    * They're a special class of functions that simplify the task of writing iterators.
    * It's a function that produces a sequence of results instead of a single value, i.e you generate ​a series of values.
    * It's a function which returns an object on which you can call next(). Every invocation of next() will return an object of shape.
