# Day 1 — React Fundamentals

## 1. Installing React with Vite

**Vite** is a tool used to create and run React projects.

Create a React project:

```bash
npm create vite@latest
```

React + JavaScript:

```bash
npm create vite@latest my-app -- --template react
```

Then:

```bash
cd my-app
npm install
npm run dev
```

Vite usually runs the application at:

```text
http://localhost:5173
```

---

## 2. Library vs Framework

### Library

A library gives us tools that we can use when we need them.

**React is a library for building user interfaces.**

```text
We control the application
        ↓
We use the library
```

### Framework

A framework provides a complete structure for building an application.

Examples:

* Next.js
* Angular

Simple difference:

```text
Library → We call it

Framework → It controls more of the application flow
```

---

## 3. Public Folder

The `public` folder stores files that can be accessed directly.

For example:

```text
public/
 ├── image.png
 ├── favicon.svg
 └── icons.svg
```

We can use an image like:

```jsx
<img src="/image.png" />
```

---

## 4. `main.jsx`

`main.jsx` is where the React application starts.

It connects React to the HTML element:

```html
<div id="root"></div>
```

The basic flow is:

```text
main.jsx
   ↓
App.jsx
   ↓
Components
   ↓
UI
```

---

## 5. JSX

**JSX** allows us to write HTML-like code inside JavaScript.

Example:

```jsx
function App() {
  return <h1>Hello React</h1>;
}
```

We can also use JavaScript inside JSX using `{}`:

```jsx
const name = "Sarath";

return <h1>Hello {name}</h1>;
```

JSX makes writing UI easier.

---

## 6. Components

A component is a **reusable piece of UI**.

Example:

```jsx
function Welcome() {
  return <h1>Welcome</h1>;
}
```

We can use it inside another component:

```jsx
function App() {
  return <Welcome />;
}
```

Large applications are divided into smaller components.

---

## 7. Types of Components

There are two common types:

### Functional Component

A JavaScript function that returns JSX.

```jsx
function Welcome() {
  return <h1>Hello</h1>;
}
```

This is the common approach in modern React.

### Class Component

An older way of creating React components.

```jsx
class Welcome extends React.Component {
  render() {
    return <h1>Hello</h1>;
  }
}
```

Modern React mainly uses **functional components and Hooks**.

---

## 8. Single Page Application (SPA)

SPA means **Single Page Application**.

The browser loads the application and React changes the UI without completely reloading the page for every interaction.

Example:

```text
Open website
     ↓
React application loads
     ↓
Click button
     ↓
UI changes
     ↓
No full page reload
```

---

## 9. `node_modules`

`node_modules` contains the packages required by our project.

When we run:

```bash
npm install
```

npm downloads the dependencies into `node_modules`.

Example:

```text
node_modules/
 ├── react/
 ├── react-dom/
 ├── vite/
 └── ...
```

We normally **do not push `node_modules` to GitHub**.

Instead, we push:

```text
package.json
package-lock.json
```

Another developer can run:

```bash
npm install
```

to install the required packages.

---

## 10. README.md

`README.md` is the **documentation file** of a project.

It can contain:

* Project description
* Installation steps
* How to run the project
* Technologies used
* Features

GitHub automatically displays the README on the repository page.

---

## 11. DOM vs Virtual DOM

### DOM

DOM stands for **Document Object Model**.

It represents the actual webpage inside the browser.

JavaScript can directly change the DOM.

```text
JavaScript
    ↓
Real DOM
    ↓
Browser UI
```

### Virtual DOM

The Virtual DOM is a representation of the UI that React keeps in memory.

When something changes:

```text
State/Props change
       ↓
React creates new UI representation
       ↓
React compares old and new
       ↓
Finds what changed
       ↓
Updates the Real DOM
```

### Simple difference

```text
DOM
→ Actual webpage structure

Virtual DOM
→ React's representation of the UI
```

---

## 12. JSON

JSON stands for **JavaScript Object Notation**.

It is a format commonly used to exchange data between frontend and backend.

Example:

```json
{
  "name": "Sarath",
  "age": 21
}
```

For example:

```text
React
  ↓
API Request
  ↓
Backend
  ↓
JSON Response
  ↓
React
```

---

## 13. Props

**Props** means properties.

Props are used to send data from a **parent component to a child component**.

Example:

```jsx
function User({ name }) {
  return <h2>Hello {name}</h2>;
}

function App() {
  return <User name="Sarath" />;
}
```

Here:

```text
App
 ↓
name="Sarath"
 ↓
User
```

Props allow components to receive data from their parent.

---

## 14. React / Vite Port

When we run a React project created with Vite:

```bash
npm run dev
```

Vite normally starts the development server at:

```text
http://localhost:5173
```

Remember:

```text
React → UI library

Vite → Development/build tool
```

So `5173` is the **Vite development server port**.

---

## 15. React Lifecycle

A component generally goes through three important stages:

```text
Mounting
   ↓
Updating
   ↓
Unmounting
```

### Mounting

The component is added to the UI.

### Updating

The component updates when its state or props change.

### Unmounting

The component is removed from the UI.

In functional components, `useEffect()` is commonly used for effects related to these stages.

---

## 16. Virtual DOM

The Virtual DOM is React's **in-memory representation of the UI**.

When state or props change:

```text
State changes
     ↓
React renders again
     ↓
Compare old and new UI
     ↓
Find changes
     ↓
Update Real DOM
```

The goal is to update only the parts of the actual DOM that need to change.

---

# Day 1 Summary

Today I learned:

* How to create a React project using Vite
* Difference between a library and framework
* Purpose of the `public` folder
* Purpose of `main.jsx`
* JSX
* Components
* Functional and class components
* Single Page Applications
* `node_modules`
* `README.md`
* DOM vs Virtual DOM
* JSON
* Props
* Vite development server
* React lifecycle

### Overall React Flow

```text
Vite
 ↓
Creates and runs React project
 ↓
main.jsx
 ↓
App.jsx
 ↓
Components
 ↓
JSX
 ↓
Props + State
 ↓
React
 ↓
Virtual DOM
 ↓
Real DOM
 ↓
Browser UI
```
