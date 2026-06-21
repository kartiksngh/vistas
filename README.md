# Vistas

A self-hosted, Bloomberg-style analytics terminal for NSE indices, stocks and India macro.

## Live links

- **Terminal (current — the main product) → https://kartiksngh.github.io/vistas/terminal/**
- **Passive (legacy self-contained deck — RETAINED as a live-data source for the FFT project)
  → https://kartiksngh.github.io/vistas/passive/**

The bare URL (https://kartiksngh.github.io/vistas/) redirects to the terminal.

The **terminal** is the hosted hybrid site (Performance + Fundamentals + Macro tabs; per-symbol
data fetched on demand). The **passive** deck is the original self-contained Performance-only deck —
kept and untouched because a separate ongoing project consumes its data.

## How it stays fresh

- Terminal: `Refresh Vistas Terminal.bat` (`publish_terminal.py`).
- Passive:  `Refresh Vistas Passive.bat` (`publish_passive.py`).

Each pulls data → rebuilds → validates (Node runtime smoke-test) → publishes only if it renders cleanly.

## Layout

- `terminal/` — the hosted terminal (shell + per-symbol data).
- `passive/index.html` — the retained passive deck.
- `index.html` — redirects to `terminal/`.
