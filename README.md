# Daily Motivation Dashboard 

A  React application that displays motivational quotes, allows users to like quotes, and saves liked quotes in local storage.

This project was built as a frontend-only class assignment to practice React state management, `useEffect`, conditional rendering, and list rendering with `map()`.

## Features
 
- Fetches a random quote on load and when the user clicks **New Quote**
- Shows a loading state while fetching
- Disables the fetch button while a request is in progress
- Like/Unlike quote toggle
- Displays total liked quotes count
- Shows a list of liked quotes
- Search/filter for liked quotes
- Show/Hide liked quotes list toggle
- Persists liked quotes using `localStorage`
- Fallback offline quotes if the API is unavailable

## Tech Stack

- React
- Vite
- CSS (custom styling)

## API Used

- `https://dummyjson.com/quotes/random`

## Project Structure

```text
.
├── index.html
├── package.json
├── vite.config.js
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   └── styles.css
└── README.md
```

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm

### Installation

```bash
npm install
```

### Run Locally

```bash
npm run dev
```

Vite will print a local development URL (usually `http://localhost:5173`).

## Available Scripts

- `npm run dev` - Starts the development server
- `npm run build` - Creates a production build in `dist/`
- `npm run preview` - Previews the production build locally

## Deployment (GitHub Pages)

This is a frontend-only project and can be hosted on GitHub Pages.

### Notes

- Do not commit `node_modules/`
- Do not commit `dist/` (it is generated during build/deploy)
- Make sure the `base` path in `vite.config.js` matches your repository name if deploying to `https://username.github.io/repo-name/`

Example:

```js
export default defineConfig({
  plugins: [react()],
  base: "/your-repo-name/",
});
```

## Assignment Requirements Covered

- `useState` for UI and data state
- `useEffect` for API calls
- Loading and empty states
- `map()` list rendering with proper keys
- Filter/search interaction
- Toggle interaction (like/unlike and show/hide liked list)

## License

This project is for educational use.
