# How to host this website on GitHub Pages

This repo is a static HTML/CSS/JS site for **Habit Care**. You can publish it for free with GitHub Pages.

## What you need

- A GitHub account
- This project pushed to a GitHub repository (this repo is fine)
- About 2 minutes

## Option A — Publish from the `main` branch (recommended)

1. Push this project to GitHub (if it is not already there).
2. Open the repository on GitHub in your browser.
3. Go to **Settings** → **Pages** (under “Code and automation”).
4. Under **Build and deployment**:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/` (root)
5. Click **Save**.
6. Wait 1–2 minutes, then refresh the Pages settings. GitHub will show a URL like:

   `https://YOUR-USERNAME.github.io/habit-care-pages/`

7. Open that URL. You should see the Habit Care home page.

### Useful page URLs

| Page | Path |
|------|------|
| Home | `/` or `/index.html` |
| Privacy Policy | `/privacy-policy.html` |
| Delete Account | `/delete-account.html` |

Example:

`https://YOUR-USERNAME.github.io/habit-care-pages/privacy-policy.html`

## Option B — Custom domain (optional)

1. In **Settings** → **Pages**, under **Custom domain**, enter your domain (e.g. `habitcare.app`).
2. Follow GitHub’s DNS instructions (usually a `CNAME` or `A` records at your domain registrar).
3. After DNS propagates, enable **Enforce HTTPS** if available.

## Updating the site later

1. Edit the HTML/CSS/JS files locally.
2. Commit and push to `main`:

```bash
git add .
git commit -m "Update site content"
git push origin main
```

3. GitHub Pages will republish automatically in a minute or two.

## Local preview (before publishing)

Open `index.html` in a browser, or serve the folder:

```bash
# Python
python -m http.server 8080

# Node (if you have npx)
npx serve .
```

Then visit `http://localhost:8080`.

## App Store / Play Console links

Use these live URLs in store listings:

- Privacy Policy: `https://YOUR-USERNAME.github.io/habit-care-pages/privacy-policy.html`
- Account deletion: `https://YOUR-USERNAME.github.io/habit-care-pages/delete-account.html`

Replace `YOUR-USERNAME` and `habit-care-pages` with your real GitHub username and repo name.
