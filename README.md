# Travel Blog Starter (GitHub Pages + Jekyll)

Minimum-boilerplate blog: GitHub builds and hosts it for you, no local install needed.

## 1. Create the repo
On GitHub, create a **new public repo** named exactly:

```
<your-username>.github.io
```

(Replace `<your-username>` with your actual GitHub username. This exact name is
what triggers GitHub's free auto-hosting.)

## 2. Push these files
```bash
cd travel-blog-starter
git init
git add .
git commit -m "Initial blog setup"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

## 3. Turn on Pages
Repo → **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` / `(root)` → Save.

Your site goes live at `https://<your-username>.github.io` within about a minute.

## 4. Write new posts
Add a file to `_posts/` named `YYYY-MM-DD-your-title.md`:

```markdown
---
layout: post
title: "Title Here"
date: 2026-08-01
categories: [country-name]
---

Your post content in markdown.
```

Commit + push, and it appears on the site automatically — no build command required.

## Customizing
- Swap `theme: minima` in `_config.yml` for any other GitHub Pages–supported theme
  (e.g. `jekyll-theme-cayman`, `jekyll-theme-minimal`) — just change the name and push.
- Add images to an `/assets/` folder and reference them with normal markdown `![]()`.
- Want a fancier travel-specific theme later? Browse https://jekyllthemes.io and swap
  it in — the `_posts` structure stays the same.
