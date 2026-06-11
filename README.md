# FlixStream — Netflix-Inspired Movie App

A full-featured Netflix-style movie browser built with React + Vite + Tailwind CSS, powered by the TMDB API.

## 🚀 Quick Start

### 1. Get a TMDB API Key (Free)
1. Go to [https://www.themoviedb.org/signup](https://www.themoviedb.org/signup)
2. Create a free account
3. Go to **Settings → API** and request an API key (choose "Developer")
4. Copy your **API Key (v3 auth)**

### 2. Set Up Environment
Create a `.env` file in the project root:

```bash
cp .env.example .env
```

Edit `.env` and replace with your actual key:
```
VITE_TMDB_API_KEY=your_actual_api_key_here
```

### 3. Install & Run

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) 🎉

## 🎯 Features

- **Home Page** — Netflix-style rows: Trending, Popular, Top Rated, Now Playing, Action, Comedy, Horror, Romance, Sci-Fi
- **Hero Banner** — Random trending movie with backdrop, overview, and action buttons
- **Movie Details** — Full page with backdrop, poster, cast, trailer (YouTube embed), similar movies
- **Search** — Real-time search with genre filters and load-more pagination
- **My List** — Save/remove favorites (persisted in localStorage)
- **Responsive** — Mobile-first design
- **Loading Skeletons** — Smooth shimmer placeholders while fetching
- **Scroll-to-top** — Automatic on route changes

## 📁 Structure

```
src/
  components/
    Navbar.jsx        # Fixed top nav with search
    HeroBanner.jsx    # Hero section with movie backdrop
    MovieCard.jsx     # Individual movie card with hover effects
    MovieRow.jsx      # Horizontally scrollable row
    SkeletonRow.jsx   # Loading skeleton components
  pages/
    Home.jsx          # Main page with all rows
    MovieDetail.jsx   # Full movie details page
    Search.jsx        # Search + genre filter page
    Favorites.jsx     # My List page
  services/
    api.js            # All TMDB API calls
  utils/
    favorites.js      # LocalStorage favorites helper
```

## 🛠️ Tech Stack

- **React 18** + **Vite** — Fast development
- **React Router v6** — Client-side routing
- **Tailwind CSS** — Utility-first styling
- **TMDB API** — Movie data

## 📦 Build for Production

```bash
npm run build
npm run preview
```
