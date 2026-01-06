# vue-crud-local-storage

A minimal Vue CRUD (Create, Read, Update, Delete) application using browser `localStorage`.  
Designed for learning Vue basics with simple client-side persistence — no backend required.

---

## Features

- Create, Read, Update, Delete operations.
- Data persistence using `localStorage`.
- Simple and clean Vue Single File Components (SFC).
- Lightweight and beginner-friendly.

---

## Getting Started

### Prerequisites

- Node.js (v14+)
- npm or yarn

### Installation

```
npm install
```

#### Run the Application

```
npm run dev
# or
npm run serve
```
Open the URL shown in the terminal.

## Features

- Application state is stored in Vue reactive data.
- Data is loaded from localStorage on startup.
- Any create, update, or delete action automatically updates localStorage.
- Uses a single storage key:
  ```
  vue-crud-local-storage-items
  ```

## Project Structure
```
src/
 ├── App.vue
 ├── main.js
 ├── components/
 └── services/ | composables/
```
