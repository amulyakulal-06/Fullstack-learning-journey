# Week 2: Core JavaScript Fundamentals

## 1. Variables & Scope (`var`, `let`, `const`)
- **`const`**: Cannot be reassigned, but properties of a `const` object or array can still be mutated.
- **`let`**: Block-scoped variable that can be reassigned.
- **`var`**: Function-scoped variable (legacy).
- **Temporal Dead Zone (TDZ)**: Accessing `let`/`const` variables before their declaration results in a `ReferenceError`.

## 2. Data Types & Type Checking
- **Primitives**: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`.
- **Reference Types**: `Object`, `Array`, `Function`.
- **Key Quirks**:
  - `typeof null` returns `"object"`.
  - Use `Array.isArray(value)` to accurately check for arrays.
- **Truthy & Falsy**:
  - Falsy values: `0`, `""`, `null`, `undefined`, `NaN`, `false`.
  - Truthy values: Non-empty strings, numbers other than zero, empty arrays `[]`, and empty objects `{}`.

## 3. Operators & Type Coercion
- **Arithmetic Coercion**: `10 + "5"` yields `"105"` (concatenation), whereas `10 - "5"` yields `5`.
- **Equality**: `==` performs type coercion, while `===` checks both value and type without coercion.
- **Logical Operators**:
  - `&&` returns the first falsy operand or the last operand if all are truthy.
  - `||` returns the first truthy operand or the last operand if all are falsy (useful for fallbacks).
  - `!!` converts any value to its explicit boolean equivalent.

## 4. Control Flow & Loops
- **Conditionals**: Avoid using assignment `=` inside `if` statements. Use `? :` (ternary operator) for concise conditional checks.
- **Loops**:
  - Use `for...of` for clean array iteration.
  - `break` exits the loop entirely, while `continue` skips to the next iteration.

## 5. Functions & Arrow Functions
- **Parameters vs Arguments**: Parameters are defined in the function declaration; arguments are the actual values passed during execution.
- **Implicit Return**: Arrow functions without curly braces automatically return the expression (e.g., `(a, b) => a + b`).
- **Callbacks**: Functions passed as arguments to other functions for delayed or deferred execution.

## 6. Arrays & Objects
- **Property Access**: Dot notation (`user.name`) vs Bracket notation (`user["name"]`).
- **Data Nesting**: Accessing nested properties via chaining (`user.address.city`).
- **Mutations**: Methods like `.push()` modify the original array instead of returning a new copy.

## 7. Higher-Order Array Methods
- **`.map()`**: Transforms each element in an array and returns a new array of the same length.
- **`.filter()`**: Returns a new array containing only elements that satisfy the condition.
- **`.find()`**: Returns the first element matching the condition, or `undefined` if no match is found.
- **Method Chaining**: Array methods can be chained together (e.g., `.filter().map()`).

## 8. Destructuring, Spread & Rest
- **Destructuring**: Extracting values from arrays or objects into distinct variables.
- **Spread Operator (`...`)**: Expands arrays or objects into individual elements (useful for shallow copying and immutability in React).
- **Rest Parameter (`...`)**: Collects remaining function arguments into a single array.

## 9. Value vs Reference Types
- **Primitives**: Passed and copied by value.
- **Objects/Arrays**: Passed and copied by reference.
- **Shallow Copy**: Using `{ ...obj }` or `[ ...arr ]` creates a top-level copy, but nested objects still share references.
