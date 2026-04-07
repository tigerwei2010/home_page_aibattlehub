# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static landing page for **AI Battle, Inc.** — a single-page site hosted on GitHub Pages at `aibattlehub.com`.

## Tech Stack

- Pure HTML/CSS/JavaScript (no frameworks, no build system, no package manager)
- GitHub Pages for hosting (configured via `CNAME`)

## Architecture

The entire site is a single `index.html` file containing inline CSS and minimal JS. There is no build step, no bundler, and no dependencies.

- `index.html` — all markup, styles, and scripts
- `logo_200.png` — logo (also used as favicon)
- `use_this.jpg` — hero background image (animated via CSS `kenBurns`)
- `CNAME` — GitHub Pages custom domain (`aibattlehub.com`)

## Development

No build or install commands. Open `index.html` in a browser to preview. Changes deploy automatically when pushed to `main` via GitHub Pages.

## Design System

CSS custom properties defined in `:root`:
- `--primary: #f5a623` (orange accent)
- `--glow: rgba(245,166,35,.6)`
- `--bg: #0a0e17` (dark background)
- `--surface: rgba(255,255,255,.04)`

Key visual effects: Ken Burns background animation, floating particles (JS-generated), backdrop-filter glass effects, staggered `fadeSlideUp` entrance animations.

## Conventions

- All styles are inline in `<style>` within `index.html` (no external CSS files)
- Responsive breakpoint at 600px
- Fluid typography using `clamp()`
