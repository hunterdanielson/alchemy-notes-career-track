# Alchemy Reading Notes

- Advantages of TDD
    1. It makes you really consider what you want from the code.
    1. Spend less time in the debugger.
    1. Tells you whether your last change broke the code.
    - [Source](https://dzone.com/articles/20-benefits-of-test-driven-development)

- When to use beforeEach() & afterEach()
    1. beforeEach() can be used to run a function before each of the tests in the describe runs.
    1. afterEach() is used after each function in a describe.

- Downside of TDD
    - Requires some maintenance 
    - Upfront energy and time, can make coding feel slow

- Difference between ES6 Classes and Constructor/Prototype classes
    - The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance. [Source](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=Prototypes%20vs.,is%20itself%20an%20object%20instance.)

- Use case for static method
    - Often used as an alternative constructor, or frequently used in order to define helper and utility functions [Source](https://teamtreehouse.com/community/what-is-a-good-usecase-for-the-es2015-static-methods)
    - Static methods are called without instantiating their class and are also not callable when the class is instantiated [Source](https://medium.com/@yyang0903/static-objects-static-methods-in-es6-1c026dbb8bb1#:~:text=Static%20methods%20in%20Javascript%20are,static%20inside%20the%20class%20declaration.&text=As%20MDN%20describes%20it%2C%20%E2%80%9CStatic,when%20the%20class%20is%20instantiated.)

- Example of Higher Order function
    - Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them. In simple words, A Higher-Order function is a function that receives a function as an argument or returns the function as output.
    - Example of doubling each item in an array using map, a higher order function
    ```javascript
    const arr1 = [1, 2, 3];
    const arr2 = arr1.map(item => item * 2);
    console.log(arr2);
    ```

- Vocab terms
    - functional programming
        - Functional programming (often abbreviated FP) is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions. Contrast with object oriented programming, where application state is usually shared and colocated with methods in objects. [Source](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
    - pure function
        - Pure functions are functions that accept an input and returns a value without modifying any data outside its scope(Side Effects). Its output or return value must depend on the input/arguments and pure functions must return a value. [Source](https://blog.bitsrc.io/understanding-javascript-mutation-and-pure-functions-7231cc2180d3#:~:text=Pure%20functions%20are%20functions%20that,functions%20must%20return%20a%20value.)
    - higher-order function
        - Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them. [Source](https://blog.bitsrc.io/understanding-higher-order-functions-in-javascript-75461803bad#:~:text=Higher%2DOrder%20Functions,returns%20the%20function%20as%20output.)
    - immutable state
        - State that cannot be changed
    - object
        - Objects are containers for named values called properties or methods.
    - object-oriented programming (OOP)
        - Object-oriented programming (OOP) refers to a type of computer programming (software design) in which programmers define the data type of a data structure, and also the types of operations (functions) that can be applied to the data structure. [Source](https://www.webopedia.com/TERM/O/object_oriented_programming_OOP.html#:~:text=Object%2Doriented%20programming%20(OOP),applied%20to%20the%20data%20structure.)
    - class
        - A JavaScript class is a type of function. Classes are declared with the class keyword.
    - prototype
        - All JavaScript objects inherit properties and methods from a prototype.
    - super
        - The super keyword is used to access and call functions on an object's parent.
    - inheritance
        - Methods from base class are copied to derived class, inheritance is supported by using prototype object.
    - constructor
        - The constructor method is a special method for creating and initializing an object created within a class.
    - instance
        - A single instance of the object at runtime, like a made recipe from a cookbook, not the recipe itself
    - context
        - Context in JavaScript is related to objects. It refers to the object within the function being executed. this refers to the object that the function is executing in. this is determined by how a function is invoked. [Source](https://blog.pragmatists.com/the-many-faces-of-this-in-javascript-5f8be40df52e)
    - this
        - The value of this is determined by how a function is called (runtime binding). It can't be set by assignment during execution, and it may be different each time the function is called.
    - Test Driven Development (TDD)
        - Test Driven Development (TDD) is a process for writing software that provably satisfies the software requirements.
    - Jest
        - Jest is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase. [Jest](https://jestjs.io/)
    - Continuous Integration (CI)
        - Continuous Integration (CI) is the process of automating the build and testing of code every time a team member commits changes to version control. [Source](https://medium.com/@mosheezderman/how-to-set-up-ci-cd-pipeline-for-a-node-js-app-with-jenkins-c51581cc783c)
    - unit test
        - Unit tests only test a single part of your implementation. A unit. No dependencies or integrations, no framework specifics. [Source](https://www.freecodecamp.org/news/how-to-start-unit-testing-javascript/)