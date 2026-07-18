# CARBONZY

CARBONZY is a lightweight carbon habit tracking demo for university students. It helps students log greener daily choices, earn coins, complete challenges, verify recycling actions, and redeem rewards in an eco marketplace.

Live app: https://phk006.github.io/CARBONZY/

## Documentation

- [Project Overview](docs/PROJECT_OVERVIEW.md)
- [User Guide](docs/USER_GUIDE.md)
- [Technical Notes](docs/TECHNICAL_NOTES.md)
- [Deployment Guide](docs/DEPLOYMENT.md)
- [Roadmap](docs/ROADMAP.md)
- [Contributing](CONTRIBUTING.md)
- [Security](SECURITY.md)

## Features

- Daily green score dashboard
- Habit tracking with coin rewards
- Step tracker with distance, calories, and CO2 saved estimates
- Plastic disposal camera flow with demo verification
- Weekly challenges and bonus rewards
- Eco marketplace with redeemable student products
- Profile view with badges and purchase history
- Mobile-first single-page experience

## Project Structure

```text
.
├── index.html
├── .github/workflows/pages.yml
├── .nojekyll
├── .gitignore
├── CONTRIBUTING.md
├── SECURITY.md
└── docs/
    ├── DEPLOYMENT.md
    ├── PROJECT_OVERVIEW.md
    ├── ROADMAP.md
    ├── TECHNICAL_NOTES.md
    └── USER_GUIDE.md
```

## Quick Start

Open `index.html` directly in a browser.

For a local server:

```bash
npx serve .
```

Then open the local URL shown in the terminal.

## Deployment

This project is deployed with GitHub Pages from the `gh-pages` branch.

Production URL:

```text
https://phk006.github.io/CARBONZY/
```

See [docs/DEPLOYMENT.md](docs/DEPLOYMENT.md) for publishing steps.

## Status

Current version: prototype/demo.

The app currently stores state in memory only. Refreshing the browser resets demo progress.
