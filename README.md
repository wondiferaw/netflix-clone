# Netflix Clone

A responsive movie and TV discovery interface inspired by streaming platforms. Built with React and Vite, Netflix Clone uses The Movie Database (TMDB) API to display a featured title and curated rows of movies and shows.

> **Note:** Netflix Clone is a front-end demonstration project. It does not stream movies or provide user accounts.

## Features

- Dynamic hero banner featuring a TMDB title
- Browse rows for trending titles, popular TV, top-rated movies, and action movies
- Swiper-powered horizontal carousels
- Movie cards with poster artwork, genre labels, and hover details
- Responsive layout with navigation and profile menu interactions
- TMDB API integration for live movie and TV metadata

## Built With

- [React](https://react.dev/)
- [Vite](https://vite.dev/)
- [Axios](https://axios-http.com/)
- [Swiper](https://swiperjs.com/)
- [TMDB API](https://developer.themoviedb.org/docs)
- CSS Modules and regular CSS

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 20.19+ or 22.12+
- npm (included with Node.js)
- A TMDB API key

### Installation

1. Clone the repository and enter the project directory:

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   cd YOUR-REPOSITORY
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a local `.env` file in the project root. Copy `.env.example`, then add your TMDB API key:

   ```env
   VITE_TMDB_API_KEY=your_tmdb_api_key
   ```

   Get an API key from your [TMDB account settings](https://www.themoviedb.org/settings/api). Keep `.env` private; it is excluded from Git. Restart the development server after changing environment variables.

4. Start the local development server:

   ```bash
   npm run dev
   ```

5. Open the local URL printed in the terminal, typically `http://localhost:5173`.

## Available Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server |
| `npm run build` | Create a production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run Oxlint |

## Project Structure

```text
src/
├── assets/
│   └── image/              # Local image assets
├── components/
│   ├── Banner/             # Featured title hero
│   ├── DisplayRow/         # TMDB data fetching and movie rows
│   ├── Footer/
│   ├── Header/
│   ├── MovieCard/
│   └── SlideShow/          # Horizontal carousel
├── Data/                   # Local sample movie data
├── Utility/
│   ├── MovieInstance.js    # Axios client for TMDB
│   └── requestUrls.js      # TMDB request endpoints
├── App.jsx
├── index.css
└── main.jsx
```

## Environment Variables

| Variable | Required | Description |
| --- | --- | --- |
| `VITE_TMDB_API_KEY` | Yes | TMDB API key used by the client to request movie and TV data |

Vite exposes variables prefixed with `VITE_` to browser code. Use this project only with a TMDB key you are comfortable using in a client-side demo, and never commit your `.env` file.

## Attribution

This product uses the TMDB API but is not endorsed or certified by TMDB.

## Contributing

Contributions are welcome. For substantial changes, open an issue first to discuss what you would like to change. For a pull request:

1. Create a focused branch.
2. Install dependencies and make your changes.
3. Run `npm run lint` and `npm run build`.
4. Submit a pull request with a clear summary and any relevant screenshots.

## License

No license is currently specified. Unless a license is added to this repository, all rights are reserved by the copyright holder.
