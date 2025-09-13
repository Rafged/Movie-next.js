Movie Search — Next.js 15 + /app + TypeScript with TMDB search

Features:
- Top tabs (Search / Rated) with search field positioned like the screenshot
- Search uses TMDB API via a server route (you must provide TMDB_API_KEY)
- Results show poster, title, date, genres, overview, TMDB vote average, and star rating (1-10)
- Ratings saved in localStorage and visible in Rated tab
- Pagination (client-side) 6 items per page

Setup:
1. Copy this project locally.
2. Create `.env.local` in the project root with:
   TMDB_API_KEY=your_tmdb_api_key_here
3. npm install
4. npm run dev
5. Open http://localhost:3000

Notes:
- The server route `/api/search?q=...` proxies requests to TMDB and returns a simplified JSON.
- If poster images are missing, a placeholder is shown.
