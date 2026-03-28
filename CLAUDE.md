# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Static portfolio website for John Hicks, freelance media composer. Deployed via GitHub Pages at johnhickscomposer.com. No build tools — push to `main` deploys.

## Development

No build, lint, or test commands. Edit `index.html` and `main.css` directly. Preview locally by opening `index.html` in a browser.

## Architecture

Single-page scrolling site. All content lives in `index.html`; all custom styling in `main.css`.

**External dependencies (all via CDN):**
- Bootstrap 5.3.3 (layout + components)
- Font Awesome (kit `75d3d70df0`) — social icons
- Google Fonts — Baumans typeface
- ReelCrafter — embedded music reel players
- YouTube (`youtube-nocookie.com` iframes) — film/theatre work

**Page sections (by anchor ID):**
- `#jhc_home` — header, logo, social links, testimonial
- `#jhc_bio` — bio text and portrait photos
- `#jhc_reels` — ReelCrafter embeds
- `#jhc_games` — game portfolio (itch.io projects)
- `#jhc_projects` — YouTube film/theatre embeds
- `#jhc_footer` — company info

## CSS Conventions

Custom classes use `jhc-` prefix (e.g. `.jhc-container`, `.jhc-button`, `.jhc-reel-embed`). Colour palette: dark backgrounds `#212529`/`#17191c`, purple accents `#4e027a`/`#a66bd7`, red hover `#e53d3d`.