# Decision Makers Club — website

The site for **[decisionmakersclub.com](https://decisionmakersclub.com)** — an invite-only community of founders and CXOs making AI-driven decisions.

Built with [Hugo](https://gohugo.io/) (extended). Minimal, black-and-white. By [Robobrainstorm](https://robobrainstorm.com).

## Develop

```bash
hugo server
```

Open http://localhost:1313.

## Structure

- `hugo.toml` — all site copy lives here (headline, meetup, principles, social links, Luma/apply URLs).
- `layouts/` — templates: `index.html` (home), `_default/sell.html` (Sell to Enterprise), `_default/baseof.html` (shell).
- `assets/css/main.css` — styles (fingerprinted at build).
- `content/sell-to-enterprise.md` — the Sell to Enterprise page stub.

## Deploy

Pushing to `main` triggers `.github/workflows/hugo.yml`, which builds with Hugo and deploys to GitHub Pages. The custom domain is set via `static/CNAME`.
