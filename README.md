# Sam Sinha · Portfolio

A single-page, dependency-free portfolio site with a dark theme and neon teal, indigo, and violet accents. Everything is in one `index.html` plus a photo, so it runs anywhere with no build step. Your photo is embedded directly in the page.

## Files
- `index.html` — the whole site (HTML, CSS, JS, and your photo, all inline)
- `sam.jpg` — backup copy of the photo (the site does not depend on it)
- `README.md` — this file

## Put it on GitHub Pages (free, about 3 minutes)

1. Create a new repository. Name it `samvibhaw.github.io` if you want it at `https://samvibhaw.github.io`, or any name (for example `portfolio`) for a project URL.
2. Upload the files to the root of the repo. On GitHub: **Add file → Upload files**, drag them in, then **Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then **Save**.
5. Wait about a minute. Your site goes live at:
   - `https://samvibhaw.github.io` (if you used that repo name), or
   - `https://<your-username>.github.io/portfolio` (for a project repo).

## Editing
- All copy and numbers live in `index.html`. Search for the text you want to change.
- Your photo is embedded directly inside `index.html` (as a data URI), so it always shows and never breaks. To swap it later, the simplest path is to ask for a fresh build with a new photo, or replace the three `src="data:image/jpeg;base64,..."` values.
- The project artwork is hand-built SVG inside each `.card-art` block. You can later drop in real screenshots of dashboards or decks by replacing the `<svg>` with an `<img src="...">`.

## What is interactive
- Floating gradient glows in the hero and education sections
- A rotating headline that cycles through your six target roles
- Filter buttons on Selected Work that show projects by role
- A live testimonial bulletin under About that auto-rotates with dots and arrows
- A centered Professional Timeline with experiences alternating on both sides
- Count-up animation on the impact numbers
- A scroll progress bar and active section highlighting in the nav
- Hover lift and colored glow on every card

## Adding your real recommendations
The testimonial bulletin currently has your one quote plus two placeholders. To add your LinkedIn recommendations, open `index.html`, find the `testimonials` array near the bottom, and edit each entry's `q` (the quote) and `a` (name and title). Or send the quotes over and I will drop them in.

All of it respects reduced-motion settings and works down to mobile.

## Custom domain (optional)
In **Settings → Pages → Custom domain**, add your domain and follow the DNS steps GitHub shows. A `CNAME` file gets created for you.

## Notes
- No frameworks, no `npm`, no tracking. Fonts load from Google Fonts; everything else is self-contained.
- Works down to mobile, keyboard-focusable, and respects reduced-motion settings.
