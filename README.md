# vue-crud-local-storage

A small Vue-based CRUD (Create, Read, Update, Delete) example application that stores data in the browser's localStorage. This project is intended as a lightweight starter / learning resource for building CRUD apps with Vue and persisting data locally without any backend.

## Features

- Create, read, update and delete items
- Data persisted in localStorage so it survives page reloads
- Simple, easy-to-understand structure suitable for beginners
- Single-file components (SFCs) and straightforward state management

## Demo

Open the app in your browser after running the dev server. The app provides a simple list interface where you can add items, edit them inline (or in a form), and delete items. All changes are saved to localStorage automatically.

## Screenshots

Add screenshots in the `docs/` folder or replace these placeholders with images hosted in this repo.

## Getting started

Prerequisites

- Node.js (v12+ recommended)
- npm or yarn

Install dependencies

```bash
npm install
# or
# yarn
```

Run the development server

Check package.json to see which dev script is available for this project. Common scripts:

```bash
npm run dev    # for Vite / modern setups
# or
npm run serve  # for Vue CLI setups
```

Then open http://localhost:3000 (Vite) or the URL printed by the CLI.

Build for production

```bash
npm run build
```

Lint / Format (if available)

```bash
npm run lint
```

## How it works

- The application keeps the list of items in a Vue component's reactive state.
- On any create/update/delete operation the state is written to localStorage using a small storage utility.
- On app startup the storage utility reads from localStorage and hydrates the app state.

Typical localStorage key: `your-app-key` (check `src` for the actual key used in this repo).

Files of interest

- `src/` — main source files
- `src/components/` — Vue components for list, item, form, etc.
- `src/services/storage.js` (or similar) — wrapper around localStorage reads/writes

## Customization

- Change the localStorage key inside the storage utility if you want the app to use a different namespace.
- Swap the localStorage persistence with an API call to a backend when you want to add server sync.

## Development tips

- Keep state mutations centralized (a small store or composable) so persistence is easy to manage.
- Validate inputs before saving to prevent corrupt data in localStorage.
- Consider namespacing your keys and using JSON versioning if you plan to change stored data shape.

## Contributing

Contributions are welcome. Open an issue or send a PR with a clear description of the change.

## License

MIT

## Acknowledgements

This project is a simple educational example — inspired by many small tutorials and starter kits for Vue CRUD apps using localStorage.
