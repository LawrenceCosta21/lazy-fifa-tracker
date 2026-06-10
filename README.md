# ⚽ FIFA World Cup 2026 — Live Fixture Tracker

A mobile-friendly, zero-dependency static website showing FIFA World Cup 2026 group stage fixtures with live score simulation, dynamic local time display, and dark mode support.

## Features

- 🔴 Live score updates (auto-refresh every 5 seconds)
- 🕐 All times shown in the visitor's local timezone
- 📱 Fully responsive — works on mobile, tablet, and desktop
- 🌙 Automatic dark mode
- 🔍 Filter by: All / Live / Today / Upcoming / Group A–H
- ⚡ Zero dependencies — pure HTML, CSS, JavaScript

## Deploy in 60 seconds

### Option 1 — GitHub Pages (free)

```bash
# 1. Create a new repo on GitHub, then:
git init
git add .
git commit -m "Initial commit: FIFA 2026 fixture tracker"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/fifa2026.git
git push -u origin main

# 2. Go to your repo → Settings → Pages
#    Source: Deploy from branch → main / root
#    Your site will be live at: https://YOUR_USERNAME.github.io/fifa2026
```

### Option 2 — Netlify (drag & drop)

1. Go to [netlify.com](https://netlify.com) → drag the `fifa2026-site` folder onto the deploy area
2. Done — live in seconds with a random URL you can customize

### Option 3 — Vercel

```bash
npm i -g vercel
vercel
# Follow the prompts — deployed in ~30 seconds
```

### Option 4 — Cloudflare Pages

```bash
# Connect your GitHub repo at dash.cloudflare.com → Pages
# Build command: (leave empty)
# Output directory: /
```

## File structure

```
fifa2026-site/
├── index.html     ← Everything is here (self-contained)
└── README.md
```

## Customization

All match data lives in the `MATCHES` array inside `index.html`. Each match object has:

```js
{
  id: 1,
  group: 'Group A',
  home: 'Mexico',  hf: '🇲🇽',   // home team + flag emoji
  away: 'Poland',  af: '🇵🇱',   // away team + flag emoji
  venue: 'Estadio Azteca, Mexico City',
  date: '2026-06-12T14:00:00',   // ISO date string
  sH: 2, sA: 1,                  // scores (null = not played yet)
  status: 'ft'                   // 'upcoming' | 'live' | 'ft'
}
```

## License

MIT — free to use and modify.
