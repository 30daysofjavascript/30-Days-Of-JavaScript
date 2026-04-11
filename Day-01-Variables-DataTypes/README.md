# 🚀 Day 01 — Variables & Data Types

### 📚 30 Days of JavaScript: Beginner to Advanced

# 📘 JavaScript Variables (Full Guide)

---

## 🧠 Introduction

Variables in JavaScript are used to **store data values**.
Think of a variable as a **container** that holds information which can be used and modified later.

---

## 📦 What is a Variable?

A variable is:

* A **named storage** for data
* Used to store values like numbers, text, objects, etc.

### ✅ Example:

```js
let name = "Rahul";
```

**Breakdown:**

* `let` → keyword
* `name` → variable name
* `"Rahul"` → value

---

## 🔑 Ways to Declare Variables

JavaScript provides **3 main keywords**:

---

### 1️⃣ `var` (Old way)

```js
var age = 25;
```

📌 **Features:**

* Function-scoped
* Can be re-declared
* Can be updated

```js
var age = 25;
var age = 30; // ✅ allowed
```

⚠️ **Issues:**

* Can cause bugs
* Affected by hoisting
* Not recommended in modern JS

---

### 2️⃣ `let` (Modern & Recommended)

```js
let city = "Delhi";
```

📌 **Features:**

* Block-scoped
* Cannot be re-declared in same scope
* Can be updated

```js
let city = "Delhi";
city = "Mumbai"; // ✅ allowed
```

❌ **Not allowed:**

```js
let city = "Delhi";
let city = "Mumbai"; // ❌ error
```

---

### 3️⃣ `const` (Constant values)

```js
const PI = 3.14;
```

📌 **Features:**

* Block-scoped
* Cannot be re-declared
* Cannot be updated

```js
const PI = 3.14;
PI = 3.1415; // ❌ error
```

⚠️ **Important:**

Objects and arrays can still be modified:

```js
const person = { name: "Rahul" };
person.name = "Amit"; // ✅ allowed
```

---

## 🧱 Variable Naming Rules

### ✅ Allowed:

* Letters (`a-z`, `A-Z`)
* Numbers (not at the start)
* `_` and `$`

```js
let name1;
let _value;
let $price;
```

---

### ❌ Not Allowed:

```js
let 1name;     // ❌ starts with number
let my-name;   // ❌ hyphen not allowed
```

---

### ⚠️ Reserved Words (Cannot use)

```js
let let = 5;      // ❌
let class = "JS"; // ❌
```

---
---

## 🔢 2. Data Types in JavaScript

## 🧠 Introduction

In JavaScript, **data types define the kind of value a variable can hold**.

JavaScript is a **dynamically typed language**, which means:

* You don’t need to specify the type manually
* The type is determined automatically

### ✅ Example:

```js
let x = 10;       // Number
x = "Hello";      // Now String
```

---

## 📦 Types of Data Types

JavaScript has **2 main categories**:

1. 🧱 Primitive Data Types
2. 📦 Non-Primitive (Reference) Data Types

---

# 🧱 1. Primitive Data Types

Primitive data types:

* Store **single values**
* Are **immutable** (cannot be changed directly)

#### 1. 📝 String (Text)

📌 **Description:**
Represents text data

```js
let name = "Rahul";
let city = 'Delhi';
```

### 📌 Template Literals:

```js
let msg = `Hello ${name}`;
```

### 📌 Properties:

* Immutable
* Supports `"`, `'`, and `` ` ``

---

```js
let firstName = "John";
let lastName = 'Doe';
let greeting = `Hello, ${firstName}!`;

console.log(greeting); // "Hello, John!"
```

---

#### 2. 🔢 Number

📌 **Description:**
Represents both integers and floating-point numbers

```js
let age = 25;
let price = 99.99;
```

### 📌 Special Values:

```js
let x = Infinity;
let y = -Infinity;
let z = NaN; // Not a Number
```

⚠️ **Example:**

```js
console.log(10 / "abc"); // NaN
```

---

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

📌 **Description:**
Used for **very large integers**

```js
let big = 123456789012345678901234567890n;
```

📌 **Use Case:**

* Large number calculations beyond `Number` limits

---

```js
let bigInteger = 9007199254740991n;
console.log(typeof bigInteger); // "bigint"
```

---

#### 4. ✅ Boolean

📌 **Description:**
Represents `true` or `false`

```js
let isLoggedIn = true;
let isAdmin = false;
```

📌 **Used in:**

* Conditions
* Comparisons

---

```js
let isLoggedIn = true;
let hasAccount = false;

console.log(typeof isLoggedIn); // "boolean"
```

---

#### 5. ❓ Undefined

📌 **Description:**
A variable declared but not assigned a value

```js
let x;
console.log(x); // undefined
```

---


```js
let notAssigned;

console.log(notAssigned);        // undefined
console.log(typeof notAssigned); // "undefined"
```

---

#### 6. 🚫 Null

📌 **Description:**
Represents an **intentional empty value**

```js
let data = null;
```

⚠️ **Difference from undefined:**

* `undefined` → not assigned
* `null` → intentionally empty

---

```js
let emptyValue = null;

console.log(emptyValue);        // null
console.log(typeof emptyValue); // "object" ⚠️ (JS bug)
```

---

#### 7. 🆔 Symbol

📌 **Description:**
Used to create **unique identifiers**

```js
let id = Symbol("id");
```

📌 **Features:**

* Always unique
* Mostly used in objects

---

```js
let sym1 = Symbol("id");
let sym2 = Symbol("id");

console.log(sym1 === sym2); // false
```

---

# 📦 2. Non-Primitive (Reference) Data Types

These types:

* Store **references (memory addresses)**
* Can hold multiple values

---

#### 🧩 Object

📌 **Description:**
Collection of key-value pairs

```js
let person = {
  name: "Rahul",
  age: 25
};
```

### 📌 Access:

```js
console.log(person.name);
```

---

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

📌 **Description:**
Stores multiple values in a list

```js
let colors = ["red", "green", "blue"];
```

### 📌 Access:

```js
console.log(colors[0]); // red
```

---

```js
let colors = ["red", "green", "blue"];
console.log(typeof colors); // "object"
```

---

#### ⚙️ Functions (special objects)

📌 **Description:**
Functions are treated as objects in JavaScript

```js
function greet() {
  console.log("Hello");
}
```

```js
function sayHi() {
  return "Hi!";
}

console.log(typeof sayHi); // "function"
```

---

📌 **Description:**
Used to work with dates and time

---

## ⚖️ Primitive vs Non-Primitive

| Feature    | Primitive      | Non-Primitive |
| ---------- | -------------- | ------------- |
| Stores     | Value          | Reference     |
| Mutability | Immutable      | Mutable       |
| Examples   | Number, String | Object, Array |


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

## 🧠 Introduction

Type Conversion means **converting a value from one data type to another**.

JavaScript is a **loosely (dynamically) typed language**, so type conversion happens in two ways:

* ⚡ Automatically (Implicit)
* 🔧 Manually (Explicit)

---

## 🔄 Types of Type Conversion

1. ⚡ Implicit Type Conversion (Type Coercion)
2. 🔧 Explicit Type Conversion (Type Casting)

---

---

### 🔁 Implicit Conversion (Type Coercion)

JavaScript automatically converts types when needed.

---

## 🔤 String Conversion (Automatic)

When using `+` with a string:

```js
let result = "5" + 2;
console.log(result); // "52"
```

📌 **Rule:**
If one operand is a string, JavaScript converts others to a string.

---

## 🔢 Number Conversion (Automatic)

```js
let result = "5" - 2;
console.log(result); // 3
```

📌 **Rule:**
For `-`, `*`, `/` → JavaScript converts values to numbers.

---

## ✔️ Boolean Conversion

```js
console.log(Boolean(1)); // true
console.log(Boolean(0)); // false
```

---

## ⚠️ Examples of Coercion

```js
"5" * "2"     // 10
"10" / "2"    // 5
"abc" * 2     // NaN
true + 1      // 2
false + 1     // 1
null + 1      // 1
undefined + 1 // NaN
```

---

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

### ✅ Methods:

```js
Number("123");      // 123
parseInt("123px");  // 123
parseFloat("12.5"); // 12.5
```

### ❌ Invalid Conversion:

```js
Number("abc"); // NaN
```

---

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
String(123);      // "123"
(123).toString(); // "123"
```

---

```js
let num = 100;

let str1 = String(num);
let str2 = num.toString();
let str3 = num + "";
```

---

#### ➤ To Boolean

```js
Boolean(1);   // true
Boolean(0);   // false
Boolean("");  // false
Boolean("Hi");// true
```

---

---

# 🧪 Truthy & Falsy Values

---

**Falsy Values ❌**

These values always convert to `false`:

* `false`
* `0`
* `""` (empty string)
* `null`
* `undefined`
* `NaN`

```js
console.log(Boolean(0));         // false
console.log(Boolean(""));        // false
console.log(Boolean(null));      // false
console.log(Boolean(undefined)); // false
console.log(Boolean(NaN));       // false

```

**Truthy Values ✅**

* Everything else!

```js
Boolean("Hello"); // true
Boolean(100);     // true
```

---

```js
console.log(Boolean("hello"));   // true
console.log(Boolean(42));        // true
console.log(Boolean({}));        // true
console.log(Boolean([]));        // true
```

---

# 🔁 Special Conversion Cases

---

## 🔹 null Conversion

```js
Number(null);  // 0
String(null);  // "null"
Boolean(null); // false
```

---

## 🔹 undefined Conversion

```js
Number(undefined);  // NaN
String(undefined);  // "undefined"
Boolean(undefined); // false
```

---

## 🔹 Array Conversion

```js
Number([10]);      // 10
Number([10,20]);   // NaN
String([1,2,3]);   // "1,2,3"
```

---

## 🔹 Object Conversion

```js
Number({});   // NaN
String({});   // "[object Object]"
```

---

# ⚖️ Comparison & Type Conversion

---

## 🔸 Loose Equality (`==`)

```js
5 == "5"; // true
```

📌 Converts types before comparing

---

## 🔸 Strict Equality (`===`)

```js
5 === "5"; // false
```

📌 No conversion, checks both type and value

---

# 🔥 Real-Life Examples

---

## Example 1:

```js
let input = "100";
let total = Number(input) + 50;

console.log(total); // 150
```

---

## Example 2:

```js
let isLoggedIn = Boolean("user");
console.log(isLoggedIn); // true
```

---

## Example 3:

```js
let value = "10" * 2;
console.log(value); // 20
```

---

# ⚠️ Common Mistakes

---

❌ String + Number confusion:

```js
"10" + 5; // "105"
```

---

❌ Unexpected NaN:

```js
Number("Hello"); // NaN
```

---

❌ Confusing null & undefined

---

# 🧠 Best Practices

---

### ✅ Use explicit conversion

```js
Number(value);
String(value);
Boolean(value);
```

---

### ✅ Prefer strict equality

```js
===
```

---

### ✅ Validate input before converting

---

# 📊 Conversion Summary Table

| Value     | Number() | String()    | Boolean() |
| --------- | -------- | ----------- | --------- |
| "123"     | 123      | "123"       | true      |
| "abc"     | NaN      | "abc"       | true      |
| 0         | 0        | "0"         | false     |
| 1         | 1        | "1"         | true      |
| null      | 0        | "null"      | false     |
| undefined | NaN      | "undefined" | false     |

---

# 🎯 Conclusion

* Type conversion can be **automatic or manual**
* JavaScript often performs **implicit conversion**
* Always prefer **explicit conversion for control and safety**
* Use `===` instead of `==` to avoid bugs

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
