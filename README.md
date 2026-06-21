# Vistas

A self-hosted, Bloomberg-style analytics terminal for NSE indices, stocks and India macro.

## Live link

**Terminal → https://kartiksngh.github.io/vistas/terminal/**

The bare URL (https://kartiksngh.github.io/vistas/) redirects here.

An interactive, hosted dashboard: NSE total-return indices (NAV, comparative stats,
rolling alpha/beta, rolling risk, correlation, capture, calendar-year, monthly
heatmap, distributions), a per-company **Fundamentals** tab, and an India-first
**Macro** tab (CPI/WPI/core inflation, policy & market rates, the G-sec curve,
money & credit, forex reserves, market internals, derived signals). Analytics
recompute in the browser; per-symbol data is fetched on demand.

## How it stays fresh

Published by **`Refresh Vistas Terminal.bat`** (`publish_terminal.py`) on the
author's machine. One run: pull latest data → rebuild the hosted site →
**validate** it renders with no errors → only then push here (a faulty build is
never published). GitHub Pages serves it within ~1 minute.

## Layout

- `terminal/` — the published hosted terminal (shell + per-symbol data).
- `index.html` — redirects to `terminal/`.
