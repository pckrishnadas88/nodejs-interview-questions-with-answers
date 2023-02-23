# Node.js interview questions with answers

These are various interview questions with answers collected from various resources across the web.

<details>
  <summary>1. What is Node.js</summary>
  Node.js® is an open-source, cross-platform JavaScript runtime environment. As an asynchronous event-driven JavaScript runtime, Node.js is designed to build scalable network applications. Node.js is perfect for data-intensive applications as it uses an asynchronous, event-driven model. You can use  I/O intensive web applications like video streaming sites. You can also use it for developing: Real-time web applications, Network applications, General-purpose applications, and Distributed systems.
</details>
<details>
  <summary>2. How does Node.js works(Event loop Explained)</summary>
  This is best explained in this video.

  [Morning Keynote- Everything You Need to Know About Node.js Event Loop - Bert Belder, IBM](https://www.youtube.com/watch?v=PNa9OMajw9w).
</details>
<details>
  <summary>2. How does Node.js works(Event loop Explained)</summary>
  This is best explained in this video.

  [Morning Keynote- Everything You Need to Know About Node.js Event Loop - Bert Belder, IBM](https://www.youtube.com/watch?v=PNa9OMajw9w).
</details>
<details>
  <summary>3. Explain callback in Node.js</summary>
 A callback is a function called when the task finishes, and a callback function allows other code to run in the meantime. Using the Callback concept, Node.js can process many requests without waiting for any function to return the result, making Node.js highly scalable.
</details>
<details>
  <summary>4. Explain blocking code vs non blocking code with an example</summary>
Blocking methods execute synchronously and non-blocking methods execute asynchronously.
Using the File System module as an example, this is a synchronous file read:

## Blocking code example

```js
const fs = require("fs");
const data = fs.readFileSync("/file.md"); // blocks here until file is read
```

## Non blocking code example

```js
const fs = require("fs");
fs.readFile("/file.md", (err, data) => {
  if (err) throw err;
});
```
</details>