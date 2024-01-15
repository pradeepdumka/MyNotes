# MyNotes
# What is Hoisting?
>In JavaScript, hoisting is a behavior where **variable** and **function** declarations are **moved to the top of their containing scope during the compilation phase**, before the code is executed. 
>>This means that you can use a variable or a function in your code **before** it's  **declared** in the source code..
 
>* Variable Hoisting: .

    > console.log(x); // undefined .
    > var x = 5; .
    > console.log(x); // 5 .
  The variable x is hoisted to the top, so the first console.log doesn't throw an error, but the value is undefined until the actual assignment is reached.

>* Function Hoisting: .

    > sayHello(); // "Hello, World!".
      function sayHello() { .
        console.log("Hello, World!"); .
      } .
  The function declaration is hoisted to the top, so you can call the function before its actual declaration in the code .
  On the other hand, function expressions and variables declared with let or const are not hoisted in the same way: .

    > console.log(foo); // ReferenceError: foo is not defined .
      let foo = "bar"; .
    
   In the example above, using let or const instead of var would result in a ReferenceError because the entire variable is hoisted but not the initialization.

-----------------------------------------------------------------------------------------
# What is Closure?
>A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). . 
>>In other words, a closure gives you access to an outer function's scope from an inner function. .


     > function outerFunction() { .

        let outerVariable = 'I am from the outer function' .

        function innerFunction() { .

          console.log(outerVariable); .

        } .

        return innerFunction; .
      } .

>Call outerFunction and store the returned innerFunction in a variable. .

const closureExample = outerFunction(); .

>Call the innerFunction, which still has access to outerVariable. .
closureExample(); // Output: I am from the outer function .





