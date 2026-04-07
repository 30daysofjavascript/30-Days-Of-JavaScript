# 🚀 Day 03 — Strings & String Methods

### 📚 30 Days of JavaScript: Beginner to Advanced

---

## 🔤 1. Creating Strings

```js id="1f2k9a"
let single   = 'Hello';          
let double   = "World";          
let backtick = `Template Literal`; // ✅ Most powerful
```

---

### 🔐 Escaping Special Characters

```js id="2x9qpl"
let quote = "He said \"Hello!\"";
let path  = 'C:\\Users\\Alice\\file';
let newLine = "Line 1\nLine 2";
let tab     = "Column1\tColumn2";

console.log(newLine);
```

---

## ✨ 2. Template Literals (Modern Way)

```js id="7mda81"
let name = "Alice";
let age  = 25;

let message = `My name is ${name} and I am ${age} years old.`;
console.log(message);
```

---

### 🧠 Expressions Inside `${}`

```js id="9h2vxs"
console.log(`2 + 2 = ${2 + 2}`);
console.log(`Uppercase: ${name.toUpperCase()}`);
```

---

### 📜 Multi-line Strings

```js id="c1as8o"
let poem = `
Roses are red,
Violets are blue,
JavaScript is awesome,
And so are you!
`;

console.log(poem);
```

---

## 🔎 3. String Properties & Indexing

```js id="8sk0jf"
let str = "JavaScript";

console.log(str.length);        // 10
console.log(str[0]);            // "J"
console.log(str[4]);            // "S"
console.log(str[str.length-1]); // "t"
```

---

### ⚠️ Strings are Immutable

```js id="s3n9dq"
str[0] = "j"; 
console.log(str); // Still "JavaScript"
```

---

## 🛠️ 4. String Methods

```js id="u8plxv"
let text = "  Hello, World!  ";
```

---

### 🔠 Case Methods

```js id="g0k2px"
text.toUpperCase();
text.toLowerCase();
```

---

### ✂️ Trim Whitespace

```js id="z5kq1p"
text.trim();
text.trimStart();
text.trimEnd();
```

---

### 🔍 Searching

```js id="l2q9sn"
let sentence = "The quick brown fox jumps over the lazy dog";

sentence.indexOf("fox");
sentence.lastIndexOf("the");
sentence.includes("fox");

sentence.startsWith("The");
sentence.endsWith("dog");
```

---

### ✂️ Extracting Parts

```js id="w7s4ad"
let lang = "JavaScript";

lang.slice(0, 4);
lang.slice(4);
lang.slice(-6);

lang.substring(0, 4);

lang.charAt(0);
```

---

### 🔄 Replacing

```js id="3d0gqs"
let phrase = "I love cats. Cats are great!";

phrase.replace("Cats", "Dogs");
phrase.replaceAll("cats", "dogs");

phrase.replace(/cats/gi, "dogs");
```

---

### 🔗 Splitting & Joining

```js id="m8v6ye"
let csv = "Alice,Bob,Charlie,Diana";

let names = csv.split(",");
let chars = "hello".split("");

names.join(" | ");
```

---

### 🔁 Repeat & Padding

```js id="x0as92"
"ha".repeat(3);

"5".padStart(3, "0");
"5".padEnd(3, "0");
"42".padStart(5, "0");
```

---

### 🧩 Convert to Array

```js id="k3p9sd"
let word = "hello";
let arr = [...word];
```

---

## ⚖️ 5. String Comparisons

```js id="n7q2lp"
console.log("apple" < "banana");
console.log("Z" < "a");
```

---

### 🌍 Locale Compare

```js id="p2x7fa"
"a".localeCompare("b");
"b".localeCompare("a");
"a".localeCompare("a");
```

---

## 💡 6. Practical Examples

---

### 🧪 Capitalize First Letter

```js id="q1m8st"
function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1).toLowerCase();
}
```

---

### 🔢 Count Character Occurrence

```js id="a8f3ds"
function countChar(str, char) {
  return str.split(char).length - 1;
}
```

---

### 🔁 Palindrome Check

```js id="z9c4lp"
function isPalindrome(str) {
  const cleaned = str.toLowerCase().replace(/[^a-z0-9]/g, "");
  return cleaned === cleaned.split("").reverse().join("");
}
```

---

### ✂️ Truncate String

```js id="b2x9vr"
function truncate(str, maxLength) {
  if (str.length <= maxLength) return str;
  return str.slice(0, maxLength) + "...";
}
```

---

## 📝 Exercises

---

### 🧪 Exercise 1

Extract first & last name from:

```js id="k9x1df"
"John Doe"
```

---

### 🧪 Exercise 2

Check if string contains only digits
👉 Hint: `/^\d+$/`

---

### 🧪 Exercise 3

Convert:

```js id="v3s7qa"
"hello_world_foo" → "helloWorldFoo"
```

---

### 🧪 Exercise 4

Count vowels (`a, e, i, o, u`) in a string

---

### 🧪 Exercise 5

Reverse a string **without using `.reverse()`**

---

## ⭐ Support

If you found this helpful:

👉 Give this repo a ⭐
👉 Share with others 🚀
👉 Keep building 💻

---

## 🎉 Day 03 Complete!

Now you know:

* String creation & template literals
* Powerful string methods
* Searching & manipulation
* Real-world string problems

👉 Next: **Arrays & Array Methods** 🔥
