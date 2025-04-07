### 🧠 **Topic for Today**: Data Types in JavaScript

- - -

### 📘 **1\. What are Data Types?**

In JavaScript, **data types** define the kind of value a variable can hold. Understanding them helps you use variables properly and avoid bugs.

- - -

### 🧩 **2\. The 7 Primitive Data Types**

| Type | Example | Description |
| --- | --- | --- |
| `String` | `"Hello"` | Text |
| `Number` | `42`, `3.14` | Integers and floats |
| `Boolean` | `true`, `false` | True/false logic |
| `Undefined` | `let x;` | Declared but not assigned |
| `Null` | `let y = null;` | Intentional absence of a value |
| `Symbol` | `Symbol('id')` | Unique identifiers (advanced) |
| `BigInt` | `1234567890123456789n` | For large integers (rare use cases) |

- - -

### 🛠️ **3\. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:

Create the following variables and print their types using `typeof`:

`let username = "Sam";        // String let score = 85;              // Number let isOnline = true;         // Boolean let notAssigned;             // Undefined let emptyValue = null;       // Null  // Example output: typeof username => "string"`

#### ✅ Challenge 2:

Try this funny bug:

`console.log(typeof null); // What does this return? And why?`

_(Hint: It's a known JavaScript quirk.)_

- - -

### 🔗 **4\. Connecting the Dots**

Now that you know variables **can hold different types of data**, you'll start using them for **conditions and logic** soon (like: _if the user is online, show a green dot_). These types are the **building blocks of decision making** in your code.

---

### 🧠 **Topic for Today**: Operators and Expressions

---

### 📘 **1. What Are Operators?**

Operators let you **perform operations** on variables and values.

---

### 🔢 **2. Types of Operators in JavaScript**

#### ➕ Arithmetic Operators:
Used for math operations.

```javascript
let x = 10, y = 3;
console.log(x + y); // 13
console.log(x - y); // 7
console.log(x * y); // 30
console.log(x / y); // 3.333...
console.log(x % y); // 1 (remainder)
```

#### 🧠 Assignment Operators:
Used to assign values.

```javascript
let a = 5;
a += 2; // same as a = a + 2
a *= 3; // a = a * 3
```

#### 🔍 Comparison Operators:
Used to compare two values.

```javascript
console.log(10 > 5);   // true
console.log(10 < 5);   // false
console.log(10 == '10'); // true (loose comparison)
console.log(10 === '10'); // false (strict comparison)
```

#### ❗ Logical Operators:
Used in conditions.

```javascript
console.log(true && false); // false
console.log(true || false); // true
console.log(!true);         // false
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Create two variables: `num1 = 20`, `num2 = 5`
- Print the sum, difference, product, and remainder.

#### ✅ Challenge 2:
Use `==` and `===` to compare:
```javascript
let value1 = 100;
let value2 = "100";
```
Print the result and explain the difference.

#### ✅ Challenge 3:
Evaluate this logic:
```javascript
let isLoggedIn = true;
let hasProfile = false;

console.log(isLoggedIn && hasProfile); // ?
console.log(isLoggedIn || hasProfile); // ?
```

---

### 🔗 **4. Connecting the Dots**

Today’s topic is your entry to **writing logic**. With operators, you'll soon write `if` statements, loops, and full-blown decision flows in your apps.

---

### 🧠 **NEXT Topic**: Conditional Statements (`if`, `else`, `else if`)

---

### 📘 **1. What Are Conditional Statements?**

Conditional statements let you **run code based on conditions**. It's like telling your program:

> “**If** this is true, do this. **Otherwise**, do that.”

---

### 🔀 **2. Syntax Overview**

#### 🧪 `if` Statement:
```javascript
let age = 18;
if (age >= 18) {
  console.log("You can vote.");
}
```

#### ❓ `if...else`:
```javascript
let isLoggedIn = false;
if (isLoggedIn) {
  console.log("Welcome back!");
} else {
  console.log("Please log in.");
}
```

#### 🔄 `else if`:
```javascript
let score = 75;

if (score >= 90) {
  console.log("A grade");
} else if (score >= 75) {
  console.log("B grade");
} else {
  console.log("Try again");
}
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Write a program that checks a person’s age and prints:
- “Child” if age < 13
- “Teenager” if age between 13–19
- “Adult” if age >= 20

#### ✅ Challenge 2:
Check if a number is **positive**, **negative**, or **zero**.

#### ✅ Challenge 3:
You have two variables: `username` and `password`.  
- If both are non-empty, print “Login successful”
- Otherwise, print “Missing credentials”

---

### 🔗 **4. Connecting the Dots**

Now that you know **operators + data types**, you can use `if/else` to start building **real logic flows** like login forms, validations, and decision trees.

---

### 🧠 **Topic for Today**: `switch` Statement & Ternary Operator

---

### 📘 **1. What is a `switch` statement?**

A `switch` is an alternative to long `if...else if` chains when you're comparing the **same variable** against multiple values.

#### ✅ Syntax:
```javascript
let fruit = "apple";

switch (fruit) {
  case "apple":
    console.log("Apples are red or green.");
    break;
  case "banana":
    console.log("Bananas are yellow.");
    break;
  case "orange":
    console.log("Oranges are orange.");
    break;
  default:
    console.log("Unknown fruit.");
}
```

- `break` exits the `switch` after a match.  
- `default` runs if no case matches.

---

### ❓ **2. What is the Ternary Operator?**

A **short-hand for `if...else`**, often used when you just want to choose between two values.

#### ✅ Syntax:
```javascript
let age = 20;
let canVote = age >= 18 ? "Yes" : "No";
console.log(canVote); // "Yes"
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Use a `switch` statement to print the day of the week based on a number:
- `1` = Monday, `2` = Tuesday, ..., `7` = Sunday
- Anything else = "Invalid day"

#### ✅ Challenge 2:
Using ternary, check if a number is **even or odd** and print:
- `"Even"` if divisible by 2
- `"Odd"` otherwise

#### ✅ Challenge 3:
Use nested ternary to evaluate a score:
```javascript
let score = 85;
// "Excellent" if >= 90
// "Good" if 70–89
// "Needs improvement" if < 70
```

---

### 🔗 **4. Connecting the Dots**

With `switch` and ternary, you're learning **efficient logic flows** — especially helpful in UI apps and APIs for things like user roles, request types, or category filters.

---

### 🧠 **Topic for Today**: Arrays in JavaScript

---

### 📘 **1. What is an Array?**

An **array** is a list-like object that stores **multiple values in a single variable**.

```javascript
let fruits = ["apple", "banana", "orange"];
```

Each value in an array has an **index**, starting from `0`.

```javascript
console.log(fruits[0]); // "apple"
```

---

### ⚙️ **2. Common Array Operations**

#### 🆕 Create an Array:
```javascript
let numbers = [1, 2, 3, 4];
```

#### 📥 Add items:
```javascript
numbers.push(5);      // Add to end
numbers.unshift(0);   // Add to start
```

#### 🗑️ Remove items:
```javascript
numbers.pop();        // Remove from end
numbers.shift();      // Remove from start
```

#### 🔄 Access/Change items:
```javascript
numbers[1] = 100;
```

#### 🔍 Array length:
```javascript
console.log(numbers.length);
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Create an array of 5 favorite colors and:
- Print the first and last color
- Add one more color at the end
- Remove the first color

#### ✅ Challenge 2:
Create an array of numbers: `[10, 20, 30, 40, 50]`
- Change the third number to `99`
- Print the length of the array

#### ✅ Challenge 3:
Write a function `printAll` that takes an array and prints each item using a `for` loop.

---

### 🔗 **4. Connecting the Dots**

Arrays help store and manage **lists of things** – users, products, messages, anything. Soon you’ll loop through arrays to build dynamic UIs or process data from databases.

---

### 🧠 **Topic for Today**: Loops (`for`, `while`, `do...while`, and `for...of`)

---

### 📘 **1. Why Loops?**

Loops let you **repeat code** without writing it again.  
You use them to go through arrays, repeat actions, or perform checks multiple times.

---

### 🔄 **2. Loop Types in JS**

#### ✅ `for` loop (classic and powerful):

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

#### ✅ `while` loop (good when the end is unknown):

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

#### ✅ `do...while` loop (runs **at least once**):

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

#### ✅ `for...of` loop (perfect for arrays):

```javascript
let fruits = ["apple", "banana", "orange"];
for (let fruit of fruits) {
  console.log(fruit);
}
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Use a `for` loop to print numbers from 1 to 10.

#### ✅ Challenge 2:
Use a `while` loop to count down from 5 to 1.

#### ✅ Challenge 3:
Use a `for...of` loop to print all characters in this string:
```javascript
let name = "JavaScript";
```

---

### 🔗 **4. Connecting the Dots**

You’ve already used loops with arrays. Now you're learning to choose the **best loop for the job** — which is key when working with real data like lists of users, products, etc.

---

### 🧠 **Topic for Today**: Functions with Parameters & Return Values

---

### 📘 **1. What are Parameters and Return Values?**

- **Parameters** are placeholders in a function – they let your function accept input.
- A **return value** is the output the function gives back.

#### ✅ Basic Example:

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet("Alice")); // Hello, Alice!
```

- `name` is a parameter.
- The function returns a string using that parameter.

---

### ⚙️ **2. Why Use Them?**

- Functions with parameters are **reusable** for different inputs.
- Return values let you **store and use** the result of a function.

#### ✅ Example with Calculation:

```javascript
function add(x, y) {
  return x + y;
}

let sum = add(5, 7);
console.log(sum); // 12
```

---

### 🛠️ **3. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Create a function `multiply(a, b)` that returns the product of two numbers.

#### ✅ Challenge 2:
Create a function `isAdult(age)` that:
- Returns `true` if age >= 18
- Returns `false` otherwise

#### ✅ Challenge 3:
Create a function `getFullName(firstName, lastName)` that returns the full name as a single string.

---

### 🔗 **4. Connecting the Dots**

You’ve already written functions and loops. Now you’re combining them with **input/output** so they can be used anywhere — in APIs, buttons, calculators, login checks, etc.

---

Welcome to **Day 9** — today we unlock one of the most important parts of JavaScript: **Objects** 🧱

---

### 🧠 **Topic for Today**: Introduction to Objects in JavaScript

---

### 📘 **1. What is an Object?**

An **object** is a collection of **key-value pairs**. It lets you group related data together.

#### ✅ Example:
```javascript
const user = {
  name: "Alice",
  age: 25,
  isMember: true
};
```

- `name`, `age`, and `isMember` are **keys** (also called properties).
- `"Alice"`, `25`, and `true` are their **values**.

---

### 🛠️ **2. Accessing Object Data**

#### Dot notation:
```javascript
console.log(user.name); // Alice
```

#### Bracket notation:
```javascript
console.log(user["age"]); // 25
```

---

### ⚙️ **3. Updating and Adding Properties**

```javascript
user.age = 26;            // update
user.country = "India";   // add new
```

---

### 🧠 Bonus: Objects can even store functions (called **methods**):

```javascript
const person = {
  name: "John",
  greet: function() {
    return `Hello, I'm ${this.name}`;
  }
};

console.log(person.greet()); // Hello, I'm John
```

---

### 🛠️ **4. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:
Create an object `car` with properties:
- `brand`, `model`, `year`
- Print each property using dot notation

#### ✅ Challenge 2:
Add a new property `color` to the `car` object and change the `year` to a new value.

#### ✅ Challenge 3:
Create a method `getSummary` inside the `car` object that returns:
> `"Brand Model (Year) - Color"`

Call the method and log the result.

---

### 🔗 **5. Connecting the Dots**

Objects are everywhere — in user profiles, product listings, settings, API responses, and more. Once you master them, you’re on your way to working with **real structured data**.