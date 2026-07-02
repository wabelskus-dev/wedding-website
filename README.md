# Bri & Liam Wedding Website

One-page wedding website for Bri and Liam's intimate North Shore Kauai wedding weekend.

## How to Edit

- Main page content lives in `index.html`.
- Styling lives in `styles.css`.
- Images live in `assets/`.
- Cloudflare publishes the copied files in `public/`.

Search `index.html` for comments like:

- `HERO IMAGE`
- `WEDDING DATE / LOCATION`
- `CEREMONY DETAILS`
- `WELCOME ADDRESS`
- `SCHEDULE`
- `GALLERY IMAGES`
- `RECOMMENDATIONS`

Those comments mark the easiest places to update text, dates, addresses, and images.

## Images

Current generated placeholder images:

- `assets/kauai-hero.png`
- `assets/princeville-lanai.png`
- `assets/north-shore-details.png`
- `assets/hero-tropical-boho.png`

When replacing images, use optimized `.jpg`, `.png`, or `.webp` files and keep filenames simple. If you change a filename, update the matching `src="..."` path in `index.html`.

## Local Preview

Open `index.html` in a browser to preview the site locally.

## Publishing with GitHub Desktop

1. Open GitHub Desktop.
2. Review the changed files.
3. Add a summary, such as `Build Kauai wedding website`.
4. Click **Commit to main**.
5. Click **Push origin**.

## Cloudflare Deployment

This project includes `wrangler.jsonc`:

```json
{
  "name": "wedding-website",
  "compatibility_date": "2026-07-01",
  "assets": {
    "directory": "./public"
  }
}
```

Cloudflare deploys the static files from `public/`. After editing root files, make sure the matching files are copied into `public/` before committing.

## Do Not Include by Default

- RSVP form
- Registry section

Those can be added later if needed.
