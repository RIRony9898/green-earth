## 1. Difference between `var`, `let`, and `const`

- **`var`**: Function-scoped, can be re-declared and updated, hoisted with `undefined`.
- **`let`**: Block-scoped, can be updated but not re-declared in the same scope.
- **`const`**: Block-scoped, cannot be re-assigned (but objects/arrays can be mutated).

**Example:**

```javascript
var x = 1;
let y = 2;
const z = 3;
```

## 2. Difference between `map()`, `forEach()`, and `filter()`

- **`map()`**: Returns a new array with transformed values.
- **`forEach()`**: Executes a function on each element, does not return anything.
- **`filter()`**: Returns a new array with elements that pass a condition.

**Example:**

```javascript
const arr = [1, 2, 3];
const mapped = arr.map((x) => x * 2); // [2, 4, 6]
arr.forEach((x) => console.log(x)); // Logs each element
const filtered = arr.filter((x) => x > 1); // [2, 3]
```

## 3. Arrow Functions in ES6

Arrow functions provide a shorter syntax for writing functions: `() => {}`.

- Do not bind their own `this`, `arguments`, or `super`.
- Ideal for callbacks and simple functions.

**Example:**

```javascript
const add = (a, b) => a + b;
console.log(add(2, 3)); // 5
```

## 4. Destructuring Assignment in ES6

Destructuring allows unpacking values from arrays or objects into variables.

**Examples:**

```javascript
// Array destructuring
const [a, b] = [1, 2]; // a = 1, b = 2

// Object destructuring
const { name, age } = { name: "Rahim", age: 25 };
```

## 5. Template Literals in ES6

Template literals are strings wrapped in backticks (\`).

- Support multi-line strings and interpolation with `${expression}`.
- Easier than concatenation with `+`.

**Example:**

```javascript
let name = "World";
console.log(`Hello, ${name}!`); // Output: Hello, World!
```
