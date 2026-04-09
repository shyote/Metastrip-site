# Metastrip — Website

Landing page, privacy policy and support page for Metastrip on the App Store.

## Files

- `index.html` — Main landing page
- `privacy.html` — Privacy Policy (required by Apple)
- `support.html` — Support page (required by Apple)

## Deploy on GitHub Pages (10 minutes)

### Step 1 — Create a GitHub repo

1. Go to github.com → New repository
2. Name it `metastrip-site` (or anything you want)
3. Set it to **Public**
4. Click "Create repository"

### Step 2 — Upload the files

Option A (no git needed):
1. Click "uploading an existing file" on the repo page
2. Drag and drop all 3 HTML files
3. Click "Commit changes"

Option B (with git):
```bash
git init
git add .
git commit -m "Initial site"
git remote add origin https://github.com/YOURUSERNAME/metastrip-site.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under "Source" → select **Deploy from a branch**
3. Branch: **main** · Folder: **/ (root)**
4. Click **Save**

Your site will be live in ~2 minutes at:
`https://YOURUSERNAME.github.io/metastrip-site`

### Step 4 — Add URLs to App Store Connect

In App Store Connect → your app → App Information:
- **Support URL** → `https://YOURUSERNAME.github.io/metastrip-site/support.html`
- **Privacy Policy URL** → `https://YOURUSERNAME.github.io/metastrip-site/privacy.html`

## Optional — Custom domain (metastrip.app)

1. Buy a domain on Namecheap or Cloudflare (~$15/year)
2. In your repo → Settings → Pages → Custom domain → enter your domain
3. In your DNS settings, add a CNAME record:
   - Name: `www`
   - Value: `YOURUSERNAME.github.io`
4. Wait 10-30 minutes for DNS to propagate

## Update the email address

Replace `support@metastrip.app` in `privacy.html` and `support.html` with your real support email before going live.
