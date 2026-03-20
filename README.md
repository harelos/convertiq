# ConvertIQ Website

Marketing website for the ConvertIQ Chrome Extension. Hosted on GitHub Pages.

## Pages
- `index.html` — Landing page
- `privacy.html` — Privacy Policy (Chrome Store compliant)
- `terms.html` — Terms of Service
- `support.html` — Support center & FAQ
- `style.css` — Shared design system

## Deploy to GitHub Pages

### Step 1 — Create a GitHub repo
1. Go to github.com → New repository
2. Name it `convertiq-site` (or anything you like)
3. Set visibility to **Public**
4. Click Create repository

### Step 2 — Push these files
```bash
cd convertiq-site
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/convertiq-site.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repo → Settings → Pages
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Click Save

Your site will be live at:
`https://YOUR_USERNAME.github.io/convertiq-site/`

### Step 4 — Update all URLs
Search and replace `yourusername` with your actual GitHub username across all files.

### Step 5 — Update the Chrome Store listing
In your Chrome Web Store developer dashboard, set:
- **Homepage URL**: `https://YOUR_USERNAME.github.io/convertiq-site/`
- **Privacy Policy URL**: `https://YOUR_USERNAME.github.io/convertiq-site/privacy.html`
- **Support URL**: `https://YOUR_USERNAME.github.io/convertiq-site/support.html`

## Custom domain (optional)
1. Buy a domain (e.g. convertiq.app)
2. In your repo, create a file called `CNAME` with just your domain: `convertiq.app`
3. In your DNS provider, add a CNAME record pointing to `YOUR_USERNAME.github.io`
4. In GitHub Pages settings, enter your custom domain and enable HTTPS

## What makes this Chrome Store compliant
- Privacy Policy explains exactly what data is/isn't collected
- Support page with working email contact
- Terms of Service covering acceptable use
- All pages accessible via direct URL (no JS-only routing)
- No tracking or analytics on the site itself
