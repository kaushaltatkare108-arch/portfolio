# Kaushal Tatkare — Portfolio

A single-page portfolio: plain HTML and CSS with no build step. It is hosted free on Vercel.

## Files
- `index.html` — the whole site
- `resume.pdf` — opened by the "Download résumé" buttons
- `photo.jpg` — your headshot (already included; replace it with any 4:5 photo to change it)
- `DESIGN.md` — colours, fonts and spacing, so future edits stay consistent

## Put it online for free (Vercel + GitHub)
1. Go to https://github.com/new. Name the repo `portfolio`, make it **Public**, and click **Create repository**.
2. On the empty repo page, click **uploading an existing file**. Drag in every file from this folder and click **Commit changes**.
3. Go to https://vercel.com/signup and choose **Hobby** (free). Sign up with **Continue with GitHub**.
4. Click **Add New… → Project**. **Import** the `portfolio` repo, leave Framework Preset as **Other**, and click **Deploy**.
5. Your site is live at `portfolio-xxxx.vercel.app`. To get a cleaner address, go to **Project → Settings → Domains** and add something like `kaushal-tatkare.vercel.app`.
6. To update the site, edit a file on GitHub (pencil icon) and commit. Vercel redeploys automatically in under a minute.

### Backup option: GitHub Pages
In the repo, go to **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**. The site goes live at `https://kaushaltatkare108-arch.github.io/portfolio/`.

### Optional: your own domain
Buy something like `kaushaltatkare.com` or `.in` from a registrar (about ₹500–1,000 a year). Then add it in **Vercel → Settings → Domains** and follow the DNS records it shows. Vercel's HTTPS is free.

## Common edits
- **Hero numbers:** search `class="stat"` in `index.html`.
- **Projects:** each project is an `<article class="card">` block. Copy one to add a case study later.
- **Experience:** each role is an `<li class="job">` block.
