# 🚀 30 Days of JavaScript — Beginner to Advanced

> 🎯 **Master JavaScript step-by-step in 30 days**  
> From absolute beginner → advanced concepts → real-world project

---

## 📚 Course Roadmap

### 🟢 Beginner (Days 1–6)
- Day 01 — [Variables & Data Types](https://github.com/30daysofjavascript/30-Days-Of-JavaScript/tree/main/Day-01-Variables-DataTypes)  
- Day 02 — [Operators](https://github.com/30daysofjavascript/30-Days-Of-JavaScript/tree/main/Day-02-Operators)  
- Day 03 — Strings & Methods  
- Day 04 — Arrays  
- Day 05 — Objects  
- Day 06 — Functions  

---

### 🟡 Intermediate (Days 7–15)
- Day 07 — Scope & Hoisting  
- Day 08 — Arrow Functions  
- Day 09 — Array Methods  
- Day 10 — Destructuring  
- Day 11 — Spread & Rest  
- Day 12 — DOM Basics  
- Day 13 — DOM Events  
- Day 14 — Forms & Validation  
- Day 15 — ES6 Classes  

---

### 🟠 Advanced (Days 16–23)
- Day 16 — Prototypes & Inheritance  
- Day 17 — Promises  
- Day 18 — Async / Await  
- Day 19 — Fetch API  
- Day 20 — Error Handling  
- Day 21 — Modules  
- Day 22 — LocalStorage  
- Day 23 — Regex  

---

### 🔴 Expert (Days 24–30)
- Day 24 — Closures  
- Day 25 — Higher-Order Functions  
- Day 26 — Iterators & Generators  
- Day 27 — Map & Set  
- Day 28 — WeakMap & WeakSet  
- Day 29 — Design Patterns  
- Day 30 — 🚀 Final Project  

---

## ✨ What Makes This Course Special?

- 💡 Beginner-friendly explanations  
- 🧠 Deep understanding of core concepts  
- 🧪 Hands-on exercises every day  
- 🧾 Fully commented code  
- 🚀 Real-world final project  

---

## 🛠 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/30daysofjavascript/30-Days-of-JavaScript.git
cd 30-Days-of-JavaScript
```

### 2️⃣ Explore Each Day
- Open the folder  
- Read `README.md`  
- Study `index.js`  

---

# 🚀 Complete Guide to Running JavaScript Everywhere

This guide covers **all major ways to run JavaScript**, from beginner-friendly methods to advanced environments.

---

## 🌐 1. How to run JavaScript?

### ✅ Method 1: Developer Console (Easiest)

#### 🔹 Steps:

1. Open Google Chrome
2. Open any website or a blank tab
3. Press:

   * `Ctrl + Shift + I` (Windows/Linux)
   * `Cmd + Option + I` (Mac)
4. Go to the **Console** tab
5. Type:

```js
console.log("Hello from Chrome Console!");
```

6. Press **Enter**

🎯 **Output:**
Instant result in the console.

---

### ✅ Method 2: HTML File

#### 🔹 Steps:

1. Open Notepad / VS Code
2. Create `index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>Run JS</title>
</head>
<body>

<h1>JavaScript Test</h1>

<script>
  alert("Hello from JavaScript!");
  console.log("Check console");
</script>

</body>
</html>
```

3. Save the file
4. Open it in Chrome

🎯 **Output:**

* Popup alert
* Console message

---

### ✅ Method 3: External JavaScript File

#### 🔹 Steps:

**index.html**

```html
<!DOCTYPE html>
<html>
<head>
  <title>External JS</title>
</head>
<body>

<script src="script.js"></script>

</body>
</html>
```

**script.js**

```js
console.log("Running from external JS file!");
```

Open `index.html` in Chrome.

---

### ✅ Method 4: Chrome Snippets (Advanced)

#### 🔹 Steps:

1. Open DevTools (`F12`)
2. Go to **Sources → Snippets**
3. Create a new snippet
4. Write:

```js
console.log("Snippet executed");
```

5. Press `Ctrl + Enter`

---

## 🖥️ 2. Run JavaScript Using Node.js

### ✅ Setup & Run

#### 🔹 Install:

Download and install Node.js

#### 🔹 Run Code:

```js
// app.js
console.log("Hello from Node.js");
```

```bash
node app.js
```

---

### ✅ Node REPL (Interactive Mode)

```bash
node
```

Then:

```js
console.log("Hello REPL");
```

---

## 📦 3. Run Using npm Scripts

#### 🔹 Steps:

```bash
npm init -y
```

Edit `package.json`:

```json
"scripts": {
  "start": "node app.js"
}
```

Run:

```bash
npm start
```

---

## ⚡ 4. Run JavaScript Using Deno

#### 🔹 Steps:

```js
// app.js
console.log("Hello from Deno");
```

```bash
deno run app.js
```

---

## 🌍 5. Run JavaScript Online (No Installation)

### ✅ Platforms:

* CodePen
* JSFiddle
* Replit
* StackBlitz

#### 🔹 Example:

```js
console.log("Hello online!");
```

Click **Run**.

---

## 📱 6. Run JavaScript on Mobile

### ✅ Methods:

* Chrome mobile console (limited)
* Apps:

  * Dcoder
  * JSAnywhere

---

## 🧩 7. Run JavaScript as ES Modules

```html
<script type="module">
  console.log("Using modules");
</script>
```

---

## 🛠️ 8. Run Using Build Tools (Example: Vite)

```bash
npm create vite@latest
cd project
npm install
npm run dev
```

---

## 🧵 9. Run JavaScript in Web Workers

```js
const worker = new Worker("worker.js");
```

---

## 🖧 10. Run JavaScript on Server (Express.js)

```js
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello Server");
});

app.listen(3000);
```

Run:

```bash
node server.js
```

---

## ☁️ 11. Run JavaScript in Cloud

### ✅ Examples:

* AWS Lambda
* Google Cloud Functions
* Azure Functions

---

## 🧪 12. Run JavaScript with Testing Tools

```bash
npx jest
```

---

## 🎮 13. Run JavaScript in Games

### ✅ Libraries:

* Phaser.js
* Babylon.js

---

## 🧾 14. Run JavaScript in Database (MongoDB)

```js
db.users.find()
```

---

## 🧠 15. Run Using JavaScript Engines

### ✅ Examples:

* V8 Engine
* SpiderMonkey

---

## 📊 Summary

| Method         | Difficulty | Use Case       |
| -------------- | ---------- | -------------- |
| Chrome Console | Easy       | Quick testing  |
| HTML File      | Easy       | Beginners      |
| Node.js        | Medium     | Backend        |
| Deno           | Medium     | Modern runtime |
| Online Tools   | Easy       | Practice       |
| Cloud          | Advanced   | Production     |

---

## 🎯 Final Notes

### 👶 Beginners should start with:

* Chrome Console
* HTML file

### 👨‍💻 Developers commonly use:

* Node.js
* Build tools

---

💡 *Tip:* Start simple, then move to advanced tools as you grow.


### 🧪 4. Online Editors

- https://jsfiddle.net  
- https://codepen.io  
- https://replit.com   

---

## 📋 Prerequisites

- 🧑‍💻 VS Code (recommended)  
- 🌐 Browser (Chrome, Firefox, Edge)  
- ⚙️ Node.js (optional)  
- ❤️ Consistency  

---

---

### 🔁 VS Code extension Live Server

- Install **Live Server**  
- Right-click `index.html` → Open with Live Server 

## 🎯 By the End You Will

✔ Understand JavaScript deeply  
✔ Write modern ES6+ code  
✔ Work with APIs  
✔ Build real-world projects  
✔ Think like a developer  

---

## ⭐ Support

If this helps you:

👉 Star ⭐ the repo  
👉 Share with others  
👉 Contribute  

---

## 👨‍💻 Author

Built with ❤️ for developers  

---
