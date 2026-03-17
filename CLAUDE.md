# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A collection of daily browser games built for Bobo, a 5-year-old. Each game is a self-contained single-page HTML/CSS/JS application (no build tools, no dependencies). Games target both desktop browsers and iPad Safari.

## Repository Structure

Each game lives in a date-prefixed directory: `YYYYMMDD_game_name/`
- `index.html` — full game (desktop), all code inline (HTML + CSS + JS in one file)
- `ipad.html` — iPad-optimized version with touch controls and fullscreen support
- `README.md` — game description and play instructions
- `screenshot.png` — title screen capture

## Running Games

Open any `index.html` directly in a browser, or serve locally for iPad:
```bash
cd <game_directory>
python3 -m http.server 8080
```
Then open `http://<mac_ip>:8080/ipad.html` on iPad.

## Design Constraints

- **Audience**: 5-year-old child. Games must be forgiving (no game-over/death states, auto-recovery, encouraging messages).
- **Zero dependencies**: Everything is vanilla HTML/CSS/JS with inline `<style>` and `<script>`. No npm, no frameworks.
- **Canvas-based rendering**: Games use `<canvas>` with the 2D context API. Audio uses Web Audio API.
- **Dual-platform**: Every game needs both `index.html` (keyboard) and `ipad.html` (touch) versions.
- **Single-file**: Each HTML file is entirely self-contained — all sprites are drawn procedurally or defined inline, no external assets.
