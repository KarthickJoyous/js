## **📘 Day 11: JavaScript – Functions (Advanced Concepts)**

### 🚀 Topic: Function Expressions, Arrow Functions & Higher-Order Functions

---

### 🧠 1. Brief Explanation:

You've already seen basic functions. Today, let's go deeper with **function expressions**, **arrow functions**, and **higher-order functions**.

#### 🟩 Function Expression
A function assigned to a variable.

```javascript
const greet = function(name) {
  return `Hello, ${name}`;
};
```

#### 🟦 Arrow Function
A shorter syntax for writing functions.

```javascript
const greet = (name) => `Hello, ${name}`;
```

#### 🟨 Higher-Order Function
A function that takes another function as an argument or returns a function.

```javascript
function shout(callback) {
  return function(word) {
    return callback(word.toUpperCase());
  };
}

const say = (msg) => `You said: ${msg}`;
const loudSay = shout(say);
console.log(loudSay("hello")); // You said: HELLO
```

---

### 🧪 2. Mini Challenges:

✅ **Challenge 1:** Convert this function to an arrow function:
```javascript
function multiply(a, b) {
  return a * b;
}
```

✅ **Challenge 2:** Write a function `doTwice` that takes a function as a parameter and calls it twice.

✅ **Challenge 3:** Create a higher-order function that returns another function to greet with a custom prefix (e.g., “Hi”, “Hey”, “Yo”).

---

### 🔗 3. Connect with Previous Topics:

- You now know how to **declare variables** (Day 1–2), use **conditions and loops** (Day 5–6), and write **basic functions** (Day 10).
- Today expands on that by showing how **functions can be treated like values**, allowing powerful and reusable code patterns.

---

## **📘JavaScript – Array Methods (Map, Filter, Reduce)**

### 🚀 Topic: Transforming and Processing Arrays

---

### 🧠 1. Brief Explanation:

These three **powerful array methods** help you transform, filter, and summarize data **without writing explicit loops**.

---

### 🔧 2. Method Breakdown:

#### ✅ `map()` – transforms each element and returns a new array
```javascript
const nums = [1, 2, 3];
const squares = nums.map(n => n * n);
console.log(squares); // [1, 4, 9]
```

#### ✅ `filter()` – filters out elements that don’t match a condition
```javascript
const ages = [16, 21, 18, 25];
const adults = ages.filter(age => age >= 18);
console.log(adults); // [21, 18, 25]
```

#### ✅ `reduce()` – reduces the array to a single value (sum, max, etc.)
```javascript
const prices = [10, 20, 30];
const total = prices.reduce((acc, val) => acc + val, 0);
console.log(total); // 60
```

---

### 🧪 3. Mini Challenges:

✅ **Challenge 1:**  
Use `map()` to convert an array of strings to uppercase.  
```js
['a', 'b', 'c'] → ['A', 'B', 'C']
```

✅ **Challenge 2:**  
Use `filter()` to keep only even numbers from this array:  
```js
[1, 2, 3, 4, 5, 6]
```

✅ **Challenge 3:**  
Use `reduce()` to find the **product** of all numbers in this array:  
```js
[2, 3, 4] → 24
```

---

### 🔗 4. Connection to Previous Days:

- You already learned about **arrays** and **looping**. These methods are modern alternatives that make your code **cleaner** and **more expressive**.
- They’re widely used in real-world apps, especially when handling data from APIs or databases (hint: that’s coming soon with Node.js + MySQL 👀).

---