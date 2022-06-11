# JavaScript questions

## Basic

1.  **What is an arrow function?**

    - Arrow functions have a few important distinctions in how they work that distinguish them from traditional functions, as well as a few syntactic enhancements. The biggest functional differences are that arrow functions do not have their own this binding or prototype and cannot be used as a constructor. Arrow functions can also be written as a more compact alternative to traditional functions, as they grant the ability to omit parentheses around parameters and add the concept of a concise function body with implicit return.

2.  **What is the difference between `let`, `const` and `var`?**
    * var: The scope of a var variable is functional scope, it can be updated and re-declared into the scope, it can be declared without initialization, It can be accessed without initialization as its default value is “undefined”.
    * let: The scope of a let variable is block scope, it can be updated but cannot be re-declared into the scope, it can be declared without initialization, it cannot be accessed without initialization, as it returns an error.
    * const: The scope of a const variable is block scope, it cannot be updated or re-declared into the scope, it cannot be declared without initialization, it cannot be accessed without initialization, as it cannot be declared without initialization.

3.  **What is the ES6 destructuring assignment?**
4.  **What is the spread operator and what it does in arrays, and in objects?**
5.  **What are Promises, and when to use async/await?**
6.  **What does `.map()` do? And `.reduce()`?**
7.  **What is the callback hell and how to avoid it?**

## Advanced

8. **What does the `static` keyword mean in a ES6 class?**
9. **What does the `this` keyword mean in an ES6 arrow function, and what in a ES5 function?**
10. **How would you make a deep clone of an object?**
11. **What is a Generator function, and what does the `yield` keyword do?**
