# FUNCTIONS

1. **Function Declaration vs. Function Expression**:

   - **Declaration**: Defined with the `function` keyword, followed by a name, parameters, and a body. It is hoisted, meaning it can be called before it's defined in code.
     ```javascript
     function greet() {
       console.log("Hello!");
     }
     ```
   - **Expression**: A function defined within an expression, assigned to a variable. It's not hoisted.
     ```javascript
     const greet = function () {
       console.log("Hello!");
     };
     ```

2. **Passing Arguments**:

   - Pass arguments to a function by listing them inside the parentheses in the function call, separated by commas.
     ```javascript
     function sum(a, b) {
       return a + b;
     }
     sum(5, 3); // 8
     ```

3. **Return Statement**:

   - Exits the function and optionally passes a value back to the caller.
     ```javascript
     function sum(a, b) {
       return a + b;
     }
     ```

4. **Higher-Order Function**:

   - A function that takes another function as an argument or returns a function.
     ```javascript
     function higherOrder(fn) {
       fn();
     }
     higherOrder(function () {
       console.log("Hello!");
     });
     ```

5. **Function Scope vs. Block Scope**:

   - **Function Scope**: Variables declared within a function are not accessible outside of the function.
   - **Block Scope**: With `let` and `const`, variables are scoped to the block (`{}`) they are declared in, not just to function.
     ```javascript
     if (true) {
       var a = 5;
       let b = 10;
     }
     console.log(a); // 5
     console.log(b); // ReferenceError
     ```

6. **Arrow Functions**:

   - A concise syntax for writing functions. They do not have their own `this`, `arguments`, `super`, or `new.target`.
     ```javascript
     const sum = (a, b) => a + b;
     ```

7. **Recursive Function**:

   - A function that calls itself until a base condition is met.
     ```javascript
     function factorial(n) {
       return n < 2 ? 1 : n * factorial(n - 1);
     }
     ```

8. **Call, Apply, Bind**:

   - **call()**: Calls a function with a given `this` value and arguments provided one by one.
   - **apply()**: Similar to `call()`, but arguments are passed as an array.
   - **bind()**: Creates a new function with `this` bound to a specific object, with a given sequence of arguments preceding any provided when the new function is called.

9. **Default Parameter Values**:

   - Define default values for parameters in a function definition.
     ```javascript
     function greet(name = "Guest") {
       console.log("Hello, " + name);
     }
     ```

10. **Closures**:

    - A closure gives access to an outer function’s scope from an inner function.
      ```javascript
      function outer() {
        let count = 0;
        function inner() {
          count++;
          console.log(count);
        }
        return inner;
      }
      const counter = outer();
      counter(); // 1
      counter(); // 2
      ```

11. **Hoisting vs. Function Declarations**:

    - **Hoisting** is JavaScript's default behavior of moving declarations to the top. Function declarations are hoisted, but expressions are not.

12. **"arguments" Object**:

    - An array-like object accessible inside functions that contains the values of the arguments passed to that function.
      ```javascript
      function sum() {
        let total = 0;
        for (let i = 0; i < arguments.length; i++) {
          total += arguments[i];
        }
        return total;
      }
      ```

13. **Callback Function**:

    - A function passed into another function as an argument to be executed later. Commonly used for asynchronous operations.
      ```javascript
      function doSomething(callback) {
        callback();
      }
      doSomething(function () {
        console.log("Callback called!");
      });
      ```

14. **Named vs. Anonymous Function**:

    - **Named**: Has a name after the `function` keyword.
      ```javascript
      function greet() {
        console.log("Hello!");
      }
      ```
    - **Anonymous**: Does not have a name, often used as a function expression.
      ```javascript
      const greet = function () {
        console.log("Hello!");
      };
      ```

15. **Using "bind" to Bind "this"**:

    - Creates a new function that, when called, has its `this` keyword set to the provided value.

      ```javascript
      const obj = { name: "John" };
      function sayName() {
        console.log(this.name);
      }
      const boundSayName = sayName.bind(obj);
      boundSayName(); // John
      ```

16. **Function Hoisting**:

    - Function declarations are hoisted to the top of their scope, allowing them to be used before they are declared in the source code.

17. **Generator Function**:

    - Functions that can return multiple values over time, allowing the function to pause execution and resume later.
      ```javascript
      function* generator() {
        yield 1;
        yield 2;
      }
      const gen = generator(); // Does not execute immediately
      console.log(gen.next().value); // 1
      console.log(gen.next().value); // 2
      ```

18. **map, filter, reduce**:

    - **map()**: Creates a new array populated with the results of calling a provided function on every element in the calling array.
    - **filter()**: Creates a new array with all elements that pass the test implemented by the provided function.
    - **reduce()**: Executes a reducer function on each element of the array, resulting in a single output value.

19. **Rest Parameter**:

    - Allows a function to accept an indefinite number of arguments as an array.
      ```javascript
      function sum(...nums) {
        return nums.reduce((a, b) => a + b, 0);
      }
      ```

20. **Pure vs. Impure Functions**:

    - **Pure Function**: Given the same inputs, always returns the same output and has no side effects.
    - **Impure Function**: Its output may depend on external state or may cause side effects.

21. **Function Composition**:
    - The process of combining two or more functions to produce a new function. Composing functions together is a common technique in functional programming.
      ```javascript
      const add5 = (x) => x + 5;
      const multiply2 = (x) => x * 2;
      const multiplyThenAdd5 = (x) => add5(multiply2(x));
      console.log(multiplyThenAdd5(3)); // (3 * 2) + 5 = 11
      ```
