# ai.designmatix.co.uk

Marketing site for **Designmatix AI products** — the AI division of Designmatix Ltd.

## URLs

| Page | URL |
|---|---|
| Hub | https://ai.designmatix.co.uk |
| Text-to-CAD | https://ai.designmatix.co.uk/texttocad |
| Live app | https://app.designmatix.co.uk |
| Main site | https://designmatix.co.uk |

## Architecture

```
ai.designmatix.co.uk           → AI products hub (this repo, GitHub Pages)
ai.designmatix.co.uk/texttocad → Text-to-CAD landing
                              ↘
                                  Cross-link traffic to ↘
                              ↗
designmatix.co.uk              → WordPress (existing) — main marketing & products
app.designmatix.co.uk          → Hostinger VPS — live Designmatix Text-to-CAD app
```

## Repo structure

```
.
├── CNAME              ← required by GitHub Pages for custom domain
├── README.md
├── index.html         ← AI hub (root page)
└── texttocad/
    └── index.html     ← Text-to-CAD landing
```

## Deployment

GitHub Pages auto-deploys on every push to `main`. To update content:

```sh
# edit any HTML file
git add .
git commit -m "update copy"
git push origin main
```

Site rebuilds in 1–2 minutes.

## License

© 2026 Designmatix Ltd. All rights reserved.
