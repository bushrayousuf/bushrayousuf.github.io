# Bushra Yousuf — Portfolio Site

A single-file interactive portfolio (`index.html`): filterable project cards, expandable case-study details, light/dark mode, mobile-responsive. No build step, no dependencies.

## View it locally

Open `index.html` in any browser, or run:

```bash
cd portfolio-site
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Editing

- **Project cards:** search for `<!-- Card` in `index.html`. Copy a whole `<article class="card">…</article>` block to add a new one. Set `data-tags` from: `influencer`, `social-first`, `community`, `insights` (space-separated).
- **Hero / About / Contact:** plain HTML near the top and bottom of the file.
- **Theme:** colors live in the `:root` and `html[data-theme="dark"]` blocks at the top of the `<style>`.

## Open to-dos

- [ ] **Visuals:** drop screenshots / reels / campaign images into `assets/` and reference them in the cards (e.g. `<img src="assets/campaign-1.jpg" alt="…">`). The Canva site's phone-mockup creative would port well here.
- [ ] **Client clearance:** confirm the client work shown here is OK to display publicly.
- [ ] **Resume PDF:** export your resume as PDF into `assets/`, then uncomment the Resume button in the hero.
- [ ] **Custom domain:** buy a domain (e.g. `bushrayousuf.com`), add a file named `CNAME` containing just the domain, and follow GitHub's DNS instructions under Settings → Pages.
- [x] **Contact info:** email, phone, and LinkedIn are filled in from the Canva site.

## Deploying to GitHub Pages

1. Create a public repo named `YOUR-USERNAME.github.io` on github.com.
2. Upload this folder's contents (`index.html`, `README.md`, `.gitignore`, `assets/`).
3. Go to **Settings → Pages** → Source: **Deploy from a branch** → branch `main`, folder `/ (root)` → Save.
4. Live in ~1 minute at `https://YOUR-USERNAME.github.io`.
