# Bramley Moore Dogs website

A single-page static site. No build step, no dependencies: just `index.html`.

## Before you publish

1. Open `CNAME` and replace `www.yourdomain.co.uk` with your real domain (one line, no `https://`).
2. In `index.html`, search for these placeholders and update them:
   - `hello@bramleymooredogs.co.uk` (email)
   - `@bramleymooredogs` Instagram and TikTok links
   - Menu items and prices
   - The "Find us this week" locations and times

## Put it on GitHub Pages

1. Create a new public repository on GitHub (e.g. `bramley-moore-dogs`).
2. Upload `index.html` and `CNAME` to the root of the repository (Add file > Upload files, then Commit).
3. Go to **Settings > Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick `main` and `/ (root)`, then Save.
4. Under **Custom domain**, enter your domain and Save.

## Point your domain at GitHub

In your domain registrar's DNS settings:

- For `www.yourdomain.co.uk`: add a **CNAME** record with host `www` pointing to `YOUR-GITHUB-USERNAME.github.io`
- For the bare domain `yourdomain.co.uk`: add four **A** records with host `@` pointing to:
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153

DNS can take up to 24 hours to update. Once GitHub shows the domain as verified, tick **Enforce HTTPS** in Settings > Pages.

(These IP addresses are GitHub's published Pages addresses. Double-check them in GitHub's docs: "Managing a custom domain for your GitHub Pages site".)
