# DailyGames

Open `index.html` in a browser to submit and view scores. The page uses Tailwind CSS and the Supabase JavaScript client from CDNs, so it requires an internet connection.

The date defaults to your device's local date. After a successful submission, your player name is saved in browser local storage for your next visit.

The Supabase `scores` table must allow the public client to read and insert scores through its grants and row-level security policies. The publishable key is visible in the page; use appropriate policies to restrict access and do not put a secret or service-role key in the browser.

The `scores` table stores the chosen date in the `game_date` date column. The `created_at` timestamp records when the score was submitted.
