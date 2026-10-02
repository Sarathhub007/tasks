# Day 4 — HashMap, Arrays & APIs

Today I learned about **HashMap, fetching data from arrays, APIs, and how to fetch API data in React**.

## 1. What is a HashMap?

A HashMap stores data as **key → value** pairs.

```js
const users = {
  1: "Sarath",
  2: "Rahul"
};

console.log(users[1]); // Sarath
```

It is useful when we want to quickly find data using a key.

---

## 2. Fetching Data from an Array

We can use methods like:

```js
map()
filter()
find()
```

Example:

```js
const users = [
  { id: 1, name: "Sarath" },
  { id: 2, name: "Rahul" }
];

const user = users.find(user => user.id === 2);

console.log(user);
```

Output:

```text
{ id: 2, name: "Rahul" }
```

---

## 3. What is an API?

**API (Application Programming Interface)** allows two applications to communicate with each other.

For example:

```text
React Application
       ↓
      API
       ↓
   Backend / Server
       ↓
      Data
       ↓
React Application
```

An API can provide data such as users, products, movies, weather, etc.

---

## 4. Fetching Data from an API

JavaScript provides `fetch()` to make an API request.

```js
fetch("https://example.com/users")
  .then(response => response.json())
  .then(data => console.log(data));
```

With `async/await`:

```js
async function getUsers() {
  const response = await fetch("https://example.com/users");
  const data = await response.json();

  console.log(data);
}
```

---

## 5. Fetching API Data in React

Usually we fetch data inside `useEffect()` and store it in `useState()`.

```jsx
const [users, setUsers] = useState([]);

useEffect(() => {
  fetch("https://example.com/users")
    .then(response => response.json())
    .then(data => setUsers(data));
}, []);
```

Then we can display the data:

```jsx
{users.map(user => (
  <p key={user.id}>{user.name}</p>
))}
```

## Simple Flow

```text
API Request
    ↓
Server sends Response
    ↓
Convert Response to JSON
    ↓
Store data in State
    ↓
map() over the data
    ↓
Display in UI
```

### Key Takeaway

```text
HashMap → key-value data
Array   → collection of values
API     → communication between applications
fetch() → gets data from an API
JSON    → common format for API data
map()   → displays/processes array data
```