# Project CLAUDE.md

## Project Overview

- **Project**: BingMoeNone GitHub Profile
- **Description**: Personal GitHub profile with cyberpunk-themed README
- **Main Technologies**: TypeScript, Python, Go, Next.js, Node.js

## GitHub Profile README

Location: `README.md`

### Features
- 🐍 GitHub contribution snake animation
- ⌨️ Typing animation header
- 📊 GitHub stats and streak tracking
- 🎯 Skills radar chart
- 🚀 Featured projects showcase
- 📧 Contact email (2945707804@qq.com)

### Theme
- **Primary Color**: Cyan (#00FFFF)
- **Background**: Black (#000000)
- **Style**: Cyberpunk / Tech

## GitHub Actions Workflow

Location: `.github/workflows/snake.yml`

### Purpose
Generates dynamic SVG assets for the README:
- `output/snake.svg` - Contribution graph snake animation
- `output/grid.svg` - Cyberpunk grid background
- `output/profile-summary-card.svg` - Profile summary card

### Troubleshooting Actions

If Actions shows 404 or doesn't run:

1. **Enable Actions**: Settings → Actions → General → Workflow permissions → Select "Read and write permissions"
2. **Access Actions**: Go to `https://github.com/BingMoeNone/actions` directly
3. **Manual Trigger**: Click "Run workflow" button on the Actions page

### Update Cycle
- Auto-runs daily at midnight
- Auto-runs on push to main branch
- Can be triggered manually from Actions tab

## File Structure

```
BingMoeNone/
├── README.md                    # GitHub profile README
├── CLAUDE.md                   # This file
├── .github/
│   └── workflows/
│       └── snake.yml           # SVG generation workflow
└── output/                     # Generated assets (via Actions)
    ├── snake.svg
    ├── grid.svg
    └── profile-summary-card.svg
```

## Notes

- The snake animation uses Platane/snk service as fallback
- All external resources (badges, stats) require internet access
- Some markdown lint warnings (MD033) are expected for inline HTML used by badges
