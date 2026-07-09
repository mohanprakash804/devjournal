# DevJournal — Developer Growth Tracker

A single-file HTML app for tracking your developer growth: daily coding journal, skills progress, GitHub activity, and goal streaks. No build step, no backend — just open `index.html`.

## Features

- **Journal** — log daily entries (git-commit style) with title, notes, tags, time spent, and mood.
- **Skills** — track proficiency (0–100) per skill, log progress over time, view bar & line charts.
- **GitHub** — pull in your real public GitHub activity (profile, recent events, 12-week activity heatmap) via the public GitHub API.
- **Goals** — set goals, check in daily, track streaks with a calendar-style grid.
- **Dashboard** — overview stats: entries, streak, skills tracked, days tracking.
- **Export / Import** — back up or move your data as a `.json` file.

## Usage

Just open `index.html` in a browser. No install, no dependencies to build.

> Note: this file uses Claude.ai's `window.storage` API for persistence when opened as a Claude artifact. If you host/open it outside Claude.ai, replace the `loadState`/`saveState` functions in the `<script>` with `localStorage`, or wire up your own backend — the rest of the app works the same either way.

## Tech

- Vanilla HTML/CSS/JS, no framework
- [Chart.js](https://www.chartjs.org/) for skill charts (loaded via CDN)
- [GitHub REST API](https://docs.github.com/en/rest) for activity data (unauthenticated, public data only)

## License

MIT
