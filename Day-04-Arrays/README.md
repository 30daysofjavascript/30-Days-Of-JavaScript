# 🚀 Day 04 — Arrays

### 📚 30 Days of JavaScript: Beginner to Advanced

---

## 📦 1. Creating Arrays

An **array** is an ordered collection of values (any type).

```js id="a1b2c3"
let fruits = ["apple", "banana", "cherry"];
let numbers = [1, 2, 3, 4, 5];
let mixed = [42, "hello", true, null, { name: "Alice" }];
let empty = [];
```

---

### 🏗️ Array Constructor

```js id="d4e5f6"
let arr = new Array(3);        // [empty × 3]
let arr2 = new Array(1, 2, 3); // [1, 2, 3]
```

---

## 🔍 2. Accessing & Modifying

```js id="g7h8i9"
let colors = ["red", "green", "blue"];

console.log(colors[0]); // "red"
console.log(colors[2]); // "blue"

colors[1] = "yellow";
console.log(colors);
```

---

### ⚠️ Out of Bounds

```js id="j1k2l3"
console.log(colors[10]); // undefined
```

---

## ➕➖ 3. Adding & Removing Elements

```js id="m4n5o6"
let animals = ["cat", "dog"];

animals.push("bird");   // add to end
animals.pop();          // remove from end

animals.unshift("fish"); // add to start
animals.shift();         // remove from start
```

---

### ⚡ Performance Tip

* ✅ `push` / `pop` → FAST
* ⚠️ `shift` / `unshift` → SLOW (re-indexing)

---

### ➕ Multiple Add

```js id="p7q8r9"
animals.push("bird", "rabbit", "hamster");
```

---

## 🔧 4. splice() — All-in-One Tool

```js id="s1t2u3"
let nums = [1, 2, 3, 4, 5];

// Remove
nums.splice(1, 2); // [2,3]

// Insert
nums.splice(1, 0, 10, 20);

// Replace
nums.splice(2, 1, 99);
```

---

## ✂️ 5. slice() — Non-Destructive

```js id="v4w5x6"
let letters = ["a", "b", "c", "d", "e"];

letters.slice(1, 3);
letters.slice(2);
letters.slice(-2);

let copy = letters.slice();
```

---

## 🔎 6. Searching Arrays

```js id="y7z8a9"
let scores = [85, 92, 78, 92, 65, 92];

scores.indexOf(92);
scores.lastIndexOf(92);
scores.includes(78);
```

---

### 🔍 Advanced Search

```js id="b1c2d3"
scores.find(score => score > 90);
scores.findIndex(score => score > 90);
scores.findLast(score => score > 90);
```

---

## 🔄 7. Sorting Arrays

```js id="e4f5g6"
let fruits2 = ["banana", "apple", "cherry"];
fruits2.sort();
```

---

### ⚠️ Numbers Sorting Issue

```js id="h7i8j9"
let numArr = [100, 20, 3, 1000, 50];

numArr.sort(); // ❌ wrong
numArr.sort((a, b) => a - b); // ✅ ascending
numArr.sort((a, b) => b - a); // ✅ descending
```

---

### 🔁 Reverse

```js id="k1l2m3"
let arr3 = [1, 2, 3, 4, 5];
arr3.reverse();
```

---

## 🔗 8. Joining & Converting

```js id="n4o5p6"
let words = ["Hello", "World", "JavaScript"];

words.join(" ");
words.join(", ");
words.toString();
```

---

### 🔄 String → Array

```js id="q7r8s9"
let str = "a,b,c";
let arr4 = str.split(",");
```

---

## 🔗 9. Combining Arrays

```js id="t1u2v3"
let arr5 = [1, 2, 3];
let arr6 = [4, 5, 6];

let combined = arr5.concat(arr6);
```

---

### ✨ Spread Operator (Modern)

```js id="w4x5y6"
let combined2 = [...arr5, ...arr6];
```

---

## ✅ 10. Checking Arrays

```js id="z7a8b9"
Array.isArray([1, 2, 3]); // true
Array.isArray("hello");   // false

typeof []; // "object" ⚠️
```

---

## 🔁 11. Iterating Arrays

```js id="c1d2e3"
let nums2 = [10, 20, 30, 40];

// for loop
for (let i = 0; i < nums2.length; i++) {
  console.log(nums2[i]);
}
```

---

### 🔄 Modern Ways

```js id="f4g5h6"
for (let num of nums2) {
  console.log(num);
}

nums2.forEach((num, index) => {
  console.log(index, num);
});
```

---

## 🧠 12. Useful Methods

### 📦 flat()

```js id="i7j8k9"
let nested = [1, [2, 3], [4, [5, 6]]];

nested.flat();
nested.flat(2);
nested.flat(Infinity);
```

---

### 🎯 fill()

```js id="l1m2n3"
let filled = new Array(5).fill(0);

let arr8 = [1, 2, 3, 4, 5];
arr8.fill(9, 2, 4);
```

---

### ✔️ every() & some()

```js id="o4p5q6"
[1, 2, 3].every(n => n > 0);

[1, -2, 3].some(n => n < 0);
```

---

## 📝 Exercises

---

### 🧪 Exercise 1

Create array of 5 numbers:

* Add to front & back
* Remove from front & back

---

### 🧪 Exercise 2

```js id="r7s8t9"
let arr = [1, 2, 3, 4, 5];
```

👉 Remove `3` using `splice`

---

### 🧪 Exercise 3

Sort by age:

```js id="u1v2w3"
[
 {name:"Alice", age:30},
 {name:"Bob", age:25},
 {name:"Charlie", age:35}
]
```

---

### 🧪 Exercise 4

Remove duplicates:

```js id="x4y5z6"
[1, 2, 2, 3, 4, 4, 5]
```

---

### 🧪 Exercise 5

Flatten:

```js id="a7b8c9"
[1, [2, [3, [4, [5]]]]]
```

---

## ⭐ Support

If you found this helpful:

👉 Give this repo a ⭐
👉 Share it with others 🚀
👉 Keep coding 💻

---

## 🎉 Day 04 Complete!

Now you understand:

* Arrays & indexing
* Adding/removing elements
* Searching & sorting
* Iteration & powerful methods

👉 Next: **Objects Deep Dive** 🔥
