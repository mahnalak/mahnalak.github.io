# Lakshita Mahna — Portfolio

Personal portfolio site. Single-file, zero dependencies, zero build step — just `index.html`.

**Live at:** `https://mahnalak.github.io/` (after deploying, see below)

## Deploy to GitHub Pages (free hosting)

1. Create a new repo on GitHub named **`mahnalak.github.io`** (using your exact username gives you the cleanest URL). Any other repo name also works.
2. Upload `index.html` and this `README.md` to the repo (drag-and-drop on github.com, or:)
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/mahnalak/mahnalak.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / root → Save**.
4. Wait ~1 minute. Your site is live at `https://mahnalak.github.io/` (or `https://mahnalak.github.io/<repo-name>/` if you used a different repo name).

## Customizing

- **Contact form:** currently opens the visitor's email app with a prefilled message to `lakshitamahna04@gmail.com`. For a form that sends without opening an email client, create a free form at [formspree.io](https://formspree.io), then replace the `sendBtn` click handler with a `fetch` POST to your Formspree endpoint.
- **Logos:** pulled live from Clearbit's logo API. If any company logo fails to load, a styled monogram letter shows automatically.
- **Colors/fonts:** everything is in the `:root` CSS variables at the top of `index.html`.
- **Content:** all text lives directly in the HTML — search for the section you want to edit.
