# AIScanner Privacy Policy — GitHub Pages site

Single-page HTML privacy policy ready to deploy on GitHub Pages.

## Deploy in 5 minutes

### Step 1 — Create a new GitHub repo

Recommended name: `aiscanner-privacy` (any name works).
Make it **public** (GitHub Pages needs public on free accounts).

### Step 2 — Push these 3 files

```bash
git init
git add index.html favicon.png README.md
git commit -m "Initial privacy policy"
git branch -M main
git remote add origin https://github.com/<YOUR_GH_USERNAME>/aiscanner-privacy.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to repo → **Settings** → **Pages** (left sidebar)
2. **Source** → "Deploy from a branch"
3. **Branch** → `main` / `/ (root)` → Save
4. Wait ~30 seconds, refresh

Your URL will be: `https://<YOUR_GH_USERNAME>.github.io/aiscanner-privacy/`

### Step 4 — Fill in the placeholders

Open `index.html` and search-replace:

| Placeholder | Replace with |
|---|---|
| `{{EFFECTIVE_DATE}}` | e.g. `2026-06-02` (the date you publish the app) |
| `{{DEVELOPER_NAME}}` | e.g. `Your Name` or your studio name |
| `{{SUPPORT_EMAIL}}` | e.g. `aiscanner.support@gmail.com` |

There are 3 placeholders total (effective date appears twice — replace both). Commit and push; GitHub Pages auto-rebuilds in ~30s.

### Step 5 — Paste the URL into Play Console

Play Console → App content → **Privacy policy** → paste:
`https://<YOUR_GH_USERNAME>.github.io/aiscanner-privacy/`

Done. ✅

---

## Optional: custom domain

If you own a domain (e.g. `aiscanner.app`):

1. Add a `CNAME` file to this repo containing just: `privacy.aiscanner.app`
2. In your DNS provider, add a CNAME record:
   - Name: `privacy`
   - Value: `<YOUR_GH_USERNAME>.github.io`
3. Wait 5–60 min for DNS propagation
4. Repo Settings → Pages → Custom domain → enter `privacy.aiscanner.app` → check "Enforce HTTPS"

Then use `https://privacy.aiscanner.app/` in Play Console.

---

## What's in this folder

| File | Purpose |
|---|---|
| `index.html` | The privacy policy page (single self-contained file — no external deps, no JS, mobile-responsive, dark-mode aware) |
| `favicon.png` | 192×192 AIScanner icon shown in browser tabs |
| `README.md` | This file |
