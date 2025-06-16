# 🧩 Pokémon Fetch & Search App (React + PokeAPI)

This is a simple React application that fetches Pokémon data from the [PokeAPI](https://pokeapi.co/) and displays them as cards. It also includes a real-time search filter to search Pokémon by name.

---


---

## 🚀 Features

- Fetches data for 124 Pokémon from PokeAPI
- Displays detailed Pokémon cards (images, names, etc.)
- Real-time search functionality
- Loading and error handling
- Fully responsive UI (with `index.css`)

---

## 🛠️ Tech Stack

- React (Hooks: `useState`, `useEffect`)
- Fetch API
- CSS Modules (`index.css`)
- PokeAPI


# 📡 Fetch API in JavaScript

The **Fetch API** is a modern interface in JavaScript used to make HTTP requests to servers and handle responses. It is promise-based and provides a cleaner, more powerful alternative to the older `XMLHttpRequest`.

---

## 🔹 Basic Syntax

```javascript
fetch(url, options)
  .then(response => {
    // handle the response
  })
  .catch(error => {
    // handle the error
  });



fetch('https://api.example.com/data', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({ name: 'Ashish', age: 25 })
})
  .then(response => response.json())
  .then(data => console.log('Success:', data))
  .catch(error => console.error('Error:', error));
async function getData() {
  try {
    const response = await fetch('https://api.example.com/data');
    if (!response.ok) throw new Error('Fetch failed');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}

```
