# 🚀 Day 02 — Operators

### 📚 30 Days of JavaScript: Beginner to Advanced

---

# JavaScript Operators (Complete Guide)

Operators in JavaScript are symbols or keywords used to perform operations on values and variables. This guide covers all major JavaScript operators with detailed explanations and examples.

---

## 1. Arithmetic Operators

Used for mathematical calculations.

| Operator | Name           | Description                        | Example         |
| -------- | -------------- | ---------------------------------- | --------------- |
| `+`      | Addition       | Adds values / concatenates strings | `5 + 2` → `7`   |
| `-`      | Subtraction    | Subtracts values                   | `5 - 2` → `3`   |
| `*`      | Multiplication | Multiplies values                  | `5 * 2` → `10`  |
| `/`      | Division       | Divides values                     | `5 / 2` → `2.5` |
| `%`      | Modulus        | Remainder                          | `5 % 2` → `1`   |
| `**`     | Exponentiation | Power operation                    | `2 ** 3` → `8`  |
| `++`     | Increment      | Increase by 1                      | `a++`           |
| `--`     | Decrement      | Decrease by 1                      | `a--`           |

---

## 1. Arithmetic Operators in JavaScript (Detailed Guide)

Arithmetic operators in JavaScript are used to perform mathematical operations on numbers (and sometimes other data types like strings).

---

## 🔹 List of Arithmetic Operators

| Operator | Name           | Description                      |
| -------- | -------------- | -------------------------------- |
| `+`      | Addition       | Adds two values                  |
| `-`      | Subtraction    | Subtracts one value from another |
| `*`      | Multiplication | Multiplies two values            |
| `/`      | Division       | Divides one value by another     |
| `%`      | Modulus        | Returns remainder                |
| `**`     | Exponentiation | Raises to power                  |
| `++`     | Increment      | Increases value by 1             |
| `--`     | Decrement      | Decreases value by 1             |

---

## ➕ 1. Addition Operator (`+`)

### ✔️ Numbers

```js
let a = 10;
let b = 5;
console.log(a + b); // 15
```

### ✔️ Strings (Concatenation)

```js
let first = "Hello";
let second = "World";
console.log(first + " " + second); // Hello World
```

### ⚠️ Type Coercion

```js
console.log(5 + "5"); // "55" (number converted to string)
```

---

## ➖ 2. Subtraction Operator (`-`)

Always converts operands to numbers.

```js
console.log(10 - 5);     // 5
console.log("10" - 5);   // 5 (string converted to number)
console.log("a" - 5);    // NaN
```

---

## ✖️ 3. Multiplication Operator (`*`)

```js
console.log(4 * 3);       // 12
console.log("4" * 2);     // 8
console.log("abc" * 2);   // NaN
```

---

## ➗ 4. Division Operator (`/`)

```js
console.log(10 / 2);   // 5
console.log(10 / 3);   // 3.333...
console.log(10 / 0);   // Infinity
```

---

## 🔁 5. Modulus Operator (`%`)

Returns remainder after division.

```js
console.log(10 % 3);  // 1
console.log(8 % 2);   // 0
```

### 📌 Common Use Cases

* Check even/odd:

```js
if (num % 2 === 0) console.log("Even");
```

---

## ⚡ 6. Exponentiation Operator (`**`)

```js
console.log(2 ** 3); // 8
console.log(5 ** 2); // 25
```

Equivalent to:

```js
Math.pow(2, 3);
```

---

## 🔼 7. Increment Operator (`++`)

Increases value by 1.

### ✔️ Pre-increment

```js
let x = 5;
console.log(++x); // 6 (increment first, then use)
```

### ✔️ Post-increment

```js
let x = 5;
console.log(x++); // 5 (use first, then increment)
console.log(x);   // 6
```

---

## 🔽 8. Decrement Operator (`--`)

Decreases value by 1.

### ✔️ Pre-decrement

```js
let x = 5;
console.log(--x); // 4
```

### ✔️ Post-decrement

```js
let x = 5;
console.log(x--); // 5
console.log(x);   // 4
```

---

## ⚠️ Special Cases & Behavior

### 1. NaN (Not a Number)

```js
console.log("abc" - 2); // NaN
```

### 2. Infinity

```js
console.log(1 / 0);  // Infinity
console.log(-1 / 0); // -Infinity
```

### 3. Mixed Types

```js
console.log(true + 1);   // 2
console.log(false + 1);  // 1
console.log(null + 1);   // 1
```

---

## 🧠 Operator Precedence (Important)

Order of execution:

1. `++` `--`
2. `**`
3. `*` `/` `%`
4. `+` `-`

Example:

```js
let result = 2 + 3 * 4; // 14
```

Use parentheses to control order:

```js
let result = (2 + 3) * 4; // 20
```

---

## ✅ Best Practices

* Use parentheses `()` to avoid confusion
* Avoid mixing strings and numbers unintentionally
* Be careful with `++` and `--` in complex expressions
* Always handle `NaN` cases when working with user input

---

## 📌 Summary

Arithmetic operators are fundamental in JavaScript and are used in almost every program. Understanding their behavior—especially type coercion and precedence—is essential for writing correct and efficient code.

---


## 2. Assignment Operators

Used to assign values.

| Operator | Description         | Example   |
| -------- | ------------------- | --------- |
| `=`      | Assign              | `x = 10`  |
| `+=`     | Add and assign      | `x += 5`  |
| `-=`     | Subtract and assign | `x -= 5`  |
| `*=`     | Multiply and assign | `x *= 5`  |
| `/=`     | Divide and assign   | `x /= 5`  |
| `%=`     | Modulus and assign  | `x %= 5`  |
| `**=`    | Exponent and assign | `x **= 2` |

---

## 2. Assignment Operators in JavaScript (Detailed Guide)

Assignment operators are used to assign values to variables. They can also perform operations and assign the result in a single step.

---

## 🔹 Basic Assignment Operator

### `=` (Simple Assignment)

Assigns the value on the right to the variable on the left.

```js id="a1b2c3"
let x = 10;
```

* The right-hand side (RHS) is evaluated first
* Then the result is stored in the left-hand side (LHS)

---

## 🔹 Compound Assignment Operators

These operators combine arithmetic operations with assignment.

---

### ➕ 1. Addition Assignment (`+=`)

Adds value and assigns result.

```js id="b2c3d4"
let x = 10;
x += 5; // x = x + 5
console.log(x); // 15
```

### ✔️ With Strings

```js id="c3d4e5"
let str = "Hello";
str += " World";
console.log(str); // Hello World
```

---

### ➖ 2. Subtraction Assignment (`-=`)

```js id="d4e5f6"
let x = 10;
x -= 3; // x = x - 3
console.log(x); // 7
```

---

### ✖️ 3. Multiplication Assignment (`*=`)

```js id="e5f6g7"
let x = 4;
x *= 2; // x = x * 2
console.log(x); // 8
```

---

### ➗ 4. Division Assignment (`/=`)

```js id="f6g7h8"
let x = 10;
x /= 2; // x = x / 2
console.log(x); // 5
```

---

### 🔁 5. Modulus Assignment (`%=`)

```js id="g7h8i9"
let x = 10;
x %= 3; // x = x % 3
console.log(x); // 1
```

---

### ⚡ 6. Exponentiation Assignment (`**=`)

```js id="h8i9j0"
let x = 2;
x **= 3; // x = x ** 3
console.log(x); // 8
```

---

## 🔹 Logical Assignment Operators (ES2021)

These are modern JavaScript operators combining logical operations with assignment.

---

### 🟢 1. AND Assignment (`&&=`)

Assigns value only if left side is truthy.

```js id="i9j0k1"
let x = 10;
x &&= 5;
console.log(x); // 5
```

```js id="j0k1l2"
let x = 0;
x &&= 5;
console.log(x); // 0 (not assigned)
```

---

### 🟡 2. OR Assignment (`||=`)

Assigns value if left side is falsy.

```js id="k1l2m3"
let x = 0;
x ||= 10;
console.log(x); // 10
```

---

### 🔵 3. Nullish Assignment (`??=`)

Assigns value only if variable is `null` or `undefined`.

```js id="l2m3n4"
let x = null;
x ??= 20;
console.log(x); // 20
```

```js id="m3n4o5"
let x = 0;
x ??= 50;
console.log(x); // 0 (not null/undefined)
```

---

## 🔹 Destructuring Assignment

Used to unpack values from arrays or objects.

---

### 📦 Array Destructuring

```js id="n4o5p6"
let arr = [1, 2, 3];
let [a, b, c] = arr;

console.log(a, b, c); // 1 2 3
```

---

### 🧩 Object Destructuring

```js id="o5p6q7"
let user = { name: "John", age: 25 };
let { name, age } = user;

console.log(name, age);
```

---

## 🔹 Default Values in Assignment

```js id="p6q7r8"
let [a = 5, b = 10] = [1];
console.log(a, b); // 1 10
```

---

## 🔹 Chained Assignment

Assign multiple variables at once.

```js id="q7r8s9"
let a, b, c;
a = b = c = 10;

console.log(a, b, c); // 10 10 10
```

⚠️ Be careful: evaluated right to left.

---

## 🔹 Type Behavior & Coercion

```js id="r8s9t0"
let x = "5";
x += 2; // "52" (string concatenation)
```

```js id="s9t0u1"
let x = "5";
x -= 2; // 3 (converted to number)
```

---

## 🧠 Operator Precedence

Assignment operators have **low precedence**, meaning most operations happen before assignment.

```js id="t0u1v2"
let x;
x = 2 + 3 * 4; // 14
```

---

## ⚠️ Common Mistakes

### ❌ Using `=` instead of `==` or `===`

```js id="u1v2w3"
if (x = 10) { } // WRONG
```

### ✔️ Correct

```js id="v2w3x4"
if (x === 10) { }
```

---

## ✅ Best Practices

* Prefer `const` and `let` over `var`
* Avoid chained assignments in complex code
* Use logical assignment operators for cleaner code
* Be mindful of type coercion

---

## 📌 Summary

Assignment operators are essential for storing and updating values efficiently. Compound and logical assignment operators help write shorter and cleaner code while improving readability.

---


## 3. Comparison Operators

Return `true` or `false`.

| Operator | Description                 | Example             |
| -------- | --------------------------- | ------------------- |
| `==`     | Equal (loose)               | `5 == "5"` → true   |
| `===`    | Strict equal (type + value) | `5 === "5"` → false |
| `!=`     | Not equal                   | `5 != 3`            |
| `!==`    | Strict not equal            | `5 !== "5"`         |
| `>`      | Greater than                | `5 > 3`             |
| `<`      | Less than                   | `5 < 3`             |
| `>=`     | Greater than or equal       | `5 >= 5`            |
| `<=`     | Less than or equal          | `5 <= 3`            |

---

## 3. Comparison Operators in JavaScript (Detailed Guide)

Comparison operators are used to compare two values or expressions. The result of a comparison is always a **Boolean value**: `true` or `false`.

---

## 🔹 List of Comparison Operators

| Operator | Name                   | Description                                 |
| -------- | ---------------------- | ------------------------------------------- |
| `==`     | Equal (Loose Equality) | Checks value only (type conversion allowed) |
| `===`    | Strict Equal           | Checks value and type (no conversion)       |
| `!=`     | Not Equal              | Checks inequality (with type conversion)    |
| `!==`    | Strict Not Equal       | Checks inequality (no type conversion)      |
| `>`      | Greater Than           | Left is greater than right                  |
| `<`      | Less Than              | Left is less than right                     |
| `>=`     | Greater Than or Equal  | Left is greater or equal                    |
| `<=`     | Less Than or Equal     | Left is less or equal                       |

---

## 🔍 1. Equal Operator (`==`) — Loose Equality

Compares values **after type conversion**.

```js id="a11"
console.log(5 == "5");   // true
console.log(true == 1);  // true
console.log(null == undefined); // true
```

### ⚠️ Type Coercion Happens

JavaScript automatically converts types before comparing.

```js id="a12"
console.log("0" == 0);  // true
console.log(false == 0); // true
```

👉 This can lead to **unexpected results**, so use carefully.

---

## 🔒 2. Strict Equal (`===`)

Compares both **value and type** (recommended).

```js id="a13"
console.log(5 === "5"); // false
console.log(5 === 5);   // true
```

✔️ No type conversion
✔️ Safer and predictable

---

## ❌ 3. Not Equal (`!=`)

Checks if values are not equal (with type coercion).

```js id="a14"
console.log(5 != "5"); // false
console.log(5 != 3);   // true
```

---

## 🚫 4. Strict Not Equal (`!==`)

Checks inequality without type conversion.

```js id="a15"
console.log(5 !== "5"); // true
console.log(5 !== 5);   // false
```

---

## 📈 5. Greater Than (`>`)

```js id="a16"
console.log(10 > 5);   // true
console.log(5 > 10);   // false
```

---

## 📉 6. Less Than (`<`)

```js id="a17"
console.log(5 < 10);   // true
```

---

## ➕ 7. Greater Than or Equal (`>=`)

```js id="a18"
console.log(10 >= 10); // true
console.log(5 >= 10);  // false
```

---

## ➖ 8. Less Than or Equal (`<=`)

```js id="a19"
console.log(5 <= 5);   // true
console.log(10 <= 5);  // false
```

---

## 🔹 Special Comparison Cases

---

### 🧩 1. Comparing Different Types

```js id="a20"
console.log("5" > 3);  // true (string converted to number)
```

---

### ⚠️ 2. `null` and `undefined`

```js id="a21"
console.log(null == undefined);  // true
console.log(null === undefined); // false
```

```js id="a22"
console.log(null > 0);  // false
console.log(null == 0); // false
```

---

### ❗ 3. NaN (Not a Number)

```js id="a23"
console.log(NaN == NaN);   // false
console.log(NaN === NaN);  // false
```

✔️ Correct way:

```js id="a24"
isNaN(NaN); // true
```

---

### 🔤 4. String Comparison

Strings are compared **lexicographically** (based on Unicode).

```js id="a25"
console.log("apple" < "banana"); // true
console.log("Z" > "a"); // false (Unicode difference)
```

---

### 🔢 5. Boolean Conversion

```js id="a26"
console.log(true == 1);  // true
console.log(false == 0); // true
```

---

## 🧠 Operator Precedence

Comparison operators have **lower precedence** than arithmetic operators.

```js id="a27"
console.log(5 + 5 > 8); // true
```

---

## ⚠️ Common Mistakes

### ❌ Using `==` instead of `===`

```js id="a28"
if (value == 0) { }
```

✔️ Better:

```js id="a29"
if (value === 0) { }
```

---

### ❌ Comparing NaN directly

```js id="a30"
NaN === NaN // false
```

✔️ Use:

```js id="a31"
Number.isNaN(NaN);
```

---

## ✅ Best Practices

* Always prefer `===` and `!==`
* Avoid relying on type coercion
* Be careful when comparing `null` and `undefined`
* Use `Number.isNaN()` for checking NaN
* Understand string comparison rules

---

## 📌 Summary

Comparison operators are essential for decision-making in JavaScript. Understanding the difference between **loose equality (`==`) and strict equality (`===`)** is crucial to avoid bugs and ensure predictable behavior.

---


## 4. Logical Operators

Used for boolean logic.

| Operator | Description       | Example             |
| -------- | ----------------- | ------------------- |
| `&&`     | AND (both true)   | `true && false`   |
| `\|\|`   | OR (one true)     | `true \|\| false` |
| `!`      | NOT (reverse)     | `!true` → `false`  |

---
## 4. Logical Operators in JavaScript (Detailed Guide)

Logical operators are used to combine or manipulate Boolean values (`true` and `false`). They are commonly used in **conditions, decision-making, and control flow**.

---

## 🔹 List of Logical Operators

| Operator | Name          | Description                                  |
| -------- | --------------|----------------------------------------------|
| `&&`     | Logical AND   | Returns true if **both** operands are true |
| `\|\|`  | Logical OR    | Returns true if **at least one** is true  |
| `!`      | Logical NOT   | Reverses the Boolean value                  |
---

## 🔗 1. Logical AND (`&&`)

### ✔️ Basic Behavior

Returns `true` only if **both conditions are true**.

```js id="l1"
console.log(true && true);   // true
console.log(true && false);  // false
console.log(false && true);  // false
```

---

### ⚡ Short-Circuit Behavior

* Returns the **first falsy value**
* If all are true, returns the **last value**

```js id="l2"
console.log(5 && 10);      // 10
console.log(0 && 10);      // 0 (stops early)
console.log("Hi" && "JS"); // "JS"
```

---

### 📌 Practical Use

```js id="l3"
let isLoggedIn = true;
let hasPermission = true;

if (isLoggedIn && hasPermission) {
  console.log("Access granted");
}
```

---

## 🔀 2. Logical OR (`||`)

### ✔️ Basic Behavior

Returns `true` if **at least one condition is true**.

```js id="l4"
console.log(true || false); // true
console.log(false || false); // false
```

---

### ⚡ Short-Circuit Behavior

* Returns the **first truthy value**
* If none are true, returns the **last value**

```js id="l5"
console.log(0 || "Hello");   // "Hello"
console.log(null || 5);      // 5
console.log("" || false);    // false
```

---

### 📌 Default Values

```js id="l6"
let name = userName || "Guest";
```

---

## 🔄 3. Logical NOT (`!`)

### ✔️ Basic Behavior

Reverses Boolean value.

```js id="l7"
console.log(!true);  // false
console.log(!false); // true
```

---

### 🔁 Double NOT (`!!`)

Used to convert value to Boolean.

```js id="l8"
console.log(!!"Hello"); // true
console.log(!!0);       // false
```

---

## 🔹 Truthy and Falsy Values

### ❌ Falsy Values

* `false`
* `0`
* `""` (empty string)
* `null`
* `undefined`
* `NaN`

Everything else is **truthy**.

---

## 🔹 Combining Logical Operators

```js id="l9"
let age = 20;

if (age > 18 && age < 30) {
  console.log("Young adult");
}
```

---

## 🔹 Operator Precedence

| Operator | Priority |   
| -------- | -------- | 
| `!`      | Highest  |   
| `&&`     | Medium   |   
| `\|\|`        |    Lowest      | 

---

### Example:

```js id="l10"
console.log(true || false && false); // true
```

✔️ Because `&&` runs first:

```js id="l11"
true || (false && false)
```

---

## 🔹 Logical Assignment Operators (Related)

These combine logical operators with assignment:

| Operator | Example             | Meaning                          |
| -------- | ------------------- | -------------------------------- |
| `&&=`    | `x &&= y`           | Assign if x is truthy            |
| `\|\|=`    | `x \|\|= y`           | Assign if x is falsy             |
| `??=`    | `x ??= y`           | Assign if x is null or undefined |    

```js id="l12"
let x = 0;
x ||= 10; // 10
```

---

## ⚠️ Common Mistakes

### ❌ Confusing `||` with `??`

```js id="l13"
let value = 0 || 10; // 10 (0 is falsy)
```

✔️ Better:

```js id="l14"
let value = 0 ?? 10; // 0
```

---

### ❌ Ignoring Short-Circuiting

```js id="l15"
false && console.log("Won't run");
```

---

## ✅ Best Practices

* Use `&&` for multiple conditions
* Use `||` for default values (but prefer `??` when needed)
* Use `!!` to convert to Boolean
* Understand short-circuit behavior to write cleaner code

---

## 📌 Summary

Logical operators are essential for controlling program flow and combining conditions. Understanding **truthy/falsy values** and **short-circuit evaluation** is key to mastering them in JavaScript.

---


## 5. Bitwise Operators

Operate on binary numbers.

| Operator | Description          | Example       |
| -------- | -------------------- | ------------- |
| `&`      | AND                  | `5 & 1` → 1   |
| `\|`     | OR                   | `5 \| 1` → 5  |
| `^`      | XOR                  | `5 ^ 1` → 4   |
| `~`      | NOT                  | `~5` → -6     |
| `<<`     | Left shift           | `5 << 1` → 10 |
| `>>`     | Right shift          | `5 >> 1` → 2  |
| `>>>`    | Unsigned right shift | `-5 >>> 1`    |

---

## 5. Bitwise Operators in JavaScript (Detailed Guide)

Bitwise operators perform operations on the **binary (bit-level) representation** of numbers. In JavaScript, all numbers are converted to **32-bit signed integers** before applying bitwise operations.

---

## 🔹 What is Bitwise Operation?

Every number in JavaScript is stored in binary form.

Example:

```js
5  = 00000000 00000000 00000000 00000101  
1  = 00000000 00000000 00000000 00000001
```

Bitwise operators work directly on these bits.

---

## 🔹 List of Bitwise Operators

| Operator | Name                 | Description                        |                            |
| -------- | -------------------- | ---------------------------------- | -------------------------- |
| `&`      | AND                  | 1 if both bits are 1               |                            |
| `\| `    | OR                                 | 1 if at least one bit is 1 |
| `^`      | XOR                  | 1 if bits are different            |                            |
| `~`      | NOT                  | Inverts all bits                   |                            |
| `<<`     | Left Shift           | Shifts bits left                   |                            |
| `>>`     | Right Shift          | Shifts bits right (sign preserved) |                            |
| `>>>`    | Unsigned Right Shift | Shifts right (fills with 0)        |                            |

---

## 🔗 1. Bitwise AND (`&`)

Returns `1` only if both bits are `1`.

```js id="b1"
console.log(5 & 1); // 1
```

### Explanation:

```
5 = 101
1 = 001
---------
    001 = 1
```

---

## 🔀 2. Bitwise OR (`|`)

Returns `1` if at least one bit is `1`.

```js id="b2"
console.log(5 | 1); // 5
```

```
5 = 101
1 = 001
---------
    101 = 5
```

---

## 🔁 3. Bitwise XOR (`^`)

Returns `1` if bits are different.

```js id="b3"
console.log(5 ^ 1); // 4
```

```
5 = 101
1 = 001
---------
    100 = 4
```

---

## 🔄 4. Bitwise NOT (`~`)

Inverts all bits (1 → 0, 0 → 1).

```js id="b4"
console.log(~5); // -6
```

### Why -6?

Because:

```
5  = 00000000 00000000 00000000 00000101
~5 = 11111111 11111111 11111111 11111010
```

This is stored in **two’s complement form**, resulting in `-6`.

---

## ⬅️ 5. Left Shift (`<<`)

Shifts bits to the left and fills with `0`.

```js id="b5"
console.log(5 << 1); // 10
```

```
5 = 00000101
<<1
---------
  00001010 = 10
```

📌 Equivalent to multiplying by 2:

```js id="b6"
x << n ≈ x * (2^n)
```

---

## ➡️ 6. Right Shift (`>>`)

Shifts bits to the right, preserving the sign.

```js id="b7"
console.log(5 >> 1); // 2
```

```
5 = 00000101
>>1
---------
  00000010 = 2
```

📌 Equivalent to dividing by 2:

```js id="b8"
x >> n ≈ x / (2^n)
```

---

## 🔄 7. Unsigned Right Shift (`>>>`)

Shifts bits right and fills with `0` (ignores sign).

```js id="b9"
console.log(-5 >>> 1); // large positive number
```

---

## 🔹 Working with Negative Numbers

JavaScript uses **two’s complement** for negative numbers.

Example:

```js id="b10"
console.log(~-1); // 0
```

---

## 🔹 Practical Use Cases

---

### ✔️ 1. Check Even or Odd

```js id="b11"
if (num & 1) {
  console.log("Odd");
} else {
  console.log("Even");
}
```

---

### ✔️ 2. Fast Math Operations

```js id="b12"
console.log(4 << 1); // 8 (fast multiply)
console.log(8 >> 1); // 4 (fast divide)
```

---

### ✔️ 3. Swap Two Numbers (without temp)

```js id="b13"
let a = 5, b = 3;

a = a ^ b;
b = a ^ b;
a = a ^ b;

console.log(a, b); // 3 5
```

---

### ✔️ 4. Bit Masking

Used to store multiple flags in one number.

```js id="b14"
let READ = 1;   // 001
let WRITE = 2;  // 010

let permission = READ | WRITE;

console.log(permission & READ); // 1 (has read)
```

---

## 🧠 Operator Precedence

Bitwise operators have **lower precedence than arithmetic operators** but higher than comparison operators.

Example:

```js id="b15"
let result = 5 + 3 & 1; // (5 + 3) & 1 = 8 & 1 = 0
```

---

## ⚠️ Important Notes

* JavaScript converts numbers to **32-bit signed integers**
* Floating-point numbers are truncated
* Be careful when working with large numbers
* Results may differ for negative values

---

## ❌ Common Mistakes

### ❌ Confusing `&` with `&&`

```js id="b16"
if (a & b) // Bitwise (wrong in conditions)
```

✔️ Use:

```js id="b17"
if (a && b)
```

---

## ✅ Best Practices

* Use bitwise operators only when needed (performance or low-level logic)
* Avoid overusing them in high-level code (reduces readability)
* Always comment complex bitwise logic
* Understand binary representation before using

---

## 📌 Summary

Bitwise operators allow direct manipulation of binary data, making them powerful for performance optimization and low-level programming tasks. However, they should be used carefully due to their complexity and potential confusion.

---


## 6. String Operators

### Concatenation

```js
"Hello" + " World"  // "Hello World"
```

### Template Literals

```js
`Hello ${name}`
```

---

## 6. String Operators in JavaScript (Detailed Guide)

String operators in JavaScript are used to **manipulate, combine, and work with text (strings)**. JavaScript provides both **operators** and **special syntax** for handling strings efficiently.

---

## 🔹 What is a String?

A string is a sequence of characters enclosed in:

```js
"double quotes"
'single quotes'
`backticks` (template literals)
```

---

## 🔹 List of String Operators

| Operator  | Name              | Description                              |
| --------- | ----------------- | ---------------------------------------- |
| `+`       | Concatenation     | Combines two or more strings             |
| `+=`      | Append Assignment | Adds and assigns string                  |
| `` ` ` `` | Template Literal  | Allows interpolation and multi-line text |

---

## ➕ 1. Concatenation Operator (`+`)

Used to join strings together.

```js id="s1"
let firstName = "John";
let lastName = "Doe";

let fullName = firstName + " " + lastName;
console.log(fullName); // John Doe
```

---

### ⚠️ With Numbers (Type Coercion)

```js id="s2"
console.log("5" + 2);   // "52"
console.log(2 + "5");   // "25"
```

👉 If one operand is a string, JavaScript converts the other to string.

---

### 🔁 Multiple Concatenations

```js id="s3"
let msg = "Hello" + " " + "World" + "!";
console.log(msg); // Hello World!
```

---

## ➕ 2. Append Assignment (`+=`)

Adds string to an existing variable.

```js id="s4"
let text = "Hello";
text += " World";

console.log(text); // Hello World
```

---

### ✔️ Example with Loop

```js id="s5"
let result = "";

for (let i = 1; i <= 3; i++) {
  result += i;
}

console.log(result); // "123"
```

---

## 🔤 3. Template Literals (`` ` ` ``)

Modern and powerful way to work with strings.

---

### ✔️ Basic Syntax

```js id="s6"
let name = "John";
console.log(`Hello ${name}`);
```

---

### 🔢 Expression Inside String

```js id="s7"
let a = 5;
let b = 3;

console.log(`Sum is ${a + b}`); // Sum is 8
```

---

### 📄 Multi-line Strings

```js id="s8"
let text = `This is
a multi-line
string`;

console.log(text);
```

---

### 🎯 Function Calls Inside

```js id="s9"
function greet(name) {
  return `Hello ${name}`;
}

console.log(`${greet("John")}`);
```

---

## 🔹 String Comparison (Using Operators)

Strings can also be compared using comparison operators.

```js id="s10"
console.log("apple" < "banana"); // true
console.log("Z" > "a");          // false
```

📌 Compared based on **Unicode values**.

---

## 🔹 Escape Characters

Used to include special characters.

| Escape | Meaning      |
| ------ | ------------ |
| `\'`   | Single quote |
| `\"`   | Double quote |
| `\\`   | Backslash    |
| `\n`   | New line     |
| `\t`   | Tab          |

```js id="s11"
console.log("Hello\nWorld");
```

---

## 🔹 String + Other Types

JavaScript automatically converts types when needed.

```js id="s12"
console.log("Age: " + 25);     // "Age: 25"
console.log("Result: " + true); // "Result: true"
```

---

## 🔹 Immutability of Strings

Strings are **immutable** (cannot be changed directly).

```js id="s13"
let str = "Hello";
str[0] = "h"; // ❌ No effect

console.log(str); // "Hello"
```

✔️ Instead:

```js id="s14"
str = "h" + str.slice(1);
```

---

## 🔹 Operator Precedence

```js id="s15"
console.log("Hello" + 5 + 5); // "Hello55"
console.log(5 + 5 + "Hello"); // "10Hello"
```

👉 Left to right evaluation matters.

---

## ⚠️ Common Mistakes

### ❌ Mixing Numbers and Strings

```js id="s16"
let result = 10 + "5"; // "105"
```

---

### ❌ Forgetting Backticks in Template Literals

```js id="s17"
let name = "John";
console.log("Hello ${name}"); // ❌ Not interpolated
```

✔️ Correct:

```js id="s18"
console.log(`Hello ${name}`);
```

---

## ✅ Best Practices

* Prefer **template literals** over `+` for readability
* Avoid unnecessary string concatenation in loops
* Be mindful of type coercion
* Use meaningful variable names for clarity

---

## 📌 Summary

String operators in JavaScript make it easy to combine and manipulate text. While `+` and `+=` are useful, **template literals** provide a cleaner and more powerful way to work with strings in modern JavaScript.

---


## 7. Ternary Operator

Shortcut for `if...else`.

```js
condition ? expr1 : expr2;
```

Example:

```js
let result = age >= 18 ? "Adult" : "Minor";
```

---

## 7. Ternary Operator in JavaScript (Detailed Guide)

The **ternary operator** is a shorthand way of writing an `if...else` statement in a single line. It is the only operator in JavaScript that takes **three operands**, which is why it is called “ternary”.

---

## 🔹 Syntax

```js id="t1"
condition ? expressionIfTrue : expressionIfFalse;
```

### ✔️ How it works:

* If `condition` is **true**, the first expression runs
* If `condition` is **false**, the second expression runs

---

## 🔹 Basic Example

```js id="t2"
let age = 18;

let result = (age >= 18) ? "Adult" : "Minor";

console.log(result); // Adult
```

---

## 🔹 Equivalent if...else

```js id="t3"
let age = 18;
let result;

if (age >= 18) {
  result = "Adult";
} else {
  result = "Minor";
}

console.log(result);
```

👉 Ternary operator is a shorter version of this.

---

## 🔹 Multiple Ternary (Nested)

You can use nested ternary operators, but it may reduce readability.

```js id="t4"
let marks = 85;

let grade =
  marks >= 90 ? "A+" :
  marks >= 75 ? "A"  :
  marks >= 60 ? "B"  :
  marks >= 40 ? "C"  :
  "Fail";

console.log(grade); // A
```

---

## 🔹 Ternary with Functions

```js id="t5"
function checkNumber(num) {
  return num > 0 ? "Positive" : "Negative";
}

console.log(checkNumber(10)); // Positive
```

---

## 🔹 Ternary for Assignments

```js id="t6"
let isLoggedIn = true;

let message = isLoggedIn ? "Welcome back!" : "Please log in";

console.log(message);
```

---

## 🔹 Ternary in Return Statements

```js id="t7"
function max(a, b) {
  return a > b ? a : b;
}

console.log(max(10, 20)); // 20
```

---

## 🔹 Ternary for Conditional Rendering

Common in frontend frameworks like React.

```js id="t8"
let isLoading = true;

console.log(isLoading ? "Loading..." : "Data loaded");
```

---

## 🔹 Multiple Conditions Example

```js id="t9"
let age = 25;

let type =
  age < 13 ? "Child" :
  age < 18 ? "Teenager" :
  age < 60 ? "Adult" :
  "Senior";

console.log(type); // Adult
```

---

## 🔹 Ternary vs if...else

| Feature        | Ternary Operator           | if...else                |
| -------------- | -------------------------- | ------------------------ |
| Lines of code  | Short                      | Longer                   |
| Readability    | Good for simple conditions | Better for complex logic |
| Multiple logic | Not ideal                  | Best choice              |
| Usage          | Expressions only           | Statements               |

---

## ⚠️ Common Mistakes

### ❌ Using for complex logic

```js id="t10"
let result = a > b ? (c > d ? "X" : "Y") : "Z";
```

👉 This becomes hard to read.

---

### ❌ Forgetting return or assignment

```js id="t11"
age >= 18 ? "Adult" : "Minor"; // value not used
```

✔️ Correct:

```js id="t12"
let result = age >= 18 ? "Adult" : "Minor";
```

---

## 🔹 Truthy/Falsy with Ternary

```js id="t13"
let name = "";

let display = name ? "Name exists" : "No name";

console.log(display); // No name
```

---

## 🔹 Short-Circuit Alternative vs Ternary

```js id="t14"
// Ternary
let msg = age > 18 ? "Adult" : "Minor";

// OR operator (different behavior)
let msg2 = age > 18 || "Minor";
```

---

## ✅ Best Practices

* Use ternary for **simple conditions only**
* Avoid deeply nested ternary expressions
* Use parentheses for clarity
* Prefer `if...else` for complex logic
* Always store result in a variable or return it

---

## 📌 Summary

The ternary operator is a powerful and concise way to write conditional logic in JavaScript. It improves readability for simple decisions but should be avoided for complex branching to keep code clean and maintainable.

---


## 8. Type Operators

| Operator     | Description        | Example                |
| ------------ | ------------------ | ---------------------- |
| `typeof`     | Returns data type  | `typeof 5` → "number"  |
| `instanceof` | Checks object type | `arr instanceof Array` |

---

# 8. Type Operators in JavaScript (Detailed Guide)

Type operators in JavaScript are used to **check, determine, or work with data types** of values and objects. They help developers understand what kind of data they are dealing with at runtime.

---

## 🔹 List of Type Operators in JavaScript

| Operator / Keyword | Name            | Description                                   |
| ------------------ | --------------- | --------------------------------------------- |
| `typeof`           | Typeof Operator | Returns the data type of a value              |
| `instanceof`       | Instance Check  | Checks if an object is an instance of a class |

---

# 🔤 1. `typeof` Operator

The `typeof` operator returns a **string indicating the type of a value**.

---

## 🔹 Syntax

```js id="to1"
typeof value;
```

---

## 🔹 Basic Examples

```js id="to2"
console.log(typeof 42);            // "number"
console.log(typeof "Hello");       // "string"
console.log(typeof true);          // "boolean"
console.log(typeof undefined);     // "undefined"
```

---

## 🔹 Object Types

```js id="to3"
console.log(typeof { name: "John" }); // "object"
console.log(typeof [1, 2, 3]);        // "object"
console.log(typeof null);             // "object" ❗ (known JavaScript bug)
```

---

## ⚠️ Important Note: `typeof null`

```js id="to4"
console.log(typeof null); // "object"
```

👉 This is a long-standing bug in JavaScript, but it is not fixed due to backward compatibility.

---

## 🔹 Functions

```js id="to5"
function greet() {}

console.log(typeof greet); // "function"
```

---

## 🔹 Real-world Use Case

```js id="to6"
let input = 10;

if (typeof input === "number") {
  console.log("Valid number");
}
```

---

## 🔹 Dynamic Typing Example

```js id="to7"
let x = "Hello";
console.log(typeof x); // string

x = 100;
console.log(typeof x); // number
```

---

# 🧩 2. `instanceof` Operator

The `instanceof` operator checks whether an object is an **instance of a specific class or constructor function**.

---

## 🔹 Syntax

```js id="in1"
object instanceof Constructor
```

---

## 🔹 Basic Example

```js id="in2"
let arr = [1, 2, 3];

console.log(arr instanceof Array); // true
console.log(arr instanceof Object); // true
```

---

## 🔹 Object Example

```js id="in3"
let obj = { name: "John" };

console.log(obj instanceof Object); // true
```

---

## 🔹 Function Constructor Example

```js id="in4"
function Person(name) {
  this.name = name;
}

let p1 = new Person("Alice");

console.log(p1 instanceof Person); // true
```

---

## 🔹 Built-in Objects

```js id="in5"
let date = new Date();

console.log(date instanceof Date);   // true
console.log(date instanceof Object); // true
```

---

## 🔹 Prototype Chain Concept

`instanceof` works by checking the **prototype chain**.

```js id="in6"
console.log([] instanceof Array);   // true
console.log([] instanceof Object);  // true
```

---

# ⚖️ `typeof` vs `instanceof`

| Feature        | `typeof`                 | `instanceof`                  |
| -------------- | ------------------------ | ----------------------------- |
| Works on       | Primitive + basic types  | Objects only                  |
| Returns        | String                   | Boolean                       |
| Best for       | Type checking primitives | Checking object types/classes |
| Example output | "number", "string"       | true / false                  |

---

## 🔹 Example Comparison

```js id="co1"
let arr = [1, 2, 3];

console.log(typeof arr);       // "object"
console.log(arr instanceof Array); // true
```

---

# ⚠️ Common Mistakes

---

## ❌ Assuming typeof distinguishes arrays

```js id="cm1"
typeof [] // "object"
```

✔️ Correct way:

```js id="cm2"
Array.isArray([]);
```

---

## ❌ Using instanceof for primitives

```js id="cm3"
"hello" instanceof String // false
```

✔️ Correct:

```js id="cm4"
typeof "hello" === "string"
```

---

# 🧠 Advanced Notes

---

## 🔹 Wrapper Objects

```js id="ad1"
let str = new String("Hello");

console.log(str instanceof String); // true
console.log(typeof str); // "object"
```

---

## 🔹 Function Type

```js id="ad2"
console.log(typeof function () {}); // "function"
```

---

## 🔹 Edge Case

```js id="ad3"
console.log(typeof NaN); // "number"
```

👉 Even though NaN means "Not a Number", its type is still `number`.

---

# ✅ Best Practices

* Use `typeof` for **primitives**
* Use `instanceof` for **objects and classes**
* Use `Array.isArray()` for arrays
* Avoid relying on `typeof null`
* Combine checks for safer validation

---

# 📌 Summary

Type operators in JavaScript help identify and verify data types at runtime.

* `typeof` is best for checking primitive values
* `instanceof` is best for checking object inheritance and class instances

Understanding both is essential for writing robust and error-free JavaScript code.

---


## 9. Unary Operators

| Operator | Description       | Example    |
| -------- | ----------------- | ---------- |
| `+`      | Convert to number | `+"5"` → 5 |
| `-`      | Negation          | `-5`       |
| `++`     | Increment         | `++x`      |
| `--`     | Decrement         | `--x`      |
| `!`      | Logical NOT       | `!true`    |

---

# 9. Unary Operators in JavaScript (Detailed Guide)

Unary operators in JavaScript are operators that work with **only one operand**. They are used to perform operations like incrementing, decrementing, type conversion, negation, and logical inversion.

---

## 🔹 What is a Unary Operator?

A unary operator takes a **single value (operand)** and performs an operation on it.

### Example:

```js id="u1"
let x = 5;
-x;
```

Here, `-` is acting on only one value (`x`), so it is unary.

---

## 🔹 List of Unary Operators in JavaScript

| Operator | Name            | Description                                |
| -------- | --------------- | ------------------------------------------ |
| `+`      | Unary Plus      | Converts operand to number                 |
| `-`      | Unary Minus     | Negates a number                           |
| `++`     | Increment       | Increases value by 1                       |
| `--`     | Decrement       | Decreases value by 1                       |
| `!`      | Logical NOT     | Converts value to boolean and negates it   |
| `typeof` | Type Operator   | Returns type of a value                    |
| `delete` | Delete Operator | Removes object property                    |
| `void`   | Void Operator   | Evaluates expression and returns undefined |

---

# ➕ 1. Unary Plus (`+`)

The unary plus converts a value into a **number type**.

---

## 🔹 Example

```js id="up1"
console.log(+"5");     // 5
console.log(+"10");    // 10
console.log(+true);    // 1
console.log(+false);   // 0
console.log(+"");      // 0
```

---

## 🔹 Non-numeric values

```js id="up2"
console.log(+"hello"); // NaN
```

---

## 🔹 Use Case

Quick type conversion:

```js id="up3"
let str = "100";
let num = +str;

console.log(typeof num); // number
```

---

# ➖ 2. Unary Minus (`-`)

The unary minus converts a value to number and negates it.

---

## 🔹 Example

```js id="um1"
console.log(-5);     // -5
console.log(-"10");  // -10
console.log(-true);   // -1
```

---

## 🔹 Example with conversion

```js id="um2"
console.log(-"20"); // -20
console.log(-"abc"); // NaN
```

---

# 🔼 3. Increment Operator (`++`)

Increases a value by 1.

---

## 🔹 Pre-Increment

```js id="inc1"
let x = 5;
console.log(++x); // 6
```

✔️ Increments first, then returns value.

---

## 🔹 Post-Increment

```js id="inc2"
let x = 5;
console.log(x++); // 5
console.log(x);   // 6
```

✔️ Returns first, then increments.

---

# 🔽 4. Decrement Operator (`--`)

Decreases a value by 1.

---

## 🔹 Pre-Decrement

```js id="dec1"
let x = 5;
console.log(--x); // 4
```

---

## 🔹 Post-Decrement

```js id="dec2"
let x = 5;
console.log(x--); // 5
console.log(x);   // 4
```

---

# ❗ 5. Logical NOT (`!`)

Converts a value into boolean and then reverses it.

---

## 🔹 Example

```js id="not1"
console.log(!true);  // false
console.log(!false); // true
```

---

## 🔹 Falsy Values

```js id="not2"
console.log(!0);        // true
console.log(!"");       // true
console.log(!null);     // true
console.log(!undefined);// true
console.log(!NaN);      // true
```

---

## 🔹 Double NOT (!!)

Converts value into a boolean.

```js id="not3"
console.log(!!"Hello"); // true
console.log(!!0);       // false
```

---

# 🔍 6. typeof Operator

Returns the type of a value.

```js id="type1"
console.log(typeof 10);       // "number"
console.log(typeof "JS");     // "string"
console.log(typeof true);     // "boolean"
console.log(typeof undefined);// "undefined"
```

---

# 🗑️ 7. delete Operator

Removes a property from an object.

---

## 🔹 Example

```js id="del1"
let obj = {
  name: "John",
  age: 25
};

delete obj.age;

console.log(obj); // { name: "John" }
```

---

# 🚫 8. void Operator

Evaluates an expression and returns `undefined`.

---

## 🔹 Example

```js id="void1"
console.log(void 0); // undefined
console.log(void (2 + 2)); // undefined
```

---

## 🔹 Use Case

Often used in links to prevent navigation:

```js id="void2"
<a href="javascript:void(0)">Click Me</a>
```

---

# 🔹 Unary Operator Behavior Summary

| Operator | Effect                        |
| -------- | ----------------------------- |
| `+`      | Converts to number            |
| `-`      | Negates number                |
| `++`     | Adds 1                        |
| `--`     | Subtracts 1                   |
| `!`      | Converts to boolean and flips |
| `typeof` | Returns type                  |
| `delete` | Removes object property       |
| `void`   | Returns undefined             |

---

# ⚠️ Common Mistakes

---

## ❌ Confusing ++ usage

```js id="cm1"
let x = 5;
console.log(x++ + ++x);
```

👉 Hard to read, avoid in production code.

---

## ❌ Using delete on variables

```js id="cm2"
let x = 10;
delete x; // ❌ does not work
```

✔️ Only works on object properties.

---

## ❌ Using + on non-numeric strings

```js id="cm3"
console.log(+"abc"); // NaN
```

---

# ✅ Best Practices

* Prefer readability over clever unary usage
* Avoid mixing pre/post increment in one expression
* Use `!!` carefully for boolean conversion
* Use `delete` only for object properties
* Avoid `void` unless necessary

---

# 📌 Summary

Unary operators in JavaScript operate on a single operand and are used for type conversion, arithmetic changes, logical operations, and object manipulation. Understanding them is important for writing efficient and clean JavaScript code.

---


## 10. Spread & Rest Operators

### Spread (`...`)

Expands elements.

```js
let arr = [1, 2, 3];
let newArr = [...arr, 4];
```

### Rest (`...`)

Collects remaining elements.

```js
function sum(...nums) {
  return nums.reduce((a, b) => a + b);
}
```

---

## 10. Spread & Rest Operators in JavaScript (Full Detailed Guide)

The **spread (`...`)** and **rest (`...`) operators** use the same syntax but behave differently depending on the context. They are used for working with **arrays, objects, and function arguments** in a clean and powerful way.

---

# 🔹 What is `...` (Three Dots)?

The `...` operator can work in two ways:

| Mode   | Name            | Purpose                                         |
| ------ | --------------- | ----------------------------------------------- |
| Spread | Expands values  | Breaks arrays/objects into individual elements  |
| Rest   | Collects values | Gathers multiple elements into one array/object |

---

# 🚀 1. Spread Operator (Expanding Values)

The spread operator is used to **expand** an iterable (like array or object) into individual elements.

---

## 🔹 Spread in Arrays

### ✔️ Copying an Array

```js id="sp1"
let arr1 = [1, 2, 3];
let arr2 = [...arr1];

console.log(arr2); // [1, 2, 3]
```

👉 Creates a **shallow copy**

---

### ✔️ Merging Arrays

```js id="sp2"
let a = [1, 2];
let b = [3, 4];

let result = [...a, ...b];

console.log(result); // [1, 2, 3, 4]
```

---

### ✔️ Adding Elements

```js id="sp3"
let arr = [2, 3, 4];

let newArr = [1, ...arr, 5];

console.log(newArr); // [1, 2, 3, 4, 5]
```

---

## 🔹 Spread in Objects

### ✔️ Copying Object

```js id="sp4"
let obj1 = { name: "John", age: 25 };
let obj2 = { ...obj1 };

console.log(obj2);
```

---

### ✔️ Merging Objects

```js id="sp5"
let a = { x: 1, y: 2 };
let b = { z: 3 };

let result = { ...a, ...b };

console.log(result); // { x: 1, y: 2, z: 3 }
```

---

### ✔️ Overriding Properties

```js id="sp6"
let user = { name: "John", age: 25 };
let updatedUser = { ...user, age: 30 };

console.log(updatedUser);
```

---

## 🔹 Spread in Function Calls

### ✔️ Passing Array as Arguments

```js id="sp7"
function sum(a, b, c) {
  return a + b + c;
}

let nums = [1, 2, 3];

console.log(sum(...nums)); // 6
```

---

# 📦 2. Rest Operator (Collecting Values)

The rest operator collects multiple values into a **single array or object**.

---

## 🔹 Rest in Functions

### ✔️ Collect Arguments

```js id="rs1"
function sum(...numbers) {
  return numbers.reduce((a, b) => a + b);
}

console.log(sum(1, 2, 3, 4)); // 10
```

👉 All arguments are collected into `numbers` array.

---

## 🔹 Rest with Named Parameters

```js id="rs2"
function show(first, second, ...rest) {
  console.log(first);
  console.log(second);
  console.log(rest);
}

show(1, 2, 3, 4, 5);
```

Output:

```
1
2
[3, 4, 5]
```

---

## 🔹 Rest in Arrays (Destructuring)

```js id="rs3"
let [a, b, ...rest] = [1, 2, 3, 4, 5];

console.log(a);    // 1
console.log(b);    // 2
console.log(rest); // [3, 4, 5]
```

---

## 🔹 Rest in Objects

```js id="rs4"
let user = {
  name: "John",
  age: 25,
  city: "Delhi"
};

let { name, ...details } = user;

console.log(name);     // John
console.log(details);   // { age: 25, city: "Delhi" }
```

---

# ⚖️ Spread vs Rest (Key Difference)

| Feature | Spread (`...`)         | Rest (`...`)                       |
| ------- | ---------------------- | ---------------------------------- |
| Purpose | Expands values         | Collects values                    |
| Usage   | Array/Object expansion | Function arguments / destructuring |
| Output  | Individual elements    | Array/Object                       |

---

## 🔹 Example Comparison

### Spread

```js id="cmp1"
let arr = [1, 2, 3];
console.log(...arr); // 1 2 3
```

### Rest

```js id="cmp2"
function test(...arr) {
  console.log(arr);
}

test(1, 2, 3); // [1, 2, 3]
```

---

# 🔹 Real-World Use Cases

---

## ✔️ 1. Copying Data Safely

```js id="real1"
let original = [1, 2, 3];
let copy = [...original];
```

---

## ✔️ 2. Updating State (React style)

```js id="real2"
let state = { name: "John", age: 25 };
let newState = { ...state, age: 30 };
```

---

## ✔️ 3. Flexible Function Parameters

```js id="real3"
function logAll(...args) {
  console.log(args);
}
```

---

## ✔️ 4. Merging Data

```js id="real4"
let defaults = { theme: "dark" };
let userSettings = { fontSize: 14 };

let config = { ...defaults, ...userSettings };
```

---

# ⚠️ Common Mistakes

---

## ❌ Using rest in wrong position

```js id="err1"
let [a, ...rest, b] = [1, 2, 3]; // ❌ error
```

✔️ Rest must be last:

```js id="err2"
let [a, ...rest] = [1, 2, 3];
```

---

## ❌ Confusing spread and rest

```js id="err3"
// Spread
let arr = [...[1,2,3]]

// Rest
function f(...args) {}
```

---

# 🧠 Important Notes

* Both use `...` syntax
* Spread = expands
* Rest = collects
* Works with arrays, objects, and functions
* Always shallow copy (not deep copy)

---

# ⚠️ Shallow Copy Warning

```js id="warn1"
let obj1 = { a: 1, b: { c: 2 } };
let obj2 = { ...obj1 };

obj2.b.c = 99;

console.log(obj1.b.c); // 99 (same reference)
```

---

# ✅ Best Practices

* Use spread for clean copying and merging
* Use rest for flexible function arguments
* Avoid deeply nested mutation issues
* Be careful with shallow copy behavior
* Prefer destructuring with rest for clarity

---

# 📌 Summary

The spread and rest operators are powerful ES6 features that simplify working with arrays, objects, and functions.

* **Spread (`...`) → expands values**
* **Rest (`...`) → collects values**

Mastering them leads to cleaner, more modern JavaScript code.

---


## 11. Optional Chaining Operator (`?.`)

Safely access nested properties.

```js
user?.profile?.name
```

---

## 11. Optional Chaining Operator in JavaScript (Full Detailed Guide)

The **Optional Chaining Operator (`?.`)** is a modern JavaScript feature used to safely access deeply nested object properties without causing errors if a property is `null` or `undefined`.

It helps prevent common runtime errors like:

```
Cannot read properties of undefined
```

---

# 🔹 What is Optional Chaining?

Optional chaining allows you to **access nested properties safely**. If any part of the chain is `null` or `undefined`, JavaScript will stop and return `undefined` instead of throwing an error.

---

## 🔹 Syntax

```js id="oc1"
object?.property
object?.[expression]
object?.method()
```

---

# 🚀 1. Accessing Object Properties Safely

### ❌ Without Optional Chaining

```js id="oc2"
let user = {};

console.log(user.address.city); 
// ❌ Error: Cannot read properties of undefined
```

---

### ✔️ With Optional Chaining

```js id="oc3"
let user = {};

console.log(user?.address?.city); 
// undefined (no error)
```

---

# 🔹 2. Nested Object Access

```js id="oc4"
let user = {
  name: "John",
  address: {
    city: "Delhi"
  }
};

console.log(user?.address?.city); // Delhi
```

---

## 🔹 If Property Does Not Exist

```js id="oc5"
console.log(user?.profile?.age); // undefined
```

👉 No error is thrown even if `profile` does not exist.

---

# 🔹 3. Optional Chaining with Functions

You can safely call functions that may or may not exist.

---

## ❌ Without Optional Chaining

```js id="oc6"
let user = {};

user.sayHello(); // ❌ Error
```

---

## ✔️ With Optional Chaining

```js id="oc7"
let user = {};

user.sayHello?.(); // undefined (no error)
```

---

## ✔️ With Existing Function

```js id="oc8"
let user = {
  sayHello() {
    return "Hello!";
  }
};

console.log(user.sayHello?.()); // Hello!
```

---

# 🔹 4. Optional Chaining with Arrays

You can safely access array elements.

```js id="oc9"
let arr = null;

console.log(arr?.[0]); // undefined
```

---

## ✔️ Normal Array Case

```js id="oc10"
let arr = [10, 20, 30];

console.log(arr?.[1]); // 20
```

---

# 🔹 5. Optional Chaining with Dynamic Keys

```js id="oc11"
let user = {
  name: "John"
};

let key = "age";

console.log(user?.[key]); // undefined
```

---

# 🔹 6. Real-World Use Cases

---

## ✔️ API Response Handling

```js id="oc12"
let response = {
  data: {
    user: {
      name: "Alice"
    }
  }
};

console.log(response?.data?.user?.name); // Alice
```

---

## ✔️ Preventing UI Crashes

```js id="oc13"
let user = null;

console.log(user?.profile?.settings?.theme); // undefined
```

---

## ✔️ Safe Function Call in Config

```js id="oc14"
let config = {
  onLoad: null
};

config.onLoad?.();
```

---

# ⚖️ Optional Chaining vs Traditional Checking

---

## ❌ Without Optional Chaining

```js id="oc15"
if (user && user.address && user.address.city) {
  console.log(user.address.city);
}
```

---

## ✔️ With Optional Chaining

```js id="oc16"
console.log(user?.address?.city);
```

👉 Much cleaner and easier to read.

---

# ⚠️ Important Rules

---

## ❌ Cannot Assign Using Optional Chaining

```js id="oc17"
user?.name = "John"; // ❌ Invalid
```

✔️ You can only **read**, not assign.

---

## ❌ Cannot Use on Left Side

```js id="oc18"
user?.address?.city = "Delhi"; // ❌ Error
```

---

# 🔹 Short-Circuit Behavior

If any part of the chain is `null` or `undefined`, execution stops.

```js id="oc19"
let user = null;

console.log(user?.address?.city);
// Stops at user → returns undefined
```

---

# 🔹 Optional Chaining with Nullish Values

```js id="oc20"
let user = {
  name: null
};

console.log(user?.name); // null (not replaced)
```

👉 Only stops for `null` or `undefined`, not other falsy values.

---

# 🧠 Common Mistakes

---

## ❌ Overusing Optional Chaining

```js id="oc21"
console.log(user?.address?.city?.length);
```

👉 Can hide real bugs if overused.

---

## ❌ Assuming it fixes all errors

Optional chaining only prevents **null/undefined errors**, not logic errors.

---

# 🧪 Example: Real API Safety

```js id="oc22"
let apiResponse = {};

let username = apiResponse?.data?.user?.profile?.name ?? "Guest";

console.log(username);
```

---

# 🧩 Works Well With Nullish Coalescing (`??`)

```js id="oc23"
let user = {};

let name = user?.name ?? "Anonymous";

console.log(name); // Anonymous
```

---

# ✅ Best Practices

* Use optional chaining for **safe property access**
* Combine with `??` for default values
* Avoid overusing it everywhere
* Do not use it for assignment
* Prefer it over long `&&` checks

---

# 📌 Summary

The Optional Chaining Operator (`?.`) is a powerful JavaScript feature that allows safe access to deeply nested properties, methods, and arrays without causing runtime errors.

* Prevents "Cannot read property of undefined"
* Improves code readability
* Works with objects, arrays, and functions

👉 It is essential for modern JavaScript development, especially when dealing with APIs and dynamic data.

---


## 12. Nullish Coalescing (`??`)

Returns right-hand value if left is `null` or `undefined`.

```js
let name = userName ?? "Guest";
```

---

## 12. Nullish Coalescing Operator in JavaScript (Full Detailed Guide)

The **Nullish Coalescing Operator (`??`)** is a modern JavaScript operator used to provide a **default value only when a value is `null` or `undefined`**.

It helps you handle missing or empty values more precisely than the logical OR (`||`) operator.

---

# 🔹 What is Nullish Coalescing?

The `??` operator returns:

* The **left-hand value** if it is NOT `null` or `undefined`
* Otherwise, it returns the **right-hand (default) value**

---

## 🔹 Syntax

```js id="nc1"
let result = value ?? defaultValue;
```

---

# 🚀 1. Basic Example

```js id="nc2"
let name = null;

let displayName = name ?? "Guest";

console.log(displayName); // Guest
```

---

## ✔️ If value exists

```js id="nc3"
let name = "John";

let displayName = name ?? "Guest";

console.log(displayName); // John
```

👉 Because `name` is not null or undefined.

---

# 🔹 2. Difference Between `??` and `||`

This is very important in JavaScript.

---

## 🔸 Logical OR (`||`)

Returns the first **truthy** value.

```js id="nc4"
let value = 0 || 10;
console.log(value); // 10
```

👉 Because `0` is falsy.

---

## 🔸 Nullish Coalescing (`??`)

Only checks `null` or `undefined`.

```js id="nc5"
let value = 0 ?? 10;
console.log(value); // 0
```

👉 Because `0` is NOT null or undefined.

---

## ⚖️ Key Difference Table

| Feature | `||` (OR) | `??` (Nullish) |
|--------|----------|----------------|
| Checks | Falsy values | Only null/undefined |
| Treats `0` as | Fallback | Valid value |
| Treats `""` as | Fallback | Valid value |
| Best use | General fallback | Strict fallback |

---

# 🔹 3. Common Use Cases

---

## ✔️ Default Values in Variables

```js id="nc6"
let username = null;

let name = username ?? "Anonymous";

console.log(name); // Anonymous
```

---

## ✔️ API Response Handling

```js id="nc7"
let response = {
  data: {
    user: null
  }
};

let userName = response.data.user ?? "Guest";

console.log(userName); // Guest
```

---

## ✔️ Form Inputs

```js id="nc8"
let inputValue = "";

let value = inputValue ?? "Default Value";

console.log(value); // "" (empty string is valid)
```

---

# 🔹 4. With Optional Chaining (`?.`)

Nullish coalescing works perfectly with optional chaining.

---

## ✔️ Safe Nested Access

```js id="nc9"
let user = {};

let city = user?.address?.city ?? "Unknown";

console.log(city); // Unknown
```

---

# 🔹 5. Multiple Nullish Coalescing

You can chain multiple fallbacks.

```js id="nc10"
let value = null ?? undefined ?? "Default";

console.log(value); // Default
```

---

# 🔹 6. Real-World Example

```js id="nc11"
let settings = {
  theme: null,
  fontSize: 0
};

let theme = settings.theme ?? "light";
let fontSize = settings.fontSize ?? 14;

console.log(theme);    // light
console.log(fontSize); // 0
```

---

# ⚠️ Important Rules

---

## ❌ Cannot Use Without Proper Grouping in Mixed Expressions

```js id="nc12"
// ❌ Error
let result = null ?? 10 || 20;
```

✔️ Correct way:

```js id="nc13"
let result = (null ?? 10) || 20;
```

---

## ❌ Cannot Combine with AND/OR Without Parentheses

```js id="nc14"
// ❌ Syntax Error
null ?? 10 && 20;
```

✔️ Fix:

```js id="nc15"
(null ?? 10) && 20;
```

---

# 🔹 7. Nullish vs Falsy Values

| Value       | Falsy? | Nullish? |
| ----------- | ------ | -------- |
| `0`         | Yes    | No       |
| `""`        | Yes    | No       |
| `false`     | Yes    | No       |
| `null`      | Yes    | Yes      |
| `undefined` | Yes    | Yes      |

---

# 🧠 Common Mistakes

---

## ❌ Using `||` instead of `??`

```js id="nc16"
let age = 0 || 18; // 18 (wrong if 0 is valid)
```

✔️ Correct:

```js id="nc17"
let age = 0 ?? 18; // 0
```

---

## ❌ Assuming it works like OR

Nullish coalescing is **NOT logical OR**.

---

# 🔹 8. Why Use Nullish Coalescing?

* Prevents accidental fallback for valid falsy values
* Improves accuracy in default handling
* Works perfectly with APIs and dynamic data
* Cleaner than multiple `if` checks

---

# 🔹 9. Best Practices

✔ Use `??` for default values
✔ Use with `?.` for safe nested access
✔ Avoid mixing with `||` without parentheses
✔ Prefer it over `||` when `0`, `""`, or `false` are valid inputs

---

# 📌 Summary

The Nullish Coalescing Operator (`??`) is used to provide default values only when a variable is `null` or `undefined`.

* `??` is more precise than `||`
* It avoids unwanted fallback for valid falsy values like `0` or `""`
* It is commonly used with optional chaining for safe and clean code

👉 It is a key feature in modern JavaScript for handling missing data safely and predictably.

---


## 13. Delete Operator

Removes object property.

```js
delete obj.name;
```

---

## 13. Delete Operator in JavaScript (Full Detailed Guide)

The **`delete` operator** in JavaScript is used to **remove properties from objects**. It can also be used to remove elements from arrays (but with important limitations).

It is a **unary operator** because it works on a single operand.

---

## 🔹 Syntax

```js id="d1"
delete object.property;
delete object["property"];
```

---

# 🚀 1. Basic Example (Object Property Deletion)

```js id="d2"
let user = {
  name: "John",
  age: 25
};

delete user.age;

console.log(user);
// { name: "John" }
```

👉 The `age` property is completely removed.

---

# 🔹 2. Using Bracket Notation

```js id="d3"
let user = {
  name: "John",
  age: 25
};

delete user["name"];

console.log(user);
// { age: 25 }
```

---

# 🔹 3. Return Value of delete Operator

The `delete` operator returns:

* `true` → if deletion was successful or property does not exist
* `false` → in strict mode for non-configurable properties

```js id="d4"
let obj = { a: 1 };

console.log(delete obj.a); // true
console.log(obj);          // {}
```

---

# 🔹 4. Deleting Non-Existing Property

```js id="d5"
let obj = { a: 1 };

console.log(delete obj.b); // true
```

👉 No error occurs.

---

# ⚠️ 5. delete DOES NOT Affect Variables

You cannot delete variables declared using `let`, `const`, or `var`.

```js id="d6"
let x = 10;

delete x; // ❌ ignored
console.log(x); // 10
```

---

# 🔹 6. delete with Global Object (var case)

```js id="d7"
var a = 5;

delete a; // ❌ may work in non-strict mode (browser dependent)
console.log(a);
```

👉 In modern JavaScript (strict mode), this is not allowed.

---

# 🔹 7. Deleting Array Elements

You can delete array elements, but it creates **empty slots** (not re-indexing the array).

---

## ❌ Using delete on arrays

```js id="d8"
let arr = [10, 20, 30];

delete arr[1];

console.log(arr); // [10, empty, 30]
```

👉 The index remains but becomes empty.

---

## ✔️ Better way (recommended)

Use `splice()` instead:

```js id="d9"
let arr = [10, 20, 30];

arr.splice(1, 1);

console.log(arr); // [10, 30]
```

---

# 🔹 8. Checking Property Removal

```js id="d10"
let obj = { name: "John" };

delete obj.name;

console.log("name" in obj); // false
```

---

# 🔹 9. delete and Non-Configurable Properties

Some properties cannot be deleted (like built-in or frozen properties).

```js id="d11"
"use strict";

const obj = {};

Object.defineProperty(obj, "id", {
  value: 1,
  configurable: false
});

console.log(delete obj.id); // false
```

---

# 🔹 10. delete with Nested Objects

```js id="d12"
let user = {
  profile: {
    name: "Alice",
    age: 30
  }
};

delete user.profile.age;

console.log(user.profile);
// { name: "Alice" }
```

---

# 🔹 11. Real-World Use Cases

---

## ✔️ Removing unwanted API fields

```js id="d13"
let response = {
  id: 1,
  password: "secret",
  name: "John"
};

delete response.password;

console.log(response);
```

---

## ✔️ Cleaning objects before sending data

```js id="d14"
let formData = {
  username: "john",
  tempToken: "abc123"
};

delete formData.tempToken;
```

---

## ✔️ Dynamic property removal

```js id="d15"
let key = "age";

let user = {
  name: "John",
  age: 25
};

delete user[key];
```

---

# ⚠️ Common Mistakes

---

## ❌ Using delete for variables

```js id="d16"
let x = 10;

delete x; // ❌ does nothing
```

---

## ❌ Expecting array re-indexing

```js id="d17"
let arr = [1, 2, 3];
delete arr[1];

console.log(arr.length); // 3 (not reduced)
```

---

## ❌ Deleting non-configurable properties

```js id="d18"
delete Math.PI; // ❌ false
```

---

# 🧠 Important Notes

* `delete` only works on **object properties**
* It does NOT free memory immediately (handled by garbage collector)
* It does NOT affect variable declarations
* It may create **holes in arrays**

---

# 🔹 delete vs Undefined

| Feature           | delete | set to undefined |
| ----------------- | ------ | ---------------- |
| Removes property  | ✔️     | ❌                |
| Keeps key         | ❌      | ✔️               |
| Affects structure | ✔️     | No               |

---

## Example:

```js id="d19"
let obj = { a: 1, b: 2 };

obj.a = undefined; // key still exists
delete obj.b;      // key removed
```

---

# ✅ Best Practices

✔ Use `delete` only for objects
✔ Prefer `splice()` for arrays
✔ Avoid deleting frequently in performance-critical code
✔ Use `undefined` if structure must remain intact
✔ Understand impact on object shape (performance)

---

# 📌 Summary

The `delete` operator is used to remove object properties in JavaScript. While powerful, it should be used carefully because it:

* Removes object properties permanently
* Does NOT work on variables
* Creates holes in arrays
* Can impact performance in optimized engines

👉 For clean and efficient code, use `delete` only when necessary and prefer alternative methods for arrays.

---


## 14. in Operator

Checks if property exists.

```js
"name" in obj;
```

---

## 14. `in` Operator in JavaScript (Full Detailed Guide)

The **`in` operator** in JavaScript is used to check whether a **property exists in an object or its prototype chain**. It returns a **Boolean value (`true` or `false`)**.

---

# 🔹 Syntax

```js id="in1"
propertyName in object
```

* `propertyName` → string or symbol (property to check)
* `object` → the object being checked

---

# 🚀 1. Basic Example

```js id="in2"
let user = {
  name: "John",
  age: 25
};

console.log("name" in user); // true
console.log("email" in user); // false
```

---

# 🔹 2. How `in` Works

The `in` operator checks:

✔ Object’s own properties
✔ Inherited properties (prototype chain)

---

## Example (Prototype Inheritance)

```js id="in3"
let parent = {
  greet: "Hello"
};

let child = Object.create(parent);

child.name = "John";

console.log("name" in child);  // true (own property)
console.log("greet" in child); // true (inherited property)
```

---

# 🔹 3. `in` vs Direct Property Access

```js id="in4"
let user = {
  name: "John",
  age: undefined
};

console.log(user.age);       // undefined
console.log("age" in user);  // true
```

👉 Important difference:

* Property exists → `in` returns `true`
* Value may still be `undefined`

---

# 🔹 4. Checking Array Indices

Arrays are objects in JavaScript, so `in` works with indexes.

```js id="in5"
let arr = [10, 20, 30];

console.log(0 in arr); // true
console.log(2 in arr); // true
console.log(5 in arr); // false
```

---

## ⚠️ Important: Sparse Arrays

```js id="in6"
let arr = [10, , 30]; // empty slot at index 1

console.log(1 in arr); // false
```

👉 Because index 1 does not exist.

---

# 🔹 5. `in` with Objects and Dynamic Keys

```js id="in7"
let user = {
  name: "Alice",
  age: 30
};

let key = "name";

console.log(key in user); // true
```

---

# 🔹 6. Checking Built-in Properties

```js id="in8"
console.log("toString" in {}); // true (from Object prototype)
```

---

# 🔹 7. `in` vs `hasOwnProperty()`

| Feature                  | `in` | `hasOwnProperty()` |
| ------------------------ | ---- | ------------------ |
| Own properties           | ✔️   | ✔️                 |
| Prototype properties     | ✔️   | ❌                  |
| Safer for pure own-check | ❌    | ✔️                 |

---

## Example:

```js id="in9"
let obj = { a: 1 };

console.log("a" in obj); // true
console.log(obj.hasOwnProperty("a")); // true
```

---

## Prototype difference:

```js id="in10"
console.log("toString" in obj); // true
console.log(obj.hasOwnProperty("toString")); // false
```

---

# 🔹 8. Real-World Use Cases

---

## ✔️ 1. Safe Property Check

```js id="in11"
let config = {
  darkMode: true
};

if ("darkMode" in config) {
  console.log("Theme exists");
}
```

---

## ✔️ 2. API Response Validation

```js id="in12"
let response = {
  data: {
    user: "John"
  }
};

if ("data" in response) {
  console.log("Data available");
}
```

---

## ✔️ 3. Optional Feature Detection

```js id="in13"
if ("fetch" in window) {
  console.log("Fetch API is supported");
}
```

---

## ✔️ 4. Checking Optional Keys

```js id="in14"
let user = {
  name: "John"
};

console.log("age" in user); // false
```

---

# 🔹 9. Common Mistakes

---

## ❌ Confusing with value check

```js id="in15"
let user = { age: undefined };

console.log(user.age === undefined); // true
console.log("age" in user); // true
```

👉 Property exists, even if value is undefined.

---

## ❌ Using in for arrays incorrectly

```js id="in16"
let arr = [10, 20];

console.log(10 in arr); // false ❌ (checks index, not value)
```

✔️ Correct way:

```js id="in17"
console.log(arr.includes(10)); // true
```

---

# 🔹 10. Important Notes

* `in` checks **keys/properties**, not values
* Works with objects and arrays
* Includes prototype chain
* Returns Boolean result

---

# 🧠 Key Insight

```js id="in18"
let obj = { a: undefined };

console.log("a" in obj); // true
console.log(obj.a);      // undefined
```

👉 `in` checks existence, not value

---

# ✅ Best Practices

✔ Use `in` to check if a property exists
✔ Use `hasOwnProperty()` for strict own-property checks
✔ Use `includes()` for array values
✔ Avoid using `in` for value searching in arrays
✔ Be aware of prototype chain behavior

---

# 📌 Summary

The `in` operator is used to check whether a property exists in an object or its prototype chain. It is very useful for:

* Property validation
* Feature detection
* Safe object access checks

However, it should be used carefully because it does NOT check values—only property existence.

---


## 15. Comma Operator

Evaluates multiple expressions.

```js
let x = (1, 2, 3); // 3
```

---

## 15. Comma Operator in JavaScript (Full Detailed Guide)

The **comma operator (`,`)** in JavaScript allows you to evaluate **multiple expressions in a single statement**. It evaluates each expression from left to right and returns the value of the **last expression**.

It is one of the least commonly used operators but is useful in specific advanced scenarios.

---

# 🔹 Syntax

```js id="co1"
expression1, expression2, expression3;
```

👉 Only the **last expression’s value is returned**.

---

# 🚀 1. Basic Example

```js id="co2"
let x = (1, 2, 3);

console.log(x); // 3
```

### 🔍 Explanation:

* `1` is evaluated
* `2` is evaluated
* `3` is evaluated
* Result of last expression (`3`) is returned

---

# 🔹 2. Multiple Expressions in a Line

```js id="co3"
let a = 10;
let b = 20;

let result = (a += 5, b += 10, a + b);

console.log(result); // 45
```

---

# 🔹 3. Comma Operator in Loops

It is commonly used in `for` loops to handle multiple variables.

```js id="co4"
for (let i = 0, j = 5; i < j; i++, j--) {
  console.log(i, j);
}
```

👉 Here, comma separates multiple expressions in initialization and increment.

---

# 🔹 4. Comma Operator in Variable Assignment

```js id="co5"
let x = (10, 20, 30);

console.log(x); // 30
```

---

# 🔹 5. Using Comma Operator for Side Effects

```js id="co6"
let x = 10;

let result = (console.log("Hello"), x * 2);

console.log(result); // 20
```

👉 First logs `"Hello"`, then returns `x * 2`.

---

# 🔹 6. Comma Operator vs Comma Separator

This is very important.

---

## ❌ Comma as Separator (NOT operator)

```js id="co7"
let a = 1, b = 2, c = 3;
```

👉 This is **not comma operator**, it's just variable declaration syntax.

---

## ✔️ Comma Operator (Expression)

```js id="co8"
let x = (1, 2, 3);
```

👉 This is the actual operator.

---

# 🔹 7. Comma Operator in Function Calls (Indirect Use)

```js id="co9"
function test() {
  return (console.log("A"), console.log("B"), "Done");
}

console.log(test());
```

Output:

```
A
B
Done
```

---

# 🔹 8. Comma Operator in Return Statements

```js id="co10"
function example() {
  return (1 + 2, 3 + 4);
}

console.log(example()); // 7
```

---

# 🔹 9. Real-World Use Cases

---

## ✔️ 1. Compact Loop Operations

```js id="co11"
for (let i = 0, j = 10; i < j; i++, j--) {
  console.log(i, j);
}
```

---

## ✔️ 2. Multiple Updates in One Expression

```js id="co12"
let a = 5;
let result = (a *= 2, a += 3, a);

console.log(result); // 13
```

---

## ✔️ 3. Logging + Calculation

```js id="co13"
let x = 10;

let output = (console.log("Processing..."), x * 3);

console.log(output); // 30
```

---

# ⚠️ Important Rules

---

## 🔹 1. Only Last Expression is Returned

```js id="co14"
let result = (1, 2, 3);
console.log(result); // 3
```

---

## 🔹 2. Parentheses Matter

Without parentheses, behavior changes:

```js id="co15"
let x = 1, 2, 3; // ❌ Syntax error or invalid usage
```

✔️ Correct:

```js id="co16"
let x = (1, 2, 3);
```

---

## 🔹 3. Low Priority Operator

The comma operator has the **lowest precedence** in JavaScript.

```js id="co17"
let x = 2 + 3, 4 + 5;
```

👉 Interpreted as:

```js id="co18"
(let x = 2 + 3), 4 + 5;
```

---

# 🧠 Common Mistakes

---

## ❌ Confusing with function arguments

```js id="co19"
console.log(1, 2, 3); // NOT comma operator
```

👉 This is a function argument list, not comma operator.

---

## ❌ Using it unnecessarily

```js id="co20"
let x = (a = 5, b = 10, a + b);
```

👉 Works, but reduces readability.

---

# 🔹 When NOT to Use It

Avoid comma operator when:

* Code becomes hard to read
* Multiple logical operations are involved
* Debugging is required

---

# ✅ Best Practices

✔ Use it only in `for` loops or advanced expressions
✔ Avoid overusing in production code
✔ Prefer readability over compactness
✔ Always use parentheses for clarity
✔ Use separate statements when possible

---

# 📌 Summary

The comma operator allows multiple expressions to be evaluated in a single statement, returning the last expression’s value. While powerful, it is rarely needed and should be used carefully to avoid reducing code readability.

* Evaluates expressions left → right
* Returns last expression
* Common in `for` loops
* Should be used sparingly

---


## 16. Void Operator

Evaluates expression and returns `undefined`.

```js
void(0); // undefined
```

---

## 16. Void Operator in JavaScript (Full Detailed Guide)

The **`void` operator** in JavaScript is used to evaluate an expression and **always return `undefined`**, regardless of what the expression produces.

It is a **unary operator**, meaning it works on a single operand.

---

# 🔹 Syntax

```js id="v1"
void expression
```

or

```js id="v2"
void(expression)
```

---

# 🚀 1. Basic Example

```js id="v3"
console.log(void 0); // undefined
```

👉 Even though `0` is a valid value, `void` forces the result to be `undefined`.

---

# 🔹 2. Void with Expressions

```js id="v4"
console.log(void (2 + 2)); // undefined
```

👉 The expression `2 + 2` is evaluated, but result is discarded.

---

# 🔹 3. How Void Works

The `void` operator:

1. Evaluates the expression
2. Discards its result
3. Returns `undefined`

---

## Example:

```js id="v5"
let x = void (10 + 5);

console.log(x); // undefined
```

---

# 🔹 4. Void in JavaScript Links (Important Use Case)

One of the most common uses is in HTML links to prevent navigation.

```html id="v6"
<a href="javascript:void(0)">Click Me</a>
```

👉 This prevents the page from reloading or navigating.

---

## Why it is used:

* Stops default link behavior
* Keeps the UI interactive without page reload

---

# 🔹 5. Void in Event Handlers

```html id="v7"
<button onclick="void alert('Hello')">Click</button>
```

👉 The alert runs, but return value is ignored.

---

# 🔹 6. Void with Functions

```js id="v8"
function test() {
  return 10;
}

let result = void test();

console.log(result); // undefined
```

👉 Function runs, but result is discarded.

---

# 🔹 7. Preventing Return Values

```js id="v9"
let x = void (() => 100)();

console.log(x); // undefined
```

---

# 🔹 8. Void vs Undefined

| Feature | `void`              | `undefined`                 |
| ------- | ------------------- | --------------------------- |
| Type    | Operator            | Value                       |
| Result  | Always undefined    | May change                  |
| Use     | Force ignore result | Represents absence of value |

---

## Example:

```js id="v10"
console.log(void 1);      // undefined
console.log(undefined);   // undefined
```

---

# 🔹 9. Real-World Use Cases

---

## ✔️ 1. Prevent Default Link Navigation

```html id="v11"
<a href="javascript:void(0)">Do Nothing</a>
```

---

## ✔️ 2. Ignoring Function Return Value

```js id="v12"
void someFunction();
```

---

## ✔️ 3. IIFE Style Ignoring Result

```js id="v13"
void function () {
  console.log("Running...");
}();
```

---

## ✔️ 4. Debugging / Side Effects Only

```js id="v14"
void console.log("Debug message");
```

---

# 🔹 10. Void in Arrow Functions

```js id="v15"
let result = void (() => 5)();

console.log(result); // undefined
```

---

# ⚠️ Important Rules

---

## ❌ Cannot assign meaningful value

```js id="v16"
let x = void 10; // always undefined
```

---

## ❌ Not used for computations

```js id="v17"
let x = void (5 + 5);
console.log(x); // undefined
```

---

## ❌ Not a replacement for undefined checks

```js id="v18"
if (x === void 0) {
  console.log("x is undefined");
}
```

---

# 🔹 11. Operator Precedence

The `void` operator has **very high precedence**, similar to other unary operators.

```js id="v19"
console.log(void 2 + 3); // undefined + 3 → NaN
```

👉 Better:

```js id="v20"
console.log(void (2 + 3)); // undefined
```

---

# 🧠 Common Mistakes

---

## ❌ Confusing void with return

```js id="v21"
function test() {
  return void 10;
}
```

👉 Returns undefined, not 10.

---

## ❌ Using without understanding

```js id="v22"
void 0; // unnecessary in modern code
```

---

# 🔹 12. Why `void 0` is popular

```js id="v23"
void 0
```

👉 Always returns `undefined` safely
👉 Shorter than writing `undefined`
👉 Cannot be overridden

---

# ✅ Best Practices

✔ Use `void` only when you need to discard values
✔ Prefer modern event handling instead of `javascript:void(0)`
✔ Use `void 0` only in rare compatibility cases
✔ Avoid using it in everyday logic
✔ Prefer `undefined` directly for clarity

---

# 📌 Summary

The `void` operator evaluates an expression but always returns `undefined`. It is mostly used to:

* Prevent navigation in links
* Ignore function results
* Ensure a safe `undefined` value (`void 0`)

However, in modern JavaScript, its usage is limited and mostly replaced by better practices.

---


## 17. Await Operator

Used in async functions.

```js
let data = await fetch(url);
```

---

## 17. `await` Operator in JavaScript (Full Detailed Guide)

The **`await` operator** is used in JavaScript to **pause the execution of an async function until a Promise is resolved or rejected**. It is a key part of modern asynchronous programming introduced with **ES2017 (ES8)**.

It makes asynchronous code look and behave more like synchronous code.

---

# 🔹 What is `await`?

`await` can only be used inside an **`async` function** (or top-level in modern modules).

It waits for a **Promise** and returns its resolved value.

---

# 🔹 Syntax

```js id="aw1"
let result = await promise;
```

---

# 🚀 1. Basic Example

```js id="aw2"
async function test() {
  let promise = Promise.resolve("Hello World");

  let result = await promise;

  console.log(result);
}

test();
```

### Output:

```
Hello World
```

---

# 🔹 2. How `await` Works

When JavaScript sees `await`:

1. It pauses execution inside the async function
2. Waits for the Promise to resolve or reject
3. Resumes execution with the result

---

## Example Flow:

```js id="aw3"
async function demo() {
  console.log("Start");

  let result = await new Promise(resolve =>
    setTimeout(() => resolve("Done"), 2000)
  );

  console.log(result);
  console.log("End");
}

demo();
```

### Output:

```
Start
Done (after 2 seconds)
End
```

---

# 🔹 3. `await` with Fetch API

One of the most common real-world uses.

```js id="aw4"
async function getData() {
  let response = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  let data = await response.json();

  console.log(data);
}

getData();
```

---

# 🔹 4. Error Handling with `await`

Use `try...catch` to handle errors.

```js id="aw5"
async function getData() {
  try {
    let response = await fetch("invalid-url");
    let data = await response.json();

    console.log(data);
  } catch (error) {
    console.log("Error:", error);
  }
}
```

---

# 🔹 5. `await` vs `.then()`

| Feature        | `await`    | `.then()`      |
| -------------- | ---------- | -------------- |
| Syntax         | Cleaner    | Callback-based |
| Readability    | High       | Medium         |
| Flow           | Sequential | Chained        |
| Error handling | try/catch  | .catch()       |

---

## Example Comparison

### Using `.then()`

```js id="aw6"
fetch(url)
  .then(res => res.json())
  .then(data => console.log(data));
```

### Using `await`

```js id="aw7"
let res = await fetch(url);
let data = await res.json();
console.log(data);
```

---

# 🔹 6. Multiple `await` Calls

```js id="aw8"
async function demo() {
  let a = await Promise.resolve(10);
  let b = await Promise.resolve(20);

  console.log(a + b);
}

demo();
```

---

# ⚠️ 7. Sequential vs Parallel Execution

---

## ❌ Sequential (Slower)

```js id="aw9"
let a = await fetch(url1);
let b = await fetch(url2);
```

---

## ✔️ Parallel (Faster)

```js id="aw10"
let [a, b] = await Promise.all([
  fetch(url1),
  fetch(url2)
]);
```

---

# 🔹 8. `await` Only Works Inside Async Functions

---

## ❌ Invalid

```js id="aw11"
let result = await Promise.resolve(10); // ❌ Error
```

---

## ✔️ Valid

```js id="aw12"
async function test() {
  let result = await Promise.resolve(10);
}
```

---

## ✔️ Top-Level Await (Modern JS Modules)

```js id="aw13"
// Only in ES Modules
let data = await fetch("https://api.example.com");
```

---

# 🔹 9. Awaiting Non-Promises

If you `await` a normal value, it is automatically wrapped in a Promise.

```js id="aw14"
async function test() {
  let result = await 5;

  console.log(result); // 5
}

test();
```

---

# 🔹 10. Real-World Use Cases

---

## ✔️ 1. API Calls

```js id="aw15"
async function loadUser() {
  let res = await fetch("/api/user");
  let user = await res.json();

  console.log(user);
}
```

---

## ✔️ 2. Database Queries (Backend)

```js id="aw16"
let user = await User.findById(id);
```

---

## ✔️ 3. Delay Execution

```js id="aw17"
function wait(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function run() {
  console.log("Start");
  await wait(2000);
  console.log("After 2 seconds");
}

run();
```

---

## ✔️ 4. Sequential Steps Workflow

```js id="aw18"
async function process() {
  await step1();
  await step2();
  await step3();
}
```

---

# 🔹 11. Error Behavior

If a Promise is rejected:

```js id="aw19"
async function test() {
  await Promise.reject("Failed"); // throws error
}
```

👉 Must be handled with `try...catch`.

---

# 🔹 12. Common Mistakes

---

## ❌ Forgetting async keyword

```js id="aw20"
function test() {
  let x = await 10; // ❌ Error
}
```

---

## ❌ Not handling errors

```js id="aw21"
let data = await fetch(url); // may crash if fails
```

---

## ❌ Sequential API calls when not needed

```js id="aw22"
await fetch(a);
await fetch(b);
```

---

# 🧠 Key Concepts

* `await` pauses execution inside async function
* Only works with Promises
* Makes async code look synchronous
* Helps avoid callback hell
* Can improve readability significantly

---

# ⚖️ await vs async

| Keyword | Purpose                           |
| ------- | --------------------------------- |
| `async` | Declares function as asynchronous |
| `await` | Waits for Promise result          |

---

# ✅ Best Practices

✔ Always use inside `async` functions
✔ Use `try...catch` for error handling
✔ Use `Promise.all()` for parallel tasks
✔ Avoid unnecessary sequential `await`
✔ Prefer `await` for readability over `.then()`

---

# 📌 Summary

The `await` operator is a powerful JavaScript feature used to handle asynchronous operations in a clean and readable way. It pauses function execution until a Promise resolves, making async code easier to write and understand.

* Works only inside `async` functions
* Waits for Promises
* Improves readability
* Essential for API calls and async workflows

---


## 18. Yield Operator

Used in generators.

```js
function* gen() {
  yield 1;
}
```

---

##18. `yield` Operator in JavaScript (Full Detailed Guide)

The **`yield` operator** in JavaScript is used inside **generator functions** to **pause execution and return a value**, and later **resume from the same point**.

It is a key feature of **Generator Functions (`function*`)** introduced in ES6.

---

# 🔹 What is `yield`?

* `yield` pauses a generator function
* It returns a value to the caller
* Execution resumes when `.next()` is called again

---

# 🔹 Syntax

```js id="y1"
function* generatorFunction() {
  yield value;
}
```

---

# 🚀 1. Basic Example

```js id="y2"
function* demo() {
  yield 1;
  yield 2;
  yield 3;
}

let gen = demo();

console.log(gen.next()); // { value: 1, done: false }
console.log(gen.next()); // { value: 2, done: false }
console.log(gen.next()); // { value: 3, done: false }
console.log(gen.next()); // { value: undefined, done: true }
```

---

# 🔹 2. How `yield` Works

When `yield` is encountered:

1. Function pauses
2. Value is returned
3. Execution resumes from same point on next `.next()`

---

## Execution Flow

```js id="y3"
function* test() {
  console.log("Start");

  yield 1;
  console.log("Middle");

  yield 2;
  console.log("End");
}
```

```js id="y4"
let gen = test();

gen.next(); // Start → returns 1
gen.next(); // Middle → returns 2
gen.next(); // End
```

---

# 🔹 3. Generator Function (`function*`)

`yield` only works inside generator functions.

```js id="y5"
function* generator() {
  yield "A";
  yield "B";
}
```

---

# 🔹 4. Yielding Values Dynamically

```js id="y6"
function* numbers() {
  let x = 10;
  yield x;

  x += 5;
  yield x;
}

let gen = numbers();

console.log(gen.next().value); // 10
console.log(gen.next().value); // 15
```

---

# 🔹 5. Passing Values into `yield`

You can send values back into the generator.

```js id="y7"
function* demo() {
  let x = yield "Enter first value";
  let y = yield "Enter second value";

  return x + y;
}

let gen = demo();

console.log(gen.next().value);    // Enter first value
console.log(gen.next(10).value);   // Enter second value
console.log(gen.next(20).value);   // 30
```

---

# 🔹 6. `yield` vs `return`

| Feature             | `yield`    | `return`          |
| ------------------- | ---------- | ----------------- |
| Pauses function     | ✔️         | ❌                 |
| Continues execution | ✔️         | ❌ (ends function) |
| Multiple values     | ✔️         | ❌                 |
| Used in             | Generators | Normal functions  |

---

## Example:

```js id="y8"
function* test() {
  yield 1;
  return 2;
  yield 3; // never executed
}
```

---

# 🔹 7. Iterating with `for...of`

Generators can be iterated easily.

```js id="y9"
function* nums() {
  yield 1;
  yield 2;
  yield 3;
}

for (let n of nums()) {
  console.log(n);
}
```

### Output:

```
1
2
3
```

---

# 🔹 8. Infinite Generators

```js id="y10"
function* infinite() {
  let i = 0;

  while (true) {
    yield i++;
  }
}

let gen = infinite();

console.log(gen.next().value); // 0
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
```

---

# 🔹 9. Real-World Use Cases

---

## ✔️ 1. ID Generators

```js id="y11"
function* idGenerator() {
  let id = 1;

  while (true) {
    yield id++;
  }
}

let gen = idGenerator();

console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
```

---

## ✔️ 2. Pagination Systems

```js id="y12"
function* pages() {
  yield "Page 1";
  yield "Page 2";
  yield "Page 3";
}
```

---

## ✔️ 3. Lazy Evaluation

```js id="y13"
function* lazyNumbers() {
  yield 1;
  yield 2;
  yield 3;
}
```

👉 Values generated only when needed.

---

## ✔️ 4. Async Flow Control (Advanced)

```js id="y14"
function* flow() {
  yield "Step 1";
  yield "Step 2";
  yield "Step 3";
}
```

---

# 🔹 10. Generator Object Methods

```js id="y15"
let gen = (function* () {
  yield 1;
  yield 2;
})();

console.log(gen.next());
console.log(gen.return(100));
console.log(gen.next());
```

---

## Methods:

| Method      | Description                   |
| ----------- | ----------------------------- |
| `.next()`   | Moves execution forward       |
| `.return()` | Ends generator early          |
| `.throw()`  | Throws error inside generator |

---

# 🔹 11. Handling Errors with yield

```js id="y16"
function* demo() {
  try {
    yield 1;
  } catch (e) {
    console.log("Error:", e);
  }
}

let gen = demo();

gen.next();
gen.throw("Something went wrong");
```

---

# 🔹 12. Important Rules

---

## ❌ Cannot use yield outside generator

```js id="y17"
yield 10; // ❌ Error
```

---

## ❌ Must use function*

```js id="y18"
function test() {
  yield 1; // ❌ invalid
}
```

---

# 🧠 Key Concepts

* `yield` pauses execution
* Works only inside `function*`
* Returns `{ value, done }`
* Can resume execution
* Enables lazy and step-by-step computation

---

# ⚖️ yield vs await

| Feature          | `yield`      | `await`         |
| ---------------- | ------------ | --------------- |
| Used in          | Generators   | Async functions |
| Pauses execution | ✔️           | ✔️              |
| Works with       | Iteration    | Promises        |
| Returns          | Value object | Resolved value  |

---

# ✅ Best Practices

✔ Use for lazy iteration
✔ Use for generators and streams
✔ Avoid overusing in simple code
✔ Combine with `for...of` for clean iteration
✔ Prefer `async/await` for Promises

---

# 📌 Summary

The `yield` operator is used in generator functions to pause and resume execution, allowing values to be produced step-by-step instead of all at once.

* Works only inside `function*`
* Produces multiple values over time
* Enables lazy evaluation
* Useful for iterators and advanced control flows

👉 It is a powerful tool for managing complex iteration and flow control in JavaScript.

---


## 19. Operator Precedence

Defines execution order.

Example:

```js
let result = 2 + 3 * 4; // 14
```

Use parentheses:

```js
let result = (2 + 3) * 4; // 20
```

---

## 19. Operator Precedence in JavaScript (Full Detailed Guide)

**Operator precedence** in JavaScript defines the **order in which operators are evaluated in an expression**.

When multiple operators appear in the same expression, JavaScript uses precedence rules to decide which part is executed first.

---

# 🔹 What is Operator Precedence?

It answers this question:

> “Which operator should be evaluated first?”

---

## 🔹 Example

```js id="p1"
let result = 10 + 5 * 2;

console.log(result); // 20
```

### Why?

* `*` has higher precedence than `+`
* So: `5 * 2 = 10`
* Then: `10 + 10 = 20`

---

# 🔹 Operator Precedence Table (High → Low)

| Priority    | Operator Type      | Operators                                               |   |   |
| ----------- | ------------------ | ------------------------------------------------------- | - | - |
| 1 (Highest) | Grouping           | `( )`                                                   |   |   |
| 2           | Member Access      | `.` `[]`                                                |   |   |
| 3           | New (with args)    | `new`                                                   |   |   |
| 4           | Function Call      | `()`                                                    |   |   |
| 5           | Optional Chaining  | `?.`                                                    |   |   |
| 6           | Postfix            | `x++`, `x--`                                            |   |   |
| 7           | Unary              | `++x`, `--x`, `!`, `typeof`, `void`, `delete`, `+`, `-` |   |   |
| 8           | Exponentiation     | `**`                                                    |   |   |
| 9           | Multiplicative     | `*`, `/`, `%`                                           |   |   |
| 10          | Additive           | `+`, `-`                                                |   |   |
| 11          | Shift              | `<<`, `>>`, `>>>`                                       |   |   |
| 12          | Relational         | `<`, `<=`, `>`, `>=`, `in`, `instanceof`                |   |   |
| 13          | Equality           | `==`, `!=`, `===`, `!==`                                |   |   |
| 14          | Bitwise AND        | `&`                                                     |   |   |
| 15          | Bitwise XOR        | `^`                                                     |   |   |
| 16          | Bitwise OR         | `                                                       | ` |   |
| 17          | Logical AND        | `&&`                                                    |   |   |
| 18          | Logical OR         | `                                                       |   | ` |
| 19          | Nullish Coalescing | `??`                                                    |   |   |
| 20          | Conditional        | `? :`                                                   |   |   |
| 21 (Lowest) | Assignment         | `=`, `+=`, `-=`, `*=`, `/=`, etc.                       |   |   |
| 22          | Comma              | `,`                                                     |   |   |

---

# 🚀 1. Grouping Operator `( )`

Parentheses have the **highest priority**.

```js id="p2"
let result = (10 + 5) * 2;

console.log(result); // 30
```

👉 Forces `10 + 5` first.

---

# 🔹 2. Function Calls and Member Access

```js id="p3"
console.log(Math.max(10, 20));
```

Order:

1. `Math.max` accessed
2. Function called

---

# 🔹 3. Unary vs Binary Confusion

```js id="p4"
let x = 5;
let y = x + 2 * 3;
```

* `*` happens first
* Then `+`

---

# 🔹 4. Exponentiation (`**`)

```js id="p5"
console.log(2 + 3 ** 2); // 11
```

* `3 ** 2 = 9`
* then `2 + 9 = 11`

---

# 🔹 5. Relational Operators

```js id="p6"
console.log(5 > 3 && 2 < 4);
```

Evaluation:

* `5 > 3` → true
* `2 < 4` → true
* then `&&`

---

# 🔹 6. Logical Operators

```js id="p7"
console.log(true || false && false);
```

* `&&` evaluated first
* then `||`

Result: `true`

---

# 🔹 7. Nullish Coalescing (`??`)

```js id="p8"
let value = null ?? 10 || 20;
```

⚠️ Requires parentheses in mixed cases.

---

# 🔹 8. Conditional (Ternary)

```js id="p9"
let result = 10 > 5 ? "A" : "B";
```

* Condition evaluated first
* Then one branch selected

---

# 🔹 9. Assignment (Low Priority)

```js id="p10"
let x = 10 + 5 * 2;
```

* RHS fully evaluated first
* Then assigned

---

# 🔹 10. Postfix vs Prefix

```js id="p11"
let x = 5;

console.log(x++); // 5
console.log(++x); // 7
```

* Postfix has lower precedence than prefix

---

# ⚖️ 11. Associativity (Direction of Evaluation)

When operators have the same precedence, associativity decides direction.

---

## 🔹 Left-to-Right

```js id="p12"
let result = 10 - 5 - 2;
```

Step:

* (10 - 5) = 5
* (5 - 2) = 3

---

## 🔹 Right-to-Left

```js id="p13"
let x = 2 ** 3 ** 2;
```

Step:

* 3 ** 2 = 9
* 2 ** 9 = 512

---

# 🔹 12. Complex Expression Example

```js id="p14"
let result = 10 + 5 * 2 ** 3 > 20 && true || false;
```

Step-by-step:

1. `2 ** 3 = 8`
2. `5 * 8 = 40`
3. `10 + 40 = 50`
4. `50 > 20 = true`
5. `true && true = true`
6. `true || false = true`

Final result: `true`

---

# 🔹 13. Why Precedence Matters

Without precedence rules, expressions would be ambiguous.

```js id="p15"
10 + 5 * 2
```

Could mean:

* `(10 + 5) * 2` ❌
* `10 + (5 * 2)` ✔️

---

# ⚠️ Common Mistakes

---

## ❌ Ignoring precedence

```js id="p16"
let result = 10 + 5 * 2;
```

👉 People often assume left-to-right incorrectly.

---

## ❌ Mixing logical operators

```js id="p17"
true || false && true
```

👉 `&&` runs first.

---

## ❌ Not using parentheses for clarity

```js id="p18"
let x = a + b * c / d - e;
```

👉 Hard to read → better with parentheses.

---

# 🧠 Key Concepts

* Higher precedence operators execute first
* Parentheses override everything
* Same-level operators follow associativity rules
* Logical and arithmetic operators follow different priorities

---

# ✅ Best Practices

✔ Use parentheses for clarity
✔ Avoid writing complex one-line expressions
✔ Learn precedence for debugging
✔ Prefer readable code over clever code
✔ Break complex logic into steps

---

# 📌 Summary

Operator precedence in JavaScript defines the order in which operations are performed in an expression. It ensures consistent evaluation results.

* `()` has highest priority
* Arithmetic > comparison > logical > assignment
* Associativity decides direction when same level operators exist

👉 Understanding precedence is essential for writing correct and predictable JavaScript code.

---


## Conclusion

JavaScript operators are powerful tools for performing operations on data. Understanding them deeply helps you write clean, efficient, and bug-free code.

---

## Pro Tip

Prefer `===` over `==` to avoid unexpected type coercion issues.

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

