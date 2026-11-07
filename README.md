# kalmzeetje.nl

Single-page portfolio for Kalm Zeetje, hosted on GitHub Pages.

## Files
- `index.html` — the whole site
- `favicon.svg` — tab icon
- `CNAME` — tells GitHub Pages to serve on kalmzeetje.nl
- `images/` — project hero images (4:3, ~1600×1200, .jpg or .webp)

## Add a project
Copy one `<a class="project">` block in `index.html`, then change the link, name and tagline (`slogan`).
For an image, replace the text inside `<div class="img">` with `<img src="images/name.jpg" alt="">`.

## Go live (one-time)
1. Push this folder to a GitHub repo (e.g. `kalmzeetje`).
2. Repo → Settings → Pages → Source: "Deploy from a branch" → `main` / root.
3. Custom domain: `kalmzeetje.nl` (already set via `CNAME`).
4. Hostnet → DNS for kalmzeetje.nl:
   - Remove existing A/AAAA records for `@` and `www` (Hostnet's parking page).
   - A `@` → 185.199.108.153
   - A `@` → 185.199.109.153
   - A `@` → 185.199.110.153
   - A `@` → 185.199.111.153
   - CNAME `www` → `<github-username>.github.io.`
5. When GitHub shows the DNS check passed, tick "Enforce HTTPS".

Every push to `main` after that goes live within a minute or two.
