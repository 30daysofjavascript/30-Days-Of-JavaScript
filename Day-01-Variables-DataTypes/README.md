# 🚀 Day 01 — Variables & Data Types

### 📚 30 Days of JavaScript: Beginner to Advanced

---

## 🧠 1. What is a Variable?

A **variable** is a named container used to store data in memory.
Think of it as a **labeled box** 📦 where you can keep values.

---

## 🛠️ Variable Declarations

JavaScript provides **3 ways** to declare variables:

```js
// VAR — ❌ Old way (avoid in modern JS)
var oldSchool = "I am var";

// LET — ✅ Use when value can change
let age = 25;
age = 26; // ✔ allowed

// CONST — ✅ Use when value should NOT change
const name = "Alice";
// name = "Bob"; ❌ Error!

console.log(oldSchool); // "I am var"
console.log(age);       // 26
console.log(name);      // "Alice"
```

---

## 🔢 2. Data Types in JavaScript

JavaScript has **8 data types**:

* **7 Primitive**
* **1 Object**

---

### 🔹 Primitive Types

#### 1. 📝 String (Text)

```js
let firstName = "John";
let lastName = 'Doe';
let greeting = `Hello, ${firstName}!`;

console.log(greeting); // "Hello, John!"
```

---

#### 2. 🔢 Number

```js
let intNum = 42;
let floatNum = 3.14;
let negative = -100;
let bigNum = 1_000_000;

console.log(typeof intNum); // "number"
```

**Special Values:**

```js
console.log(Infinity);
console.log(-Infinity);
console.log(NaN);
```

---

#### 3. 🔐 BigInt

```js
let bigInteger = 9007199254740991n;
console.log(typeof bigInteger); // "bigint"
```

---

#### 4. ✅ Boolean

```js
let isLoggedIn = true;
let hasAccount = false;

console.log(typeof isLoggedIn); // "boolean"
```

---

#### 5. ❓ Undefined

```js
let notAssigned;

console.log(notAssigned);        // undefined
console.log(typeof notAssigned); // "undefined"
```

---

#### 6. 🚫 Null

```js
let emptyValue = null;

console.log(emptyValue);        // null
console.log(typeof emptyValue); // "object" ⚠️ (JS bug)
```

---

#### 7. 🆔 Symbol

```js
let sym1 = Symbol("id");
let sym2 = Symbol("id");

console.log(sym1 === sym2); // false
```

---

### 🔸 Object Type

#### 🧩 Object

```js
let person = {
  name: "Alice",
  age: 30,
  isStudent: false
};

console.log(person);
console.log(person.name);
console.log(typeof person); // "object"
```

---

#### 🎨 Arrays (also objects)

```js
let colors = ["red", "green", "blue"];
console.log(typeof colors); // "object"
```

---

#### ⚙️ Functions (special objects)

```js
function sayHi() {
  return "Hi!";
}

console.log(typeof sayHi); // "function"
```

---

## 🔍 3. `typeof` Operator

Used to check the type of any value:

```js
console.log(typeof "hello");     // "string"
console.log(typeof 42);          // "number"
console.log(typeof true);        // "boolean"
console.log(typeof undefined);   // "undefined"
console.log(typeof null);        // "object" ⚠️
console.log(typeof {});          // "object"
console.log(typeof []);          // "object"
console.log(typeof function(){});// "function"
```

---

## 🔄 4. Type Conversion

---

### 🔁 Implicit Conversion (Type Coercion)

```js
console.log("5" + 3);   // "53"
console.log("5" - 3);   // 2
console.log(true + 1);  // 2
console.log(false + 1); // 1
console.log("" + false); // "false"
```

---

### 🎯 Explicit Conversion (Type Casting)

#### ➤ To Number

```js
let strNum = "42";

let converted = Number(strNum);
let parsed = parseInt("42px");
let float = parseFloat("3.14abc");

console.log(Number("abc"));      // NaN
console.log(Number(true));       // 1
console.log(Number(false));      // 0
console.log(Number(null));       // 0
console.log(Number(undefined));  // NaN
```

---

#### ➤ To String

```js
let num = 100;

let str1 = String(num);
let str2 = num.toString();
let str3 = num + "";
```

---

#### ➤ To Boolean

**Falsy Values ❌**

* `0`, `""`, `null`, `undefined`, `NaN`, `false`

**Truthy Values ✅**

* Everything else!

```js
console.log(Boolean(0));         // false
console.log(Boolean(""));        // false
console.log(Boolean(null));      // false
console.log(Boolean(undefined)); // false
console.log(Boolean(NaN));       // false

console.log(Boolean("hello"));   // true
console.log(Boolean(42));        // true
console.log(Boolean({}));        // true
console.log(Boolean([]));        // true
```

---

## 🏷️ 5. Variable Naming Rules

### ✅ Valid Names

```js
let myVariable = 1;
let _private = 2;
let $dollar = 3;
let camelCase = 4;
let PascalCase = 5;
```

---

### ❌ Invalid Names

```js
// let 1number = 1;
// let my-var = 1;
// let let = 1;
```

---

### 💡 Best Practice

Use **camelCase**:

```js
let userFirstName = "Alice";
let totalItemCount = 100;
```

---

## 📌 6. Constants & Best Practices

### 🔒 Use UPPERCASE for constants

```js
const MAX_RETRIES = 3;
const API_BASE_URL = "https://api.example.com";
const PI = 3.14159;
```

---

### ⚠️ Objects with `const`

```js
const user = { name: "Alice", age: 25 };

user.age = 26; // ✔ allowed
// user = {}; ❌ not allowed

console.log(user);
```

---

## 📝 Exercises

### 🧪 Exercise 1

Declare:

* `const` for your name
* `let` for your age
  Log both.

---

### 🧪 Exercise 2

Find `typeof`:

```js
"hello", 42, true, null, undefined, {}, [], function(){}
```

---

### 🧪 Exercise 3

What will this output?

```js
console.log("10" + 5);
console.log("10" - 5);
```

---

### 🧪 Exercise 4

Convert `"3.99"` to a number and add `1`.

---

### 🧪 Exercise 5

Identify **truthy** and **falsy** values:

```js
0, "0", "", " ", [], null, -1, NaN
```

---

## 🎉 Congrats!

You’ve completed **Day 01** 🎯
You're now familiar with:

* Variables
* Data Types
* Type Conversion
* Best Practices

👉 Next up: **Operators & Expressions**
