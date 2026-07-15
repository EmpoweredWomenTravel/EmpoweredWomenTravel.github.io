# Empowered Women Travel

Website for [empoweredwomentravel.com](https://empoweredwomentravel.com), hosted on GitHub Pages. Originally built on Squarespace; the content and images were recovered from the [Internet Archive Wayback Machine](https://web.archive.org/web/2019/https://empoweredwomentravel.com/) (2019 snapshots) and rebuilt as plain HTML/CSS, then extended with new destinations.

## Structure

- `index.html` — home page (Cuba feature + Ghana/Tokyo promos + Coming Soon teaser)
- `ghana.html` — Ghana trip (Panafest / Emancipation Day, summer 2026); photos from Wikimedia Commons (CC BY-SA, credited in the page footer)
- `tokyo.html` — Tokyo, Japan trip (August 2026 festivals + tech conference option); photos from Unsplash (free license)
- `itinerary.html` — Cuba tour itinerary, pricing and inclusions (next departure: February 10–16, 2027)
- `destinations.html` — "Coming Soon" page: future destinations (Africa series + worldwide) with vote-by-email CTAs
- `information.html` — trip information
- `reservations.html` — tour packages (booking is via email; the original Squarespace checkout doesn't carry over)
- `gallery.html` — photos from past trips
- `about.html` — about / FAQ (including current Cuba travel rules) / contact
- `css/style.css` — shared stylesheet
- `images/` — site images; `images/og/` holds the 1200×630 social share cards used by the Open Graph tags
- `CNAME` — custom domain (do not delete; GitHub Pages reads it)
- `sitemap.xml`, `robots.txt` — search engine files; the sitemap is registered in Google Search Console
- `googlef6750ccbb09aab6a.html` — Google Search Console ownership verification (**do not delete** or the property loses verification)

## How it's deployed

Pushing to `main` publishes automatically via GitHub Pages (Settings → Pages → `main` branch, `/` root). The custom domain `empoweredwomentravel.com` is configured with Enforce HTTPS; DNS A records point at GitHub Pages (`185.199.108–111.153`) with a `www` CNAME to `empoweredwomentravel.github.io`. Google Search Console is verified for the property, with `sitemap.xml` submitted.

## Editing notes

- Every page duplicates the header/nav and footer — when adding a page or nav item, update all HTML files.
- Each page has its own `<title>`, meta description, canonical URL and Open Graph/Twitter tags in `<head>`; when adding a page, copy the block and update the values (og:image should be a 1200×630 card in `images/og/`), and add the page to `sitemap.xml`.
- Contact is via embedded [Web3Forms](https://web3forms.com/) forms delivering to `info@empoweredwomentravel.com` (About, Information, Reservations request form, Coming Soon vote form); there is intentionally no phone number on the site. The access key lives in each form's hidden `access_key` input; the Web3Forms dashboard account is under info@. Successful submissions redirect to `thanks.html` (noindex).
- Ghana and Tokyo pricing is "contact us" until dates/prices are finalized; Cuba pricing and dates live in `itinerary.html`, `reservations.html` and the `index.html` hero.
- Some Wikimedia Commons photos are CC BY-SA and require the photographer credits kept in the page footers (`ghana.html`, `destinations.html`).
