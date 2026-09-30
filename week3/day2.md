# Day 2 — React Fundamentals

## 1. `useState`

`useState` is a React Hook used to store data that can change and update the UI.

```jsx
const [count, setCount] = useState(0);
```

* `count` → current value
* `setCount` → updates the value
* `0` → initial value

```text
setCount()
   ↓
State changes
   ↓
Component re-renders
   ↓
UI updates
```

---

## 2. `useEffect`

`useEffect` is used to perform **side effects** such as API calls, timers, and event listeners.

```jsx
useEffect(() => {
  console.log("Component loaded");
}, []);
```

`[]` means the effect runs after the initial render.

With dependencies:

```jsx
useEffect(() => {
  console.log("Count changed");
}, [count]);
```

The effect runs when `count` changes.

---

## 3. `useState` vs `useEffect`

```text
useState
→ Stores data that affects the UI

useEffect
→ Performs side effects outside normal rendering
```

---

## 4. React vs Vite

**React** → JavaScript library used to build UI.

**Vite** → Development and build tool used to create, run, and build the application.

```text
React → Builds the UI
Vite  → Runs and builds the project
```

A React + Vite project uses both together.

---

## 5. XML

XML stands for **Extensible Markup Language**.

It is used to represent structured data.

```xml
<user>
  <name>Sarath</name>
</user>
```

---

## 6. JSX

JSX stands for **JavaScript XML**.

It allows us to write HTML-like UI inside JavaScript.

```jsx
const name = "Sarath";

return <h1>Hello {name}</h1>;
```

### XML vs JSX

```text
XML → Structured data

JSX → JavaScript syntax used to describe UI
```

---

## 7. DOM

DOM stands for **Document Object Model**.

It represents the actual webpage in the browser.

JavaScript can directly modify the DOM.

```text
JavaScript
    ↓
Real DOM
    ↓
Browser UI
```

---

## 8. Virtual DOM

The Virtual DOM is React's **in-memory representation of the UI**.

When state changes:

```text
State changes
     ↓
React renders
     ↓
Compare old and new UI
     ↓
Update required parts of Real DOM
```

### DOM vs Virtual DOM

```text
DOM
→ Actual webpage structure

Virtual DOM
→ React's representation of the UI
```

---

# Quick Revision

```text
useState  → Manage state
useEffect → Handle side effects

React → UI library
Vite  → Development/build tool

XML → Structured data
JSX → JavaScript + XML-like syntax

DOM         → Actual browser DOM
Virtual DOM → React's UI representation
```
