# frontend-preparation-kit

# HTML

### **HTML 5 Features**

1. **Semantic Elements** - These are HTML tags that convey meaning about structure and content of web page.

   Ex: **`<header>`**, **`<nav>`**, **`<main>`**, **`<article>`**, **`<section>`**, **`<aside>`**, **`<footer>`**, **`<figure>`**, and **`<figcaption>`**.

   They help in leveraging SEO, accessibility and browser compatibility

2. **Audio and Video Support** - To embed audio and video into HTML document, `<audio>` `<video>` tags came handy having support of numerous attributes height, width etc.

3. **Canvas Support** - It allows to easily draw graphics using Javascript. `<canvas>` requires width and height

4. **Geolocation API** - It is used to access geographical position of user.

5. **Local Storage** - It is used to store data in user’s browsers and can access them with help of Javascript APIs

6. **Responsive Images** - HTML5 makes it easy to have responsive images by including `srcset` attribute to specify multiple version of image at different screen resolution.

7. **Web Workers - It a**llows scripts to run in background in separate thread to prevent scripts from blocking one another on main thread in turn improves performance of application.

8. **Drag & Drop API** - It allows to grab any element in DOM and drop it to another location.

9. **Form Enhancements** - HTML5 introduces new features to existing forms including new input types such as email, URL, placeholder, required fields features, validation etc.

10. **Web Sockets** - Establishes an open and persistent two-way communication between the browser and server to send and receive messages over a single connection triggered by events.

11. **Cross Document Messaging** - It enables real-time communication between different parts of websites opened in different frames, windows etc.

---


# JS

### Execution Context

**What is Execution Context ?**

![](/assets/execution-context.png)

**Deep Dive - Execution Context**

- Everything in JS happens inside the execution context. Imagine it as a sealed off container within which JS runs. It is an abstract concept that holds the information about environment within which the current code is being executed.
  ![](/assets/execution-context-2.jpg)
- In the container first component is **memory component** and 2nd one is **code component.**
- Memory component has all the variables and functions in key value pairs. It is also known as **Variable environment**.
- Code component is the place where code is executed one line at a time. It is also known as **Thread of Execution**.
- JS is a **synchronous**, **single-threaded** language.
  - Synchronous - One command at a time.
  - Single-threaded - In a specific synchronous order.
- Javascript is not possible without execution context.

![](/assets/execution-context-3.png)

Arrow functions don’t have **arguments** object and **this** keyword instead they can use arguments object and this keyword from their closest regular function parent.

In the above example imagining there are hundreds of execution contexts for hundreds of function. Now how will engine keep track of order in which functions are called ? This is where call stack comes into picture.

### Call Stack

- It is the place where execution contexts get stacked on top of each other, to keep track of where we are in execution.
  _or_
- Call Stack is a mechanism to keep track of its place in script that calls multiple function.

![](/assets/call-stack.png)

- Javascript manages code execution context creation and deletion with the the help of **Call Stack**.
- Call Stack maintains the **order of execution** of execution contexts. It is also known as
  1. Program Stack
  2. Control Stack
  3. Runtime stack
  4. Machine Stack
  5. Execution context stack.
