# CineReflect 🎬

A personal movie journal web app for curating watchlists and documenting viewing reflections, built as an educational project to learn REST API integration with React & Node.js.

> ⚠️ **Disclaimer**: This is a non-commercial, private-use application. All movie metadata is sourced from [TMDB](https://www.themoviedb.org/) under their API Terms of Use. No video streaming, downloading, or public content sharing is supported.

## ✨ Features

-   **Custom Watchlists**: Create and manage personalized movie lists (e.g., "Weekend Drama", "Sci-Fi Classics")
-   **Viewing Reflections**: Write and store private notes for each watched film, including ratings, key takeaways, and emotional responses
-   **Movie Metadata**: Fetch titles, posters, cast, synopsis, and ratings via TMDB API v3
-   **Search & Filter**: Find movies by title, genre, or release year; filter watchlists by status (watched / plan-to-watch)
-   **Local Data Privacy**: User notes and watchlists are stored in a private database; TMDB data is read-only and never modified

## 🛠️ Tech Stack

| Layer       | Technology               | Purpose                          |
|-------------|----------------------------|----------------------------------|
| Frontend    | React + Vite               | UI rendering, state management   |
| Backend     | Node.js + Express          | API proxy, authentication        |
| Database    | SQLite                     | Private note/watchlist storage   |
| External API| TMDB API v3                | Movie metadata retrieval         |
| Styling     | Tailwind CSS               | Responsive, minimalist design    |

## 🚀 Getting Started

### Prerequisites
-   Node.js ≥18.x
-   A valid TMDB API Key (v3 auth) – [Apply here](https://www.themoviedb.org/settings/api)

### Installation
1.  Clone the repository:
    ```bash
    git clone https://github.com/forevercd/cinereflect.git
    cd cinereflect

    ```
2.  Install dependencies:
    ```bash
    npm install

    ```
3.  Configure environment variables:
    Create a `.env` file in the root directory:
    ```env
    TMDB_API_KEY=your_tmdb_api_key_here
    PORT=3000

    ```
4.  Start the development server:
    ```bash
    npm run dev

    ```
5.  Open `http://localhost:3000` in your browser.

## 🔒 Security Notes

-   Never commit `.env` to version control (already added to `.gitignore`)
-   TMDB API Key is proxied through the backend to avoid frontend exposure
-   No user authentication is implemented (single-user private app)

## 📜 License & Attribution

This project is licensed under the MIT License. Movie data is provided by [TMDB](https://www.themoviedb.org/). This product uses the TMDB API but is not endorsed or certified by TMDB.

## 🤝 Contributing

This is a personal educational project and not open for contributions. However, feel free to fork and adapt for your own learning purposes.
