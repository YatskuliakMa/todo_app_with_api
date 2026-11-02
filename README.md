# Todo App with API

A todo list application built with React and TypeScript that stores its data on a remote server. You can add, complete, rename and delete todos, filter them by status, and see friendly error messages when a request to the API fails.

[**Live demo**](https://YatskuliakMa.github.io/todo_app_with_api/) · [Source code](https://github.com/YatskuliakMa/todo_app_with_api)

## Features

- Load the list of todos from the server on start
- Add a new todo
- Toggle a todo as completed / active
- Delete a todo
- Filter todos: **All**, **Active**, **Completed**
- Show the number of active items left
- Clear all completed todos at once
- Show an error notification when a request fails (the notification hides automatically)

## Tech Stack

- [React 18](https://react.dev/)
- [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vitejs.dev/)
- [Bulma](https://bulma.io/) and SCSS for styling
- [classnames](https://github.com/JedWatson/classnames) and [react-transition-group](https://reactcommunity.org/react-transition-group/) for UI state and animations
- ESLint, Prettier and Stylelint for code quality

## Project Structure

```
src/
├── api/          # Functions for requests to the todos API
├── components/   # React components (Header, TodoList, TodoItem, Footer, ErrorNotification)
├── styles/       # SCSS files (todoapp, todo, filter)
├── types/        # TypeScript types (Todo, FilterStatus, ErrorMessage)
├── units/        # Helpers, including the fetch client
├── App.tsx
└── index.tsx
```

## Getting Started

### Prerequisites

- Node.js 20
- npm

### Installation

```bash
git clone https://github.com/YatskuliakMa/todo_app_with_api.git
cd todo_app_with_api
npm install
```

### Run locally

```bash
npm start
```

The app will be available at [http://localhost:5173](http://localhost:5173).

## Available Scripts

| Script             | Description                                  |
| ------------------ | -------------------------------------------- |
| `npm start`        | Start the development server                 |
| `npm run build`    | Build the app for production                 |
| `npm test`         | Run Cypress tests                            |
| `npm run lint`     | Format styles and code, then run all linters |
| `npm run lint-js`  | Lint TypeScript / JavaScript files           |
| `npm run lint-css` | Lint SCSS files                              |
| `npm run format`   | Format `.ts` and `.tsx` files with Prettier  |
| `npm run deploy`   | Build and deploy the app to GitHub Pages     |

## Deployment

The project is deployed to GitHub Pages with `gh-pages`.

1. In `package.json`, change the `homepage` value from `"."` to the repository name:

   ```json
   "homepage": "/todo_app_with_api"
   ```

2. Run:

   ```bash
   npm run deploy
   ```

## Notes

- The app uses the Mate Academy students API (`https://mate.academy/students-api`).
- The artificial delay in the fetch client is required by the tests, so do not change it.
- The project is based on the [React TypeScript Starter Pack](https://github.com/mate-academy/react_typescript-starter-pack).

## Author

[YatskuliakMa](https://github.com/YatskuliakMa)
