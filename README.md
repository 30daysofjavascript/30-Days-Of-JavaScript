# 🚀 30 Days of JavaScript — Beginner to Advanced

> 🎯 **Master JavaScript step-by-step in 30 days**  
> From absolute beginner → advanced concepts → real-world project

---

## 📚 Course Structure

| Day | Topic | Level |
|-----|-------|-------|
| [Day 01](./Day-01-Variables-DataTypes/) | Variables & Data Types | 🟢 Beginner |
| [Day 02](./Day-02-Operators/) | Operators | 🟢 Beginner |
| [Day 03](./Day-03-Strings/) | Strings & String Methods | 🟢 Beginner |
| [Day 04](./Day-04-Arrays/) | Arrays | 🟢 Beginner |
| [Day 05](./Day-05-Objects/) | Objects | 🟢 Beginner |
| [Day 06](./Day-06-Functions/) | Functions | 🟢 Beginner |
| [Day 07](./Day-07-Scope-Hoisting/) | Scope & Hoisting | 🟡 Intermediate |
| [Day 08](./Day-08-Arrow-Functions/) | Arrow Functions | 🟡 Intermediate |
| [Day 09](./Day-09-Array-Methods/) | Array Methods | 🟡 Intermediate |
| [Day 10](./Day-10-Destructuring/) | Destructuring | 🟡 Intermediate |
| [Day 11](./Day-11-Spread-Rest/) | Spread & Rest Operators | 🟡 Intermediate |
| [Day 12](./Day-12-DOM-Basics/) | DOM Manipulation Basics | 🟡 Intermediate |
| [Day 13](./Day-13-DOM-Events/) | DOM Events | 🟡 Intermediate |
| [Day 14](./Day-14-Forms-Validation/) | Forms & Validation | 🟡 Intermediate |
| [Day 15](./Day-15-ES6-Classes/) | ES6 Classes | 🟡 Intermediate |
| [Day 16](./Day-16-Prototypes-Inheritance/) | Prototypes & Inheritance | 🟠 Advanced |
| [Day 17](./Day-17-Promises/) | Promises | 🟠 Advanced |
| [Day 18](./Day-18-AsyncAwait/) | Async / Await | 🟠 Advanced |
| [Day 19](./Day-19-Fetch-API/) | Fetch API & HTTP | 🟠 Advanced |
| [Day 20](./Day-20-Error-Handling/) | Error Handling | 🟠 Advanced |
| [Day 21](./Day-21-Modules/) | ES Modules | 🟠 Advanced |
| [Day 22](./Day-22-LocalStorage/) | LocalStorage & SessionStorage | 🟠 Advanced |
| [Day 23](./Day-23-Regex/) | Regular Expressions | 🟠 Advanced |
| [Day 24](./Day-24-Closures/) | Closures | 🔴 Expert |
| [Day 25](./Day-25-Higher-Order-Functions/) | Higher-Order Functions | 🔴 Expert |
| [Day 26](./Day-26-Iterators-Generators/) | Iterators & Generators | 🔴 Expert |
| [Day 27](./Day-27-Map-Set/) | Map & Set | 🔴 Expert |
| [Day 28](./Day-28-WeakMap-WeakSet/) | WeakMap & WeakSet | 🔴 Expert |
| [Day 29](./Day-29-Design-Patterns/) | Design Patterns | 🔴 Expert |
| [Day 30](./Day-30-Final-Project/) | Final Project — Full App | 🔴 Expert |

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

Built with ❤️ for the developer community.  
Feel free to star ⭐ this repo if it helps you!

---
