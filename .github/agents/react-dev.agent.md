---
name: react-dev
description: Develop and test a new react project with the latest tools and best practices.
argument-hint: The inputs this agent expects, e.g., "a task to implement" or "a question to answer".
# tools: ['vscode', 'execute', 'read', 'agent', 'edit', 'search', 'web', 'todo'] # specify the tools this agent can use. If not set, all enabled tools are allowed.
---
Develop a new React project that displays a list of items fetched from an API


## Technologies
- [React](https://react.dev/) (for building the user interface)
- [Axios](https://github.com/axios/axios) (for API calls)
- CSS with [Tailwind](https://tailwindcss.com/docs/installation/using-vite) (for styling)
- UI testing with [Playwright with network mocking](https://playwright.dev/docs/mocking) (for testing API calls and UI interactions)

## Project structure with feature-based organization
```src/
├── components/
│   ├── ItemList/
│   │   ├── ItemList.jsx
│   │   ├── ItemList.css
│   └── Item/
│       ├── Item.jsx
│       ├── Item.css
├── services/
│   └── api.js
├── App.jsx
├── index.js
└── index.css
```

## Commands to run
- `npm install` to install dependencies
- `npm start` to run the development server
- `npx playwright test` to run playwright tests


## Best practices to follow
- MUST use functional components and React hooks
- MUST keep components small and focused on a single responsibility
- MUST use PropTypes for type checking
- MUST handle errors gracefully, especially for API calls
- MUST write tests for components and API calls with mocking to ensure reliability and maintainability
- MUST use Tailwind for consistent styling and responsive design
