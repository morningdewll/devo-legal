# quiettime-legal

Static legal site for the QuietTime mobile app. Hosted on GitHub Pages.

## Files

- `index.html` — landing
- `privacy.html` — Privacy Policy (Last updated: May 10, 2026)
- `terms.html` — Terms of Service (Effective: May 10, 2026)
- `style.css` — shared styling

## Deploy (one-time, ~2 minutes)

1. Create a new public repo on GitHub. Suggested name: `quiettime-legal`.
   - Go to https://github.com/new
   - Owner: `morningdewll`
   - Repository name: `quiettime-legal`
   - Visibility: **Public** (required for free GitHub Pages)
   - Do NOT initialize with README, .gitignore, or license — this folder already has the README.

2. From this folder (`C:\Users\4Bros\Desktop\Quiettime\legal-site`):
   ```bash
   git init
   git add .
   git commit -m "init: privacy policy + terms of service"
   git branch -M main
   git remote add origin https://github.com/morningdewll/quiettime-legal.git
   git push -u origin main
   ```

3. Enable Pages:
   - Repo → Settings → Pages
   - Source: **Deploy from a branch**
   - Branch: `main` / Folder: `/ (root)`
   - Save.
   - Wait ~30s for first deploy.

4. Live URLs (replace `morningdewll` with the actual GitHub username if different):
   - Landing: `https://morningdewll.github.io/quiettime-legal/`
   - Privacy: `https://morningdewll.github.io/quiettime-legal/privacy.html`
   - Terms: `https://morningdewll.github.io/quiettime-legal/terms.html`

5. Use these URLs in:
   - Play Console → Store presence → Main store listing → Privacy Policy
   - App Store Connect → App Information → Privacy Policy URL
   - Anywhere else the listings ask for terms or privacy

## Updating

Edit any HTML file in this folder, then:
```bash
git add . && git commit -m "update: <reason>" && git push
```
GitHub Pages re-deploys within a minute. Keep `Last updated` dates in sync between `privacy.html` and `terms.html`.

## Source of truth

The canonical Markdown drafts live in the QuietTime app repo:
- `docs/store/privacy-policy.md`
- `docs/legal/terms-of-service.md`

When changing legal language, edit the Markdown first, then mirror into the HTML here. The HTML is what users actually see.
