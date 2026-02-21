# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static personal academic homepage for Wending Gao, hosted on GitHub Pages at `wendinggao.github.io`. No build system, bundler, or package manager — the site is plain HTML + CSS served directly.

## Architecture

- **`index.html`** — Single-page site with all content. Sections: navigation, hero/about, education, experience, publications, skills, contact, footer. Contains inline `<script>` at the bottom for mobile nav toggle, smooth scroll, and scroll-based navbar styling.
- **`style.css`** — All styles. Uses CSS custom properties (`:root` variables) for theming (colors, fonts, shadows). Responsive breakpoint at 768px. Fonts loaded from Google Fonts: Crimson Text (serif, headings) and Source Sans 3 (sans-serif, body).

## Development

No build or test commands. To preview locally, open `index.html` in a browser or use any static file server (e.g., `python3 -m http.server`).

## Deployment

Push to `main` branch — GitHub Pages serves the site automatically from the repository root.

## Style Conventions

- CSS follows a section-comment pattern (`/* ===== Section Name ===== */`)
- Color palette defined via CSS custom properties: `--primary` (dark blue), `--accent` (red), `--text`, `--bg`, `--border`
- Layout uses flexbox and CSS grid; max-width container is 900px
- Many content sections use placeholder text (e.g., "20XX", "University Name") — these are templates to be filled in with real data
