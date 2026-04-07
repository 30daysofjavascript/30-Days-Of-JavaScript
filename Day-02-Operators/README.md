# 🚀 Day 02 — Operators

### 📚 30 Days of JavaScript: Beginner to Advanced

---

## 🧮 1. Arithmetic Operators

Used to perform **mathematical operations**:

```js
let a = 10;
let b = 3;

console.log(a + b);  // 13  ➕ Addition
console.log(a - b);  // 7   ➖ Subtraction
console.log(a * b);  // 30  ✖️ Multiplication
console.log(a / b);  // 3.33 ➗ Division
console.log(a % b);  // 1   🧩 Modulus (remainder)
console.log(a ** b); // 1000 ⚡ Exponentiation
```

---

### 🔼 Increment & 🔽 Decrement

```js
let x = 5;

console.log(x++); // 5  (Post-increment)
console.log(x);   // 6

console.log(++x); // 7  (Pre-increment)
console.log(x--); // 7  (Post-decrement)
console.log(x);   // 6

console.log(--x); // 5  (Pre-decrement)
```

---

## 📝 2. Assignment Operators

```js
let num = 10;

num += 5;   // 15
num -= 3;   // 12
num *= 2;   // 24
num /= 4;   // 6
num %= 4;   // 2
num **= 3;  // 8

console.log(num);
```

---

### ⚡ Logical Assignment (ES2021)

```js
let count = null;
count ??= 10;  // Assign if null/undefined
console.log(count); // 10

let score = 5;
score ||= 100; // Assign if falsy
console.log(score); // 5

let flag = true;
flag &&= false; // Assign if truthy
console.log(flag); // false
```

---

## ⚖️ 3. Comparison Operators

Always return **true or false**:

```js
console.log(5 == "5");   // true  ⚠️ loose equality
console.log(5 === "5");  // false ✅ strict equality

console.log(5 != "5");   // false
console.log(5 !== "5");  // true

console.log(10 > 5);   // true
console.log(10 < 5);   // false
console.log(10 >= 10); // true
console.log(10 <= 9);  // false
```

---

### ⚠️ Important Tip

Always prefer **`===` over `==`** to avoid unexpected results:

```js
console.log(0 == false);   // true  ❌ confusing
console.log(0 === false);  // false ✅ correct

console.log("" == false);  // true  ❌
console.log("" === false); // false ✅

console.log(null == undefined);  // true ⚠️ special case
console.log(null === undefined); // false
```

---

## 🔗 4. Logical Operators

### ✅ AND (`&&`)

```js
console.log(true && true);   // true
console.log(true && false);  // false
```

### 🔀 OR (`||`)

```js
console.log(true || false);  // true
console.log(false || false); // false
```

### ❗ NOT (`!`)

```js
console.log(!true);  // false
console.log(!false); // true
```

---

### ⚡ Short-Circuiting

```js
let user = null;
let username = user && user.name;

console.log(username); // null

let displayName = username || "Guest";
console.log(displayName); // "Guest"
```

---

### 💡 Default Values Example

```js
function greet(name) {
  name = name || "stranger";
  console.log("Hello, " + name + "!");
}

greet("Alice");
greet();
greet("");
```

---

## 🧠 5. Nullish Coalescing (`??`)

```js
let val1 = null ?? "default";
let val2 = undefined ?? "default";
let val3 = 0 ?? "default";
let val4 = "" ?? "default";
let val5 = false ?? "default";

console.log(val1, val2, val3, val4, val5);
```

---

### 🔍 Difference: `||` vs `??`

```js
0 || "default";  // "default" ❌
0 ?? "default";  // 0 ✅
```

---

## 🔀 6. Ternary Operator (`? :`)

```js
let age = 20;

let status = age >= 18 ? "adult" : "minor";
console.log(status); // "adult"
```

---

### 🎯 Chained Example

```js
let score2 = 75;

let grade = score2 >= 90 ? "A"
          : score2 >= 80 ? "B"
          : score2 >= 70 ? "C"
          : score2 >= 60 ? "D"
          : "F";

console.log(grade); // "C"
```

---

## 🔗 7. Optional Chaining (`?.`)

Safely access nested properties:

```js
let userObj = {
  name: "Alice",
  address: {
    city: "Wonderland"
  }
};

console.log(userObj?.address?.city); // "Wonderland"
console.log(userObj?.phone?.number); // undefined
console.log(userObj?.getName?.());   // undefined
```

---

## 🧬 8. Bitwise Operators (Quick Look)

```js
console.log(5 & 3);   // 1
console.log(5 | 3);   // 7
console.log(5 ^ 3);   // 6
console.log(~5);      // -6
console.log(5 << 1);  // 10
console.log(5 >> 1);  // 2
```

---

## 📊 9. Operator Precedence

```js
let result = 2 + 3 * 4;    // 14
let result2 = (2 + 3) * 4; // 20
```

👉 Multiplication runs before addition (like math)

---

## 📝 Exercises

### 🧪 Exercise 1

What is:

```js
17 % 5
```

👉 Use it to check **even/odd numbers**

---

### 🧪 Exercise 2

Predict output:

```js
console.log(5 + "5");
console.log(5 - "5");
console.log(true + true + true);
```

---

### 🧪 Exercise 3

Use ternary to check:

* Positive
* Negative
* Zero

---

### 🧪 Exercise 4

Difference between:

```js
null ?? "fallback"
null || "fallback"
0 ?? "fallback"
0 || "fallback"
```

---

### 🧪 Exercise 5

```js
let data = { user: { profile: null } };

// Safely access avatar
data.user?.profile?.avatar;
```

---

## ⭐ Support

If you found this helpful:

👉 **Give this repo a ⭐ on GitHub**
👉 Share it with others 🚀
👉 Keep learning & building 💻

---

## 🎉 Day 02 Complete!

You're now comfortable with:

* Arithmetic & Assignment
* Comparison & Logical Operators
* Ternary & Optional Chaining
* Operator Precedence

👉 Next up: **Control Flow (if/else, switch, loops)** 🔥

