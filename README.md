# zakirzb.github.io

Personal website for **Zakir ZB** — a self-taught cybersecurity learner. Plain, static, no trackers, no JavaScript.

## Files
- `index.html` — the whole site (single page)
- `style.css` — terminal-inspired dark theme
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Before you publish — edit these
In `index.html`, replace the placeholder contact details:
- `mailto:you@example.com` → your real email
- `https://github.com/zakirzb` → your GitHub
- `https://www.linkedin.com/in/zakirzb` → your LinkedIn

Update the footer year and any text in the About / Skills / Work sections to match you.

## Deploy to GitHub Pages

### Option A — user site (recommended, gives you `zakirzb.github.io`)
1. Create a **public** repo named exactly `zakirzb.github.io`.
2. Push these files to the `main` branch:
   ```sh
   cd zakirzb-site
   git init
   git add .
   git commit -m "Initial cybersecurity site"
   git branch -M main
   git remote add origin https://github.com/zakirzb/zakirzb.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main` / `/ (root)`.
4. Visit **https://zakirzb.github.io** (allow a minute or two for the first build).

### Option B — project site
Push to any repo, then enable Pages the same way. URL becomes
`https://zakirzb.github.io/<repo-name>/`.

## Security notes
- No JavaScript and no third-party requests — minimal attack surface.
- A Content-Security-Policy `<meta>` tag restricts the page to its own origin.
- External links use `rel="noopener noreferrer"`.
- GitHub Pages serves everything over HTTPS automatically.
