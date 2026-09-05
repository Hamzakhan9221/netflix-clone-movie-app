# Movie App 🎬

A Netflix-style movie browsing app built with React and the TMDB API. Search for movies, view popular titles, and save your favorites.

## 🔗 Live Demo
[reactmovieproject2026.netlify.app](https://reactmovieproject2026.netlify.app)

## ✨ Features
- Browse popular movies
- Search movies by title
- Add/remove favorites
- Responsive, dark-themed UI

## 🛠️ Built With
- React
- Vite
- TMDB API (via Fetch API)
- CSS

## 🔌 API Integration

This project uses the **TMDB (The Movie Database) API** to fetch movie data via the native **Fetch API**.

### Files involved
- `src/Services/api.js` — handles all API calls

### Functions
- `getPopularMovies()` — fetches the list of popular movies
- `searchMovies(query)` — searches movies by title using a query string

### How it works

    const API_KEY = import.meta.env.VITE_TMDB_API_KEY;
    const BASE_URL = "https://api.themoviedb.org/3";

- The API key is stored securely in a `.env` file and accessed via Vite's `import.meta.env`
- The `.env` file is excluded from version control via `.gitignore`

## 📦 Environment Variables

Create a `.env` file in the root directory and add:

    VITE_TMDB_API_KEY=your_tmdb_api_key_here

> Get your free API key from [themoviedb.org](https://www.themoviedb.org/settings/api)

## 🗂️ Project Structure

    src/
    ├── pages/
    │   ├── Home.jsx
    │   ├── Favorites.jsx
    ├── Services/
    │   └── api.js        → TMDB API integration (fetch calls)
    ├── App.jsx
    ├── main.jsx
