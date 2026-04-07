# 🚀 Day 05 — Objects

### 📚 30 Days of JavaScript: Beginner to Advanced

---

## 🧠 1. What is an Object?

An **object** is a collection of **key-value pairs**.

* 🔑 Keys → strings (or Symbols)
* 📦 Values → anything (string, number, array, function, object, etc.)

---

### 🏗️ Creating an Object

```js id="o1p2q3"
let person = {
  name: "Alice",
  age: 30,
  isStudent: false,
  hobbies: ["reading", "coding"],
  address: {
    city: "Wonderland",
    zip: "12345"
  },
  greet: function() {
    return `Hello, I'm ${this.name}`;
  }
};

console.log(person.name);
console.log(person.address.city);
console.log(person.greet());
```

---

## 🔍 2. Accessing Properties

```js id="r4s5t6"
let car = { make: "Toyota", model: "Camry", year: 2022 };

// Dot notation
car.make;

// Bracket notation
car["model"];

// Dynamic key
let key = "make";
car[key];
```

---

### ⚠️ Special Cases

```js id="u7v8w9"
let weirdObj = {
  "first name": "Alice",
  "123": "number key",
  "class": "special keyword"
};

weirdObj["first name"];
weirdObj["123"];
```

---

## ➕➖ 3. Add, Update, Delete

```js id="x1y2z3"
let obj = { a: 1, b: 2 };

// Add
obj.c = 3;

// Update
obj.a = 100;

// Delete
delete obj.b;
```

---

### ✅ Check Properties

```js id="a4b5c6"
"a" in obj;
obj.hasOwnProperty("c");
```

---

## ⚙️ 4. Methods (Functions in Objects)

```js id="d7e8f9"
let calculator = {
  value: 0,

  add(n) {
    this.value += n;
    return this;
  },

  subtract(n) {
    this.value -= n;
    return this;
  },

  multiply(n) {
    this.value *= n;
    return this;
  },

  getResult() {
    return this.value;
  }
};

let result = calculator.add(10).multiply(3).subtract(5).getResult();
console.log(result); // 25
```

---

## 🧭 5. The `this` Keyword

```js id="g1h2i3"
let user = {
  name: "Bob",
  age: 28,

  introduce() {
    console.log(`I'm ${this.name}, age ${this.age}`);
  },

  arrowIntroduce: () => {
    console.log(this); // ❌ not user object
  }
};
```

---

### ⚠️ Rule

* ✅ Use **normal functions** for object methods
* ❌ Avoid arrow functions for methods

---

## 🔁 6. Object Iteration

```js id="j4k5l6"
let student = {
  name: "Charlie",
  grade: "A",
  score: 95
};

for (let key in student) {
  console.log(key, student[key]);
}
```

---

### 📦 Built-in Methods

```js id="m7n8o9"
Object.keys(student);
Object.values(student);
Object.entries(student);
```

---

### 🔄 Entries Loop

```js id="p1q2r3"
for (let [key, value] of Object.entries(student)) {
  console.log(key, value);
}
```

---

## 📋 7. Copying Objects

```js id="s4t5u6"
let original = { name: "Alice", age: 25 };

// ❌ Reference copy
let same = original;

// ✅ Shallow copy
let copy1 = Object.assign({}, original);
let copy2 = { ...original };
```

---

### ⚠️ Shallow Copy Problem

```js id="v7w8x9"
let deepObj = { name: "Alice", address: { city: "NY" } };

let shallowCopy = { ...deepObj };
shallowCopy.address.city = "LA"; // affects original!
```

---

### ✅ Deep Copy

```js id="y1z2a3"
// JSON method
let deepCopy = JSON.parse(JSON.stringify(deepObj));

// Modern way
let deepCopy2 = structuredClone(deepObj);
```

---

## 🧰 8. Object Static Methods

```js id="b4c5d6"
// Merge
Object.assign({}, {a:1}, {b:2});

// Freeze
let config = Object.freeze({ apiKey: "abc123" });

// From entries
Object.fromEntries([["name","Alice"],["age",25]]);
```

---

### 💡 Transform Example

```js id="e7f8g9"
let prices = { apple: 1.5, banana: 1 };

let doubled = Object.fromEntries(
  Object.entries(prices).map(([k,v]) => [k, v * 2])
);
```

---

## ✨ 9. Shorthand Properties

```js id="h1i2j3"
let firstName = "Alice";
let lastName = "Smith";

let person = { firstName, lastName };
```

---

## 🧮 10. Computed Properties

```js id="k4l5m6"
let prop = "color";

let obj = {
  [prop]: "blue",
  [`${prop}Code`]: "#0000ff"
};
```

---

## 📝 Exercises

---

### 🧪 Exercise 1

Create a **book object** with:

* title, author, year, pages
* method: `getSummary()`

---

### 🧪 Exercise 2

Find highest score:

```js id="n7o8p9"
[
 {name:"Alice", score:85},
 {name:"Bob", score:92},
 {name:"Charlie", score:78}
]
```

---

### 🧪 Exercise 3

Merge objects:

```js id="q1r2s3"
{a:1, b:2}, {b:3, c:4}, {c:5, d:6}
```

---

### 🧪 Exercise 4

Count characters:

```js id="t4u5v6"
"hello"
```

---

### 🧪 Exercise 5

Deep clone:

```js id="w7x8y9"
{name:"Alice", scores:[1,2,3], address:{city:"NY"}}
```

---

## ⭐ Support

If you found this helpful:

👉 Give this repo a ⭐
👉 Share with others 🚀
👉 Keep learning 💻

---

## 🎉 Day 05 Complete!

Now you understand:

* Objects & properties
* Methods & `this`
* Iteration & copying
* Modern ES6 features

👉 Next: **Functions Deep Dive** 🔥
