### 🧠 **Topic for Today**: Introduction to JavaScript + Variables

- - -

### 📘 **1\. What is JavaScript?**

JavaScript is a **programming language for the web**. It's used to make web pages interactive — think sliders, popups, games, form validation, etc. It runs in the browser, and also on the server using **Node.js**.

- - -

### 🧩 **2\. Variables in JavaScript**

Variables are **containers for storing data**. In JavaScript, we declare them using:

*   `var` (old, avoid it)
    
*   `let` (modern, block-scoped)
    
*   `const` (constant, cannot be reassigned)
    

#### 🔍 Example:

`let name = "Alice"; const age = 25;  console.log("My name is " + name + " and I am " + age + " years old.");`

- - -

### 🛠️ **3\. Mini Challenges (Practice Time!)**

#### ✅ Challenge 1:

Create two variables: `firstName` and `lastName`, and print `Hello, firstName lastName!`

#### ✅ Challenge 2:

Declare a constant `birthYear` and a variable `currentYear`, calculate the age, and print:

> "You are XX years old."

#### ✅ Challenge 3:

What happens if you try to reassign a `const` variable? Try this:

`const country = "India"; country = "USA"; // What happens here?`

- - -

### 🔗 **4\. Connecting the Dots**

Today you're learning the **foundation of all programming: variables**. Tomorrow, we’ll build on this by introducing **data types** (strings, numbers, booleans, etc.) and how JavaScript treats them.

- - -

### 🌀 **What is Scope in JavaScript?**

**Scope** determines **where** variables are accessible in your code.

There are 3 main types of scope in JavaScript:

#### 1\. **Global Scope**

Variables declared outside any block or function are _globally scoped_ — they can be accessed from **anywhere** in your code.

`let planet = "Earth";  function showPlanet() {   console.log(planet); // ✅ accessible }  showPlanet(); console.log(planet); // ✅ accessible`

- - -

#### 2\. **Function Scope**

Variables declared _inside_ a function using `var`, `let`, or `const` are only accessible **inside that function**.

`function greet() {   let message = "Hello";   console.log(message); // ✅ accessible }  greet(); // console.log(message); // ❌ Error: message is not defined`

- - -

#### 3\. **Block Scope** (only for `let` and `const`)

Variables declared inside `{ }` using `let` or `const` are only accessible **inside that block**.

`if (true) {   let mood = "happy";   const weather = "sunny";   console.log(mood);     // ✅   console.log(weather);  // ✅ }  // console.log(mood);    // ❌ Error // console.log(weather); // ❌ Error`

> ⚠️ `var` is **not** block-scoped — it's only function-scoped, which can lead to bugs. That's why `let` and `const` are preferred.

- - -

### 🧪 Try This!

`let greeting = "Hi";  function sayHi() {   let greeting = "Hello";   console.log("Inside function:", greeting); }  sayHi(); console.log("Outside function:", greeting);`

👉 Can you guess what the output will be? Try it out and let me know what you get!

- - -

### 🔁 **Block Scope Refresher**

A **block** is anything inside `{ }` — like in `if`, `for`, or `while` statements.

With `let` and `const`, variables declared inside a block **stay inside that block**. But `var` does **not** behave this way.

- - -

### ❗ Example: `var` is _not_ block-scoped

`if (true) {   var city = "New York";   let country = "USA";   const planet = "Earth"; }  console.log(city);    // ✅ New York (accessible outside block) console.log(country); // ❌ Error: country is not defined console.log(planet);  // ❌ Error: planet is not defined`

🔍 **Why?**

*   `var city` gets **hoisted** to the top of the _function_ or _global_ scope.
    
*   `let` and `const` stay **inside the block** (`if { }` in this case).
    

- - -

### 📦 Visual Breakdown

`{   var a = 1;   let b = 2;   const c = 3; }  console.log(a); // ✅ 1 console.log(b); // ❌ ReferenceError console.log(c); // ❌ ReferenceError`

> So `var` **leaks out** of the block — which is why it’s considered **not block-scoped**.

- - -

### ✅ Pro Tip: Always use `let` and `const`

Because `var` behaves this way, it can lead to **unexpected bugs**. Modern JavaScript best practice is to avoid `var` altogether unless you absolutely need it for legacy code.