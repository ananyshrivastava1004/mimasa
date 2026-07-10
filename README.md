# The Databrief — Jekyll starter theme

A magazine-style, data-journalism blog theme (inspired by Visual Capitalist),
built to run **100% free** on GitHub Pages.

## What's inside

- `_config.yml` — site settings and the category color legend
- `_layouts/` — homepage and post page templates
- `_includes/chart-thumb.html` — reusable inline SVG bar-chart thumbnail
- `_posts/` — 5 sample posts across 5 categories (Markets, Technology, Energy, Geopolitics, Environment)
- `assets/css/style.css` — all styling, no external CSS framework

## Preview it locally (optional but recommended)

If you have Ruby installed:

```
gem install bundler jekyll
cd databrief
bundle init
bundle add jekyll jekyll-feed
bundle exec jekyll serve
```

Then open http://localhost:4000

If you don't want to install anything locally, skip straight to deploying —
GitHub will build it for you automatically.

## Deploy free on GitHub Pages

1. Create a free GitHub account at github.com if you don't have one.
2. Create a new **public** repository, e.g. named `my-blog`.
3. Upload every file in this folder into that repository (drag-and-drop
   works fine in GitHub's web UI, or use `git push` if you're comfortable
   with git).
4. In the repo, go to **Settings → Pages**.
5. Under "Build and deployment", set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`. Save.
6. Wait 1–2 minutes. Your site will be live at:
   `https://YOUR-USERNAME.github.io/my-blog/`

## Writing new posts

Add a new file to `_posts/` named `YYYY-MM-DD-your-title.md` with this
front matter at the top:

```
---
title: "Your Headline Here"
category: Markets
accent: "#D98E2B"
chart_bars: "30,50,40,70,90"
---

Your article content in Markdown goes here.
```

`category` must be one of: Markets, Technology, Energy, Geopolitics,
Environment — each has a matching color already wired up in
`_config.yml` and `style.css`. Add more categories by adding a color
to both files.

## Custom domain (still free hosting, just a paid domain ~$10/yr)

If you later want `www.yourblog.com` instead of the github.io address:
1. Buy a domain from any registrar (Namecheap, Google Domains, etc).
2. Add a `CNAME` file to the repo root containing just your domain.
3. Point your domain's DNS to GitHub Pages per GitHub's docs.

Everything else — hosting, bandwidth, SSL certificate — stays free.
