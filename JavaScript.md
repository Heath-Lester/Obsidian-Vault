
<iframe width="100%" src="https://www.youtube-nocookie.com/embed/lkIFF4maKMU?si=io7q9kWSvVtqDWDO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" style="border-radius: 4px; aspect-ratio: 16/9" allowfullscreen></iframe>

## EYNTK about JS:

- High-level Language
- Standard Implementation is [[ECMAScript]]
- Is the only coding language that runs natively in the browser aside from [[WebAssembly]]
- Can run JS on a server using [[Node.js]] & Dino
- Scripting Language ([[Scripting vs Programming Language]])
- Interpreted Language ([[Interpreted vs Compiled Languages]])
- Vanilla JS tends to be used imperatively ([[Declarative vs Imperative Programming]])
- JS Frameworks allow declarative programming
- Uses the engine [[V8]]
- Used by HTML imported through a script element ([[Hypertext Markup Language]])
- Can use the `defer` attribute on script tags to wait until the document is fully loaded before executing the index.js file
- Dynamically Typed Language ([[Dynamic vs Static Typed]]) 
- The parser automatically add semicolons as an end of statement [[Delimiter]]
- Any value that is not one of its [[Primitive Data Types]] inherits from the object class
- Uninstantiated values are undefined
- Variables defined as `var` are defaulted to global scope
- Variables defined as `let` or `const` are hoisted to the top of the code block allowing them to be used before being declared ([[Hoisting]])
- Functions are objects with the additional capability to be called which allows them to be used as expressions ([[Expression vs Statement]])
- `This` refers to the global object or window when used globally or the object from where it is used
- Functions from an object can be bound to another object using: `objectName.bind(otherObject)`
- Functions can be defined using a function declaration or using arrow function syntax
- Arrow functions are anonymous
- When primitive types are passed into into a function, they are `passed by value`, meaning the value is copied into another variable as the argument.
- When objects are passed into a function, the are `passed by reference`, meaning the changes to the object within the function will change it everywhere else it is referenced.
- Objects can inherit properties from one another using the prototype chain.
- Every object has a private property that links to exactly one prototype.
- Prototype inheritance differs from class inheritance
- Memory is automatically Garbage Collected ([[Garbage Collection]])
- WeakMap and WeakSet are types that are optimized to have their properties garbage collected
- Has non-blocking event loops that is asynchronous by running in a different thread pool than the other
- Single Threaded, the thread it uses is called the "main" thread
- Can use callback functions ([[Callback Functions]])
- Can use NPM to import third-party modules ([[Node Package Manager]])
- Code is organized in [[Modules]]
- Can use [[Non-Blocking Event Loops]] to utilize multiple threads
- After the code base reaches a certain size, can greatly benefit from [[Module Bundlers]]
- Functions are able to use [[Higher Order Functions]]
- Has [[Signed Integers]]
- `.sort()` method converts input into strings and compares their Unicode character code at the first position. ([[Sorting]])


### Primitive Data Types

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures

|Type|`typeof` return value|Object wrapper|
|---|---|---|
|[Null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#null_type)|`"object"`|N/A|
|[Undefined](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#undefined_type)|`"undefined"`|N/A|
|[Boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#boolean_type)|`"boolean"`|[`Boolean`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)|
|[Number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#number_type)|`"number"`|[`Number`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)|
|[BigInt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#bigint_type)|`"bigint"`|[`BigInt`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt)|
|[String](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#string_type)|`"string"`|[`String`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)|
|[Symbol](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#symbol_type)|`"symbol"`|[`Symbol`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol)|


## The Weird Stuff

<iframe width="100%" src="https://www.youtube-nocookie.com/embed/Bv_5Zv5c-Ts?si=0JKmD3NwbORkub78" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>


