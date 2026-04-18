# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal portfolio website for Tzach Cohen — a static single-page site based on the "Dimension" template by HTML5 UP. The site presents modal-style article pages (About, Experience, Projects) triggered by hash-based navigation.

## Architecture

- **`index.html`** — The entire site lives in one HTML file. Content sections are `<article>` elements inside `#main`, shown/hidden via JS based on URL hash fragments (`#about`, `#exp`, `#projects`).
- **`assets/js/main.js`** — Core navigation logic using jQuery. Handles article show/hide transitions with `$main._show(id)` / `$main._hide()`, hash change routing, and keyboard (Escape) support.
- **`assets/sass/`** — SCSS source organized into `base/`, `components/`, `layout/`, and `libs/` directories. Entry point is `main.scss`.
- **`assets/css/main.css`** — Compiled CSS (served directly). Uses a custom font "BitPotion" (mapped to `Stepalange-x3BLm.otf`).
- **`images/`** — Static images including project GIFs and background assets.

## Development

This is a static site with no build system, package manager, or test framework. To develop:

- Open `index.html` directly in a browser, or serve with any static file server
- CSS is pre-compiled in `assets/css/main.css`; the SCSS sources in `assets/sass/` are present but there is no configured build step to compile them
- Custom font face is declared in `main.css` (not in the SCSS)

## Key Details

- Licensed under CCA 3.0 (HTML5 UP template license)
- Uses jQuery, Font Awesome 5, and custom breakpoint/browser utility scripts
- Responsive breakpoints defined in both SCSS (`main.scss`) and JS (`main.js`)
- Inline styles are used extensively in `index.html` for font sizing
