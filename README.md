# IT2234P Web Services and Server Technologies

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Code Quality](https://img.shields.io/badge/Code%20Quality-A-brightgreen?style=for-the-badge)]())

> 📚 A comprehensive collection of daily practical lessons for Web Services and Server Technologies course.

## 📋 Course Overview

This repository serves as a practical guide through various web services and server technologies. Each lesson is organized in dedicated folders containing both source code and visual outputs.

## 🗓️ Latest Session: Asynchronous Programming in JavaScript (April 3, 2025)

### 🎯 Learning Objectives

- Master asynchronous programming concepts in JavaScript
- Implement Promise-based asynchronous operations
- Utilize async/await for cleaner asynchronous code
- Understand event-driven and non-blocking I/O programming
- Handle file operations asynchronously
- Manage error handling in asynchronous code
- Compare different asynchronous patterns

### 💻 Code Examples & Implementations

#### 1. Async/Await Pattern (`asynwait.js`)
```javascript
//Async/await
const fs = require('fs').promises;

const readFile = async () => {
    try {
        const data = await fs.readFile('input.txt', 'utf8');
        console.log(data); 
    }
    catch (error) {
        console.error(error); 
    }
}; 
readFile();
```
[View Output](asynwait.png)

#### 2. Promise-Based Implementation (`promiseapp.js`)
```javascript
const fs = require('fs').promises;

const readFile = async (filePath) => {
    return fs.readFile(filePath, 'utf8');
};

readFile('input.txt')
    .then((data) => {
        console.log(data);
    })
    .catch((error) => {
        console.error(error);
    });
```
[View Output](promiseapp.png)

#### 3. Event-Driven Programming (`eventdrivenandnonIOblockingprogramme.js`)
```javascript
const fs = require('fs');

fs.readFile('input.txt', function(err, data) {
   if (err) return console.error(err);
   console.log(data.toString());
});

console.log("File read successfully!");
```
[View Output](eventdrivenandnonIOblockingprogramme.png)

### 📊 Implementation Summary

| Category | File | Description | Output |
|----------|------|-------------|--------|
| Async/Await | `asynwait.js` | Modern async/await pattern for file operations | [View](asynwait.png) |
| Promises | `promiseapp.js` | Promise-based asynchronous file handling | [View](promiseapp.png) |
| Event-Driven | `eventdrivenandnonIOblockingprogramme.js` | Non-blocking I/O operations | [View](eventdrivenandnonIOblockingprogramme.png) |

### 🔍 Technical Notes

- All implementations use Node.js file system module
- Demonstrates different asynchronous programming patterns
- Each example includes error handling
- Visual outputs captured for reference
- Consistent code formatting and naming conventions

---

<div align="center">

📖 **Learning Path** | 🛠️ **Practical Examples** | 📊 **Visual Outputs**

</div>