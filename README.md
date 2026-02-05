GitHub Pages static clone of kingdomtech.uk

What this is
- A minimal static clone of the provided Kingdom Tech UK homepage.
- The clone keeps visual content and external links but removes server-side WordPress/FluentForm processing.

Files
- `index.html` — static page (simplified) built from the supplied HTML.
- `images/` — place any image files you want to host locally here.
- `.nojekyll` — (optional) prevents GitHub Pages from ignoring files starting with `_`.

Notes & limitations
- Dynamic features from the original (FluentForm contact form, admin-ajax endpoints, WordPress REST calls) are not functional in this static copy. To restore form submissions you can:
  - Replace the form with a Formspree or Netlify Forms endpoint, or
  - Reconnect the form to a server-side handler.
- Many CSS/JS assets in the original reference `kingdomtech.uk` CDN/cache paths. This copy leaves those visual assets referenced where possible but uses a simplified inline stylesheet to preserve layout.

How to publish on GitHub Pages
1. Initialize repo (if not already):

```bash
cd /path/to/kingdom-tech
git init
git add .
git commit -m "Add static site for GitHub Pages"
# create remote and push as needed
```

2. Push and enable GitHub Pages
- Option A: Push `main`/`master` and set GitHub Pages to serve from the repository root or `main` branch.
- Option B: Move files into `docs/` and set GitHub Pages to serve from `/docs`.

3. If using custom domain (kingdomtech.uk), add `CNAME` with the domain root, and configure DNS accordingly.

Next steps I can help with
- Upload your images into `images/` and I will rewrite `index.html` to reference them locally.
- Enable a working contact form (Formspree/Netlify) and wire the form to that service.
- Add a simple CSS/JS asset pipeline and copy over assets from the live site for a closer clone.

Tell me which of the next steps you want and whether you will upload images now.