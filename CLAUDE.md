# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static marketing website for **Alas de Angel Express** — a Florida-based premium taxi, airport pickup, and express delivery service. Single-page site with no build system or framework.

## Architecture

- **`index.html`** — Entire site in one file: HTML structure, embedded `<style>` CSS, and `<script>` JS at the bottom. No external CSS/JS files.
- **`assets/`** — Images (JPG stock photos, SVG logo) and the original PNG logo for reference.

### CSS Organization (inside `<style>`)
Sections are marked with `/* ---- SECTION NAME ---- */` comments: buttons, animations, header, hero, trust bar, services, booking, about, coverage, testimonials, FAQ, footer, mobile bar, responsive breakpoints.

### JS Features (inside `<script>`)
- Header scroll effect (transparent → solid)
- Hamburger mobile menu toggle
- IntersectionObserver for `.reveal` scroll animations
- FAQ accordion (single-open)
- Animated stat counters (`data-count` attributes)

## Key Design System

CSS custom properties in `:root`:
- Colors: `--navy` (#0a1628), `--gold` (#c9a84c), `--cream` (#faf8f4)
- Typography: DM Serif Display (headings), Plus Jakarta Sans (body) via Google Fonts
- The `.gold-text` class applies a gradient background-clip text effect

## Development

No build step. Open `index.html` directly in a browser:
```
open index.html
```

## Brand Details

- Phone: (786) 967-3504 | tel:+17869673504
- WhatsApp: https://wa.me/17869673504
- Logo: Delivery truck with angel wings (`assets/logo.svg` — gold/navy SVG version; `assets/original-logo.png` — original white-on-blue)
- Service areas: Miami, Fort Lauderdale, Orlando, Tampa, Jacksonville, and statewide Florida

## GitHub

- Remote: `origin` on GitHub (`gh repo view` for URL)
- Single `main` branch, no CI/CD configured
