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
console.log(data);
moreWork(); // will run after console.log
```

## Non blocking code example

```js
const fs = require("fs");
fs.readFile("/file.md", (err, data) => {
  if (err) throw err;
  console.log(data);
});
moreWork(); // will run before console.log
```
[Read more about this](https://nodejs.org/en/docs/guides/blocking-vs-non-blocking/) 
</details>
<details>
  <summary>5. Where Node.js is frequently used</summary>

  1. Real-time chats
  2. Internet of Things
  3. Complex SPAs (Single-Page Applications)
  4. Real-time collaboration tools
  5. Streaming applications
  6. Microservices architecture
</details>
<details>
  <summary>6.  What do you understand by the term I/O?</summary>
  The term I/O stands for input and output. It is used to access anything outside of your application. The I/O describes any program, operation, or device that transfers data to or from a medium or another medium. This medium can be a physical device, network, or files within a system.

  I/O is loaded into the machine memory to run the program once the application starts.
</details>