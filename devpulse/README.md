# ⚡ DevPulse

> Real-time GitHub activity radar for any developer.

DevPulse lets you analyze any public GitHub profile and visualize their activity, languages, streaks, and peak coding hours — all in a clean terminal-inspired dashboard.

![DevPulse Screenshot](https://via.placeholder.com/900x500/080c10/00e5ff?text=DevPulse)

## Features

- **Dev Score** — A composite score calculated from stars, followers, repos, and commit activity
- **Contribution Heatmap** — 6 months of commit activity visualized
- **Language Breakdown** — Top languages across all public repositories
- **Commit Streak** — Current streak, best streak, and total active days
- **Peak Coding Hours** — Bar chart of when the developer commits most
- **Top Repositories** — Sorted by stars, click to open on GitHub
- **Live Activity Feed** — Recent pushes, PRs, stars, forks with relative timestamps

## Demo

Try it live → [devpulse.github.io](https://github.com) *(deploy via GitHub Pages)*

## Getting Started

No build step, no dependencies. Just open in a browser.

```bash
git clone https://github.com/yourusername/devpulse.git
cd devpulse
open index.html
```

Or serve locally:

```bash
npx serve .
```

## Deploy to GitHub Pages

1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your dashboard is live at `https://yourusername.github.io/devpulse`

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- [GitHub REST API v3](https://docs.github.com/en/rest) — no auth required for public data
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) + [Syne](https://fonts.google.com/specimen/Syne) via Google Fonts

## API Rate Limits

The GitHub API allows **60 requests/hour** for unauthenticated users. For higher limits, you can fork and add a personal access token.

## Project Structure

```
devpulse/
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── app.js
└── README.md
```

## License

MIT
