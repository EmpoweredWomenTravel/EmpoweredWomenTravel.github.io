# Empowered Women Travel

Static recreation of [empoweredwomentravel.com](https://empoweredwomentravel.com), originally built on Squarespace. Content and images were recovered from the [Internet Archive Wayback Machine](https://web.archive.org/web/2019/https://empoweredwomentravel.com/) (2019 snapshots) and rebuilt as plain HTML/CSS for GitHub Pages hosting.

## Structure

- `index.html` — home page
- `ghana.html` — Ghana trips (Panafest/Emancipation Day summer 2026 + Chale Wote festival season); Ghana photos are from Wikimedia Commons (CC BY-SA, credited in the page footer)
- `tokyo.html` — Tokyo, Japan trips (August 2026 festival trip + tech/security conference trip); Tokyo photos are from Unsplash (free license)
- `itinerary.html` — Cuba tour itinerary, pricing and inclusions
- `destinations.html` — "Coming Soon" page: future destinations (Africa series + worldwide) with vote-by-email CTAs; photos from Unsplash and Wikimedia Commons (CC, credited in the page footer)
- `information.html` — trip information
- `reservations.html` — tour packages (booking is via email/phone; the original Squarespace checkout doesn't carry over)
- `gallery.html` — photos from past trips
- `about.html` — about / FAQ / contact
- `css/style.css` — shared stylesheet
- `images/` — images recovered from the Wayback Machine
- `CNAME` — custom domain for GitHub Pages

## Things to update

- **Trip dates and prices are from 2019** (Havana trips at $697/$797 and the $1,497 tour). Update `index.html`, `itinerary.html` and `reservations.html` before promoting new trips.
- The original contact forms were Squarespace forms; they've been replaced with `mailto:` links. A service like [Formspree](https://formspree.io/) can add a real form without a backend.

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
3. Point DNS for `empoweredwomentravel.com` at GitHub Pages (A records `185.199.108.153`, `.109.`, `.110.`, `.111.153`, plus a `www` CNAME to `<username>.github.io`).
4. In Settings → Pages, set the custom domain and enable **Enforce HTTPS**.
