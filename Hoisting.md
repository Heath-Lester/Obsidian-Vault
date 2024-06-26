https://www.w3schools.com/js/js_hoisting.asp

Hoisting is where functions, variables and classes are moved to the top of their scope before their execution.  This is a feature of [[JavaScript]]'s Just-In-Time (JIT) compilation due to the fact that [[JavaScript]] is an "interpreted" language as opposed to a compiled language. This is why you can successfully reference a function above or "before" where it declared.


```JS
console.log(greeting()); // "Hello there!"


function greeting() {
 return "Hello there!";
}
```



The reason hoisting works is because in the [[Execution Context]], or the creation phase, memory is allocated for the code that has not yet been parsed by the interpreter. The pointer for the member is created before it is read. For variables, the value in the creation phase is set to undefined until the execution phase where it is assigned to what is written.