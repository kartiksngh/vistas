# Vistas

A self-hosted, Bloomberg-style analytics terminal for NSE indices.

## Live deck (shareable link)

**Passive terminal → https://kartiksngh.github.io/vistas/passive/**

Open it in any browser. It is a **fully self-contained, interactive** dashboard —
pick any indices and benchmarks, any date window, daily/weekly, excess/Jensen
alpha, and every panel (NAV, comparative stats, rolling alpha/beta, rolling risk,
correlation matrix, capture, calendar-year, monthly heatmap, return/alpha
distributions) recomputes **in the browser**. No server, no install, works
offline once loaded. Built from NSE total-return (dividends-reinvested) index
levels — public market data only.

## How it stays fresh

This repo is published by **`Refresh Vistas Passive.bat`** (in the Vistas-passive
app folder on the author's machine). One double-click:
1. pulls the latest NSE data,
2. rebuilds the deck,
3. **validates** that it renders with no errors, and
4. only then pushes here — so this link is always a *working* deck (a faulty
   rebuild is never published; the previous good deck stays live).

GitHub Pages serves it within ~1 minute of each push.

## Layout

- `passive/index.html` — the published passive deck (the live link above).
- `active/` — mutual-fund terminal (planned).
