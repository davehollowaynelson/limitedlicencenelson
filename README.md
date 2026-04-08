# Limited Licence Nelson static rebuild

Clean single-page static rebuild for free hosting on GitHub Pages.

## What's changed

- Rebuilt as a static site, no WordPress, PHP, or database
- Removed the contact form entirely
- Replaced form CTA with direct phone and email contact
- Kept the core public content, FAQ, and testimonials

## Local preview

```bash
cd /Users/jh/.openclaw/workspace/sites/limitedlicencenelson
python3 -m http.server 8000
```

Then open <http://localhost:8000>

## GitHub Pages deployment

1. Create a new GitHub repo, for example `limitedlicencenelson`
2. Push these files to the repo root
3. In GitHub, enable **Settings → Pages**
4. Deploy from the `main` branch, `/ (root)`
5. Point the domain at GitHub Pages

## DNS for apex domain

If using GitHub Pages on the apex domain, use GitHub's A records:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

For `www`, use a CNAME to:

- `<your-github-username>.github.io`

## Files

- `index.html`
- `styles.css`
- `assets/hero.jpg`
- `assets/favicon.png`
- `CNAME`
- `.nojekyll`
